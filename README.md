# rustbao

This project is a Rust version of [bao-demos](https://github.com/bao-project/bao-demos)

## 概述

针对嵌入式平台的静态分区Hypervisor有Jailhouse和Bao。与Jailhouse不同，Bao是Type-1 Hypervisor，意味着它不需要依赖其他的操作系统来启动。目前Bao支持ARM-v8和RISC-V架构。

## 如何运行rustbao

1. 运行make run，在qemu中启动rust-bao，一开始会进入uboot
2. 在uboot命令行中输入go 0x50000000进入rustbao的镜像执行
