---
title: "finally get ares-sc2 bot running on macos with M3 / arm64 chip"
date: 2024-11-04
---

so many kengs

first i have uninstall rye, and install pyenv, install poetry // poetry keep complaining python version errors.

uninstall rye: <a href="https://mac.install.guide/python/install-rye">https://mac.install.guide/python/install-rye</a>. // scroll to the end

pyenv and poetry: <a href="https://dev.to/mattcale/pyenv-poetry-bffs-20k6">https://dev.to/mattcale/pyenv-poetry-bffs-20k6</a>

remember add path &quot;export PATH=&quot;$HOME/.local/bin:$PATH&quot;&quot;

pyenv install 3.11 // the ares-sc2 bot specified version to be &gt;=3.11 and &lt;3.12.

when running poetry install

got error: &quot;Installing cython-extensions-sc2 (0.4.4): Failed Error -3 while decompressing data: invalid distance too far back&quot;

the error is because the package is built on linux not mac

to fix this,

go ares-sc2/pyproject.toml, comment out cython-extensions-sc2 = &quot;^0.4.0&quot;, and add cython-extensions-sc2 = { git = &quot;<a href="https://github.com/AresSC2/cython-extensions-sc2.git">https://github.com/AresSC2/cython-extensions-sc2.git</a>&quot;}

then poetry lock --no-update and poetry install --sync

now if we run &quot;poetry run python run.py&quot;

got another error: &quot;ModuleNotFoundError: No module named 'pkg_resources'&quot;

to fix it, poetry add setuptools

run again

ImportError: dlopen(/Users/ferryzhou/.pyenv/versions/3.11.10/lib/python3.11/lib-dynload/_<a href="http://lzma.cpython-311-darwin.so">lzma.cpython-311-darwin.so</a>, 0x0002): Library not loaded: /opt/homebrew/opt/xz/lib/liblzma.5.dylib

brew install xz

run again

ImportError: dlopen(/Users/ferryzhou/Projects/sc2_bots_ares/ares-sc2/sc2_helper/<a href="">sc2_helper.cpython-311-darwin.so</a>, 0x0002): tried: '/Users/ferryzhou/Projects/sc2_bots_ares/ares-sc2/sc2_helper/<a href="">sc2_helper.cpython-311-darwin.so</a>' (mach-o file, but is an incompatible architecture (have 'x86_64', need 'arm64e' or 'arm64'))

ok. my macbook pro 2023 is on M3, which use arm64

git clone <a href="https://github.com/danielvschoor/sc2-helper.git">https://github.com/danielvschoor/sc2-helper.git</a>

install cargo

curl --proto '=https' --tlsv1.2 -sSf <a href="https://sh.rustup.rs">https://sh.rustup.rs</a> | sh

add $HOME/.cargo/bin to path

cargo build

lots errors

warp suggested it's because some env variables not set

added the following

export PYTHON_INCLUDE_DIR=$(python -c &quot;from distutils import sysconfig; print(sysconfig.get_python_inc())&quot;)

export PYTHON_LIB_DIR=$(python -c &quot;import sysconfig; print(sysconfig.get_config_var('LIBDIR'))&quot;)

same error, noticed &quot;pyo3_ffi::boolobject::Py_True::hfb8b6c031c344b01 in libpyo3-4a88edf5219064d6.rlib[18](pyo3-4a88edf5219064d6.pyo3.e69fa0d4dd690b81-cgu.15.rcgu.o)
ld: symbol(s) not found for architecture arm64&quot;

searched google with &quot;pyo3 cargo build arm64&quot;

found solution <a href="https://github.com/PyO3/rust-numpy/issues/223">https://github.com/PyO3/rust-numpy/issues/223</a>

create ~/.cargo/config.toml

<pre><code>[target.aarch64-apple-darwin] rustflags = [
&quot;-C&quot;, &quot;link-arg=-undefined&quot;,
&quot;-C&quot;, &quot;link-arg=dynamic_lookup&quot;,
]</code></pre>
cargo build --manifest-path /Users/ferryzhou/Projects/sc2-helper/Cargo.toml --verbose

now succeed

cargo build --manifest-path /Users/ferryzhou/Projects/sc2-helper/Cargo.toml --release

ls -l /Users/ferryzhou/Projects/sc2-helper/target/release

we can see libsc2_helper.dylib

now swap the lib file

mv ares-sc2/sc2_helper/<a href="">sc2_helper.cpython-311-darwin.so</a> ares-sc2/sc2_helper/sc2_helper.cpython-311-darwin.so.x86_64

cp target/release/libsc2_helper.dylib ../sc2_bots_ares/ares-sc2/sc2_helper/<a href="">sc2_helper.cpython-311-darwin.so</a>

poetry run python run.py

raise IndexError('Cannot choose from an empty sequence')

maps problem

open run.py, change path from windows to mac sc2 maps path

#MAPS_PATH: str = &quot;C:\\Program Files (x86)\\StarCraft II\\Maps&quot;
MAPS_PATH: str = &quot;/Applications/StarCraft II/Maps&quot;

run again, and now it succeeded!!!

poetry run python run.py
Starting local game...
