# 明安里市工具箱 Ming'anli City Toolbox

一款自由、开源，适用于明安里市各类作品作者的工具箱。基于 [Python](https://www.python.org/) 和 [PyQt5](https://pypi.org/project/PyQt5/)。

项目仍在开发中，敬请期待。

## 目录

- [安装](#安装)
- [用法](#用法)
- [相关项目](#相关项目)
- [主要项目负责人](#主要项目负责人)
- [参与贡献方式](#参与贡献方式)
    - [贡献人员](#贡献人员)
- [开源协议](#开源协议)


## 安装

对于 Windows 用户，可以直接到 Releases 下载预编译版本的安装程序，运行安装程序，待安装完毕后即可直接使用。

对于 GNU/Linux 用户，下载对应发行版的软件包后直接执行软件包安装命令，待安装完成后即可直接使用。

## 用法

普通用户可以查看项目文档，了解详细的使用方法。

如果你是爱折腾的开发者，对本项目做了修改，可以用下面的方法自行编译（以 Windows 平台为例）：

1.在运行环境安装依赖

```
pip install pywin32
pip install PyInstaller
pip install PyQt5
pip install qrcode
pip install barcode
pip install "PyQt-Fluent-Widgets[full]"
```

这里还应包括你自行添加的依赖。需要注意，`PyQt-Fluent-Widgets`必须按照给出的命令安装完整版，否则编译会出错。这是由于`AcrylicLabel`在非完整版中不可用，而项目正好使用了它。

2.开始编译

转到包含源代码的文件夹，然后执行下面的命令：

`pyinstaller -w main.py `

转到`dist`文件夹，直接运行测试。如果你想编译一个单文件版本（网民俗称“绿色版”），可以执行：

`pyinstaller -F -w main.py `

## 相关项目

项目使用了[之一Yo](https://github.com/zhiyiYo)的[PyQt-Fluent-Widgets](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)作为 GUI 框架。

项目的“明安里市特殊市民身份识别码生成”功能，有单独的仓库维护控制台版本：[MinganliCity_SCIDGenerator](https://github.com/Diamochang/MinganliCity_SCIDGenerator)

## 主要项目负责人

[Diamochang (Mike Wang)](https://github.com/Diamochang)

## 参与贡献方式

提交 [PR](https://github.com/Diamochang/MinganliCity_Toolbox/pulls) 申请，我会视情况通过。

### 贡献人员

感谢所有贡献者对本项目的支持。

[Diamochang (Mike Wang)](https://github.com/Diamochang)

## 开源协议

项目遵循[GNU 通用公共许可证 第三版](LICENSE)。
