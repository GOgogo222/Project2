
## 12_20

使用的版本：18.0.0

[【保姆级图文教程】最新Windows系统QT下载、安装、入门、配置VS Qt环境，图文详细、内容充实-CSDN博客](https://blog.csdn.net/qq_62888264/article/details/132645054)

在VS Code中创建Qt项目

Qt教程：
https://www.bilibili.com/video/BV1g4411H78N?t=1072.5&p=4

## 1_04 创建第一个Qt程序

**主要熟悉了一个Qt程序的创建过程**

**主要学习了初始代码的部分，为它们写上了简明的注释**

********
- **`QWidget`** 是 Qt 所有界面元素的**基类（祖先）**。
    
- 你的 `MyPro01` 继承自 `QMainWindow`（而 `QMainWindow` 又继承自 `QWidget`）。
    
- **结论：** `QWidget` 才是父类，`MyPro01` 是子类。