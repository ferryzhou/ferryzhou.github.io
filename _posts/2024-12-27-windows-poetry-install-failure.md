---
title: "windows poetry install failure"
date: 2024-12-27
---

- Installing jedi (0.19.2): Failed

FileNotFoundError

[Errno 2] No such file or directory: 'C:\\Users\\ferry\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.12_qbz5n2kfra8p0\\LocalCache\\Local\\pypoetry\\Cache\\virtualenvs\\ares-sc2-Uaf6fc_c-py3.10\\Lib\\site-packages\\jedi\\third_party\\django-stubs\\django-stubs\\contrib\\admin\\templatetags\\admin_list.pyi'

at C:\Program Files\WindowsApps\PythonSoftwareFoundation.Python.3.12_3.12.2288.0_x64__qbz5n2kfra8p0\Lib\pathlib.py:1013 in open

search google &quot;what is WindowsApps\PythonSoftwareFoundation&quot;

WindowsApps\PythonSoftwareFoundation is the installation location for Microsoft Store apps on Windows.

follow the first link <a href="https://github.com/python-poetry/install.python-poetry.org/issues/135">https://github.com/python-poetry/install.python-poetry.org/issues/135</a>

someone suggests poetry config cache-dir C:\Users\username\pypoetry

it works!

// previously i tried remove env, change py version, blabla and all of it does not work.
