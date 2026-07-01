# Fuse文件系统


FUSE（Filesystem in Userspace）是一个允许用户在用户态创建自定义文件系统的接口，诞生于 2001 年。FUSE 的出现大大降低了文件系统开发的门槛，使得开发者能够在不修改内核代码的情况下实现创新的文件系统功能

为了更好地理解 FUSE 的设计理念，我们将首先回顾内核文件系统以及网络文件系统（如 NFS）的发展历程，这些技术的演进为 FUSE 实现用户空间文件系统功能奠定了重要基础。









## 参考

- [Libfuse GitHub](https://github.com/libfuse/libfuse)

- [FUSE - 从内核到用户态文件系统的设计之路](https://juicefs.com/zh-cn/blog/engineering/fuse-file-system-design)
