# <center>Kubernetes 安装</center>

搭建Kubernetes集群环境有以下三种方式：

一：minikube

Minikube是一个工具，可以在本地快速运行一个单点的Kubernetes，尝试Kubernetes或日常开发的用户使用。不能用于生产环境。

二：kubeadm

Kubeadm也是一个工具，提供kubeadm init和kubeadm join，用于快速部署Kubernetes集群。

三：二进制包

从官方下载发行版的二进制包，手动部署每个组件，组成Kubernetes集群。

我们选择kubeadm安装方式来快速部署kubernetes集群。

---

0.环境说明

主机名 | IP地址 | 说明
---|---|---
txl-ubuntu-18-10-master0 | 192.168.100.10 | master节点
txl-ubuntu-18-10-node0 | 192.168.100.20 | node节点

==注：本次旨在演示kubernetes安装过程，因此选择1master和1node来进行实操，高可用集群会在后续文章中探讨==