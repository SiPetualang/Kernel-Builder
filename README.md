# Generic Kernel Image Manual

> Please read this manual carefully and use it with guidance from Google.

**【Kernel Name】**

    Common Name: Generic Kernel Image
    English Name: Generic Kernel Image
    Chinese Pinyin: Tongyong Neihe Yingxiang

**【Components】**

https://kernel.org/

https://kernelsu.org/

**【Form】**

This product is a compressed archive within another archive file. SHA256 checksum is noted beside the download link.

**【Supported Devices】**

Phones compatible with GKI.

**【Adverse Reactions】**

常见：发热。偶见：死机。罕见：黑砖。

**【注意事项】**

本内核安全补丁级别来自 KernelSU workflow 的最新设定。

请在安装此项目的内核前，启动一次官方或者 5ec1cff 的 KernelSU，进入系统后打开 KernelSU 管理器，进入设置，**关闭全局 umount**。这是为了防止 susfs 对 umount 的应用处理导致系统应用出现问题。可能出现的现象包括但不限于：

- 启动后黑屏（SystemUI 无法加载）
- Wi-Fi 无法访问
- 基带有关通讯无法访问

**【核代动力学】**

对 Pixel 8 进行了通用内核映像的核代动力学研究。可以启动。

> **软件相互作用**
>
> 质感清理：susFS 与质感清理合并使用时，两者的核代动力学和核效学存在相互作用。在 susFS 上市后，曾有报道使用质感清理的用户反馈 umount 的 app 显示剩余空间 0B 的情况。此外，因为此事带来的连带效应包括微信小程序不能启动。

**【储藏】** 任意条件。

**【包装】** 压缩包文件。
