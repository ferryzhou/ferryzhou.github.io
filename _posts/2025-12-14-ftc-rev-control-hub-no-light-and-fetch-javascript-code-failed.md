---
title: "ftc rev control hub no light and fetch javascript code failed"
date: 2025-12-14
---

website can connected, but cannot create op modes. button seems disabled.

fixed by

1) install REV Hardware Client (seems windows only) <a href="https://docs.revrobotics.com/rev-hardware-client">https://docs.revrobotics.com/rev-hardware-client</a>

2) connect hub to pc with usb. // power on hub of course

3) scan and open the hub in the client

4) update controller app

restart and everything worked again

the root cause is that when we uploading an app apk through website, the hub loses power so data/code is not completed.

note that connect hub to pc with usb, not wifi.
