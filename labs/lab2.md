# Lab : system call

syscall

在上一个实验中，您使用系统调用编写了一些实用程序。在本实验室中，您将向xv6添加一些新的系统调用，这将帮助您了解它们是如何工作的，并使您了解xv6内核的一些内部结构。您将在以后的实验中添加更多系统调用。

> 在你开始写代码之前，请阅读xv6手册《book-riscv-rev1》的第2章、第4章的第4.3节和第4.4节以及相关源代码文件：
>
> + 系统调用的用户空间代码在**user/user.h**和**user/usys.pl**中。()
> + 内核空间代码是**kernel/syscall.h**、**kernel/syscall.c**。()
> + 与进程相关的代码是**kernel/proc.h**和**kernel/proc.c**。()

要开始本章实验，请将代码切换到**syscall**分支：

```shell
$ git fetch
$ git checkout syscall
$ make clean
```

如果运行`make grade`，您将看到测试分数的脚本无法执行`trace`和`sysinfotest`。您的工作是添加必要的系统调用和存根（stubs）以使它们工作。

---

## 1.System call tracing（moderate）













