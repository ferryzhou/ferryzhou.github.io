---
title: "raspberry pi 4 hdmi no audio"
date: 2022-07-22
---

right click sound icon, choose hdmi

if issue fixed, stop here

otherwise

enter root mode

$sudo su

uncomment hdmi_drive = 2 in /boot/config.txt

$reboot
