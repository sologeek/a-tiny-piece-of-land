---
title: 准备工作
---
在开始学习 Chibicc 编译器之前，我们需要了解以下知识：

1. C 编译器的工作原理
2. 汇编语言基础
3. Makefile 使用
4. Shell 使用

## C 编译器的工作原理

1. 编译时，`.c` 源文件被编译成中间目标文件，Windows 平台下为 `.obj`，Unix 平台下为 `.o`，通常情况下，一个源文件对应一个 `.o` 的中间目标文件。
2. 链接时，主要链接函数和全局变量。我们是使用中间目标文件来链接我们的应用程序，链接器只管中间目标文件。大多数时候，中间目标文件很多，会将它们进行一个打包，在 Windows 平台下，这种包称为 ”库文件“（Library File），也就是 `.lib` 文件，在 Unix 下，是 Archive File，也就是 `.a` 文件。
3. 总结，编译工作过程首先将源文件生成中间目标文件，再由中间目标文件生成可执行文件。
## 汇编语言基础

## Makefile 使用

Chibicc 项目使用 Makefile 进行构建和单元测试等自动化流程，可以参考 [[Development-Tools/Makefile/Oveview|Makefile 学习]] ，了解如何使用 Makefile。

## Shell 使用

Makefile 中执行脚本为 Shell，可以参考 [[Development-Tools/Shell/Oveview]]
