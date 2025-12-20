
## 12_20

使用的版本：18.0.0

[【保姆级图文教程】最新Windows系统QT下载、安装、入门、配置VS Qt环境，图文详细、内容充实-CSDN博客](https://blog.csdn.net/qq_62888264/article/details/132645054)

在VS Code中创建Qt项目

Qt教程：
https://www.bilibili.com/video/BV1g4411H78N?t=1072.5&p=4

## 1_04 创建第一个Qt程序

**主要熟悉了一个Qt程序的创建过程**

**主要学习了main函数的主要内容，为它们写上了简明的注释**

********
- **`QWidget`** 是 Qt 所有界面元素的**基类（祖先）**。
    
- 你的 `MyPro01` 继承自 `QMainWindow`（而 `QMainWindow` 又继承自 `QWidget`）。
    
- **结论：** `QWidget` 才是父类，`MyPro01` 是子类。

## 1_05 

Qt模块的认识。。。(Qt Modules)

- core；gui；widgets
- network；multimedia；networkauth；multimediawidgets（主要用于app联网和媒体播放功能）

.pro文件介绍：
**.pro就是工程文件（project），它是qmake自动生成的用于生产makefile的配置文件**

一个 .pro 文件所包含的东西：
模块（Moudles），生成的 **.exe** 文件的名称，模板（Template），源文件，头文件

“相当于我自己写了一个类（MyPro01），继承了QWidget的窗口类”

**注意，类名和变量名要控制大小写**

*********
应用程序模板：
在 Qt 项目的 `.pro` 文件中，**应用程序模板（TEMPLATE）** 是一个非常关键的变量。它告诉 Qt 的构建工具 `qmake`：“**这个项目最终要生成一个什么东西？**”
*——Gemini*

继承QMainWindow类：
class MyPro01 : public QMainWindow（`QMainWindow` 是 Qt 官方写好的一个“标准主窗口”。通过 `: public`，你的 `MyPro01` 自动拥有了主窗口的所有功能 ）
*——Gemini*

## 学习Qt Designer

https://www.bilibili.com/video/BV12B4y1h7QX?t=682.2

**Frame**的布局

**stytleSheet**的基础语法

多个 **Widgets** 的布局

**Ctrl+R**：预览效果






