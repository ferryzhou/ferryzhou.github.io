---
title: "Nerf 3d reconstruction"
date: 2024-09-27
---

<a href="https://github.com/bmild/nerf?tab=readme-ov-file">https://github.com/bmild/nerf?tab=readme-ov-file</a>

以前也做过3d reconstruction

今天听一个访谈

<a href="https://github.com/bmild/nerf?tab=readme-ov-file">https://github.com/bmild/nerf?tab=readme-ov-file</a>

提到这玩意儿

感觉有点意思

看了一下paper

又是一个用deep neural network来解决具体问题的case

input是三维空间坐标和视角

output是图像三维颜色和density

完全不需要我以前搞的什么multi view geometry

一个神经网络加一堆的训练数据直接搞定。
