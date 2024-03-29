# 实验目的

熟悉R语言包的安装、载入及使用方法
 
# 实验原理

包是R函数、数据、预编译代码以一种定义完善的格式组成的集合。计算机上存储包的目录称为库（library）。函数.libPaths\(\)能够显示库所在的位置，函数library\(\)则可以显示库中有哪些包。

R自带了一系列默认包（包括base、datasets、utils、grDevices、graphics、stats以及methods），它们提供了种类繁多的默认函数和数据集。其他包可通过下载来进行安装。安装好以后，它们必须被载入到会话中才能使用。命令search\(\)可以告诉你哪些包已加载并可使用。

# 实验步骤

双击桌面的“rstudio”图标，打开实验环境。
登录，Username和Password都是guest。

## 1、包的安装

有许多R函数可以用来管理包。第一次安装一个包，使用命令install.packages\(\)即可。查询自己想安装的包的名称，可以直接将包名作为参数提供给这个函数。例如，包gclus中提供了建增强型散点图的函数。可以使用命令install.packages\("gclus"\)来下载和安装它。一个包仅需安装一次。但和其他软件类似，包经常被其作者更新。使用命令update.packages\(\)可以更新已经安装的包。同时，也可以在RStudio右下方点击packages，再点击install，在对话框中输入包名下载安装包。

代码install.packages\("e1071"\)表示安装包e1071：
![](/images/1-1-2-1.png)

## 2、包的载入

包的安装是指从某个CRAN镜像站点下载它并将其放入库中的过程。要在R会话中使用它，还需要使用library\(\)命令载入这个包。例如，要使用gclus包，执行命令library\(gclus\)即可。当然，在载入一个包之前必须已经安装了这个包。在一个会话中，包只需载入一次。如果需要，你可以自定义启动环境以自动载入会频繁使用的那些包。
![](/images/1-1-2-2.png)

## 3、包的使用方法

载入一个包之后，就可以使用一系列新的函数和数据集了。包中往往提供了演示性的小型数据集和示例代码，能够让我们尝试这些新功能。帮助系统包含了每个函数的一个描述（同时带有示例），每个数据集的信息也被包括其中。命令help\(package="package\_name"\)可以输出某个包的简短描述以及包中的函数名称和数据集名称的列表。使用函数help\(\)可以查看其中任意函数或数据集的更多细节。这些信息也能以PDF帮助手册的形式从CRAN下载。

例如代码help\(package="ggplot2"\)可以输出包ggplot2的信息：
![](/images/1-1-2-3.png)
