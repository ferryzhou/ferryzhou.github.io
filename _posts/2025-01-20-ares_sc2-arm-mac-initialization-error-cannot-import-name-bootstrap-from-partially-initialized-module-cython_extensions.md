---
title: "ares_sc2 arm mac initialization error cannot import name 'bootstrap' from partially initialized module 'cython_extensions'"
date: 2025-01-20
---

<!-- wp:paragraph -->
<p>Traceback (most recent call last):<br>File "/bots/qin/run.py", line 18, in<br>from bot.main import MyBot<br>File "/bots/qin/bot/main.py", line 6, in<br>from ares import AresBot<br>File "/bots/qin/ares-sc2/src/ares/<strong>init</strong>.py", line 3, in<br>from .main import * # noqa: F403 F401<br>^^^^^^^^^^^^^^^^^^^<br>File "/bots/qin/ares-sc2/src/ares/main.py", line 6, in<br>from cython_extensions import cy_unit_pending<br>File "/bots/qin/cython_extensions/<strong>init</strong>.py", line 6, in<br>from . import bootstrap<br>ImportError: cannot import name 'bootstrap' from partially initialized module 'cython_extensions' (most likely due to a circular import) (/bots/qin/cython_extensions/<strong>init</strong>.py)</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Solution: </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>from <a href="https://github.com/AresSC2/cython-extensions-sc2">https://github.com/AresSC2/cython-extensions-sc2</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>click releases on the right side</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>download <a href="https://github.com/AresSC2/cython-extensions-sc2/releases/download/v0.5.0/ubuntu-latest_python3.12.zip">ubuntu-latest_python3.12.zip</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>unzip, and copy bootstrap.cpython-312-x86_64-linux-gnu.so to &lt;bot_dir&gt;/cython-extensions-sc2/cython-extensions.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>then run poetry run python scripts/create_ladder_zip.py</p>
<!-- /wp:paragraph -->
