## 最接近内核的无痕注入

> * 隐藏maps文件 -> /proc/self/maps 无痕迹
> * solist无注入so信息
> * 进程/proc/self/fd 下无链接
> * 无虚拟memfd 
> * 抹除elf头信息 无法暴力搜索elf
> * 注入进程无关联的注入文件信息；
> * inotify bypass
> * 可定义maps内存描述

## 限制
> * root环境下使用
> * magsisk下必须关闭lsposed和zygisk 还有其他修改zygote 相关的hook框架均会引起冲突


## 兼容版本
> * Android 8.0 - 14.0
## 架构支持
> * arm64-v8a
> * armeabi-v7a


## 本项目不会开源，完善加固后将以APK的形式发布
