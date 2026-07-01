# Fuse文件系统


FUSE（Filesystem in Userspace）是一个允许用户在用户态创建自定义文件系统的接口，诞生于 2001 年。FUSE 的出现大大降低了文件系统开发的门槛，使得开发者能够在不修改内核代码的情况下实现创新的文件系统功能

为了更好地理解 FUSE 的设计理念，我们将首先回顾内核文件系统以及网络文件系统（如 NFS）的发展历程，这些技术的演进为 FUSE 实现用户空间文件系统功能奠定了重要基础。


## 01 单机文件系统：内核态与VFS

文件系统作为操作系统中的核心底层组件，负责频繁操作存储设备，因此最初的设计完全在内核空间中进行。“内核”这一概念的提出，是随着计算机硬件和软件日益复杂化，操作系统将底层资源管理的代码与用户程序进行分离的产物。

内核是拥有超级权限的代码，负责管理计算机的核心资源（如 CPU、内存、硬盘、网络等）。当内核代码运行时，程序进入内核态，可以完全访问和操作这些底层设备。由于内核态权限极高，其代码必须经过严格测试和验证，普通用户无法随意修改。

而与内核空间形成对应的是用户空间（User space），这部分代码就是我们平时常见的各种应用程序，像浏览器、游戏等。在用户空间里，程序的权限是受到严格限制的，不能直接访问底层的重要资源。

![kernel-user-space](https://raw.githubusercontent.com/ivanzz1001/storage-filesystem/master/Fuse/image/fuse01-kernel_user_space.jpg)


## 02 网络文件系统 NFS：首次突破内核态


## 03 FUSE：从内核到用户态的文件系统创新



## 04 参考

- [Libfuse GitHub](https://github.com/libfuse/libfuse)

- [FUSE - 从内核到用户态文件系统的设计之路](https://juicefs.com/zh-cn/blog/engineering/fuse-file-system-design)
