# 实验目的

熟悉R以及RStudio的基本环境

# 实验原理

R是一套完整的数据处理、计算和制图软件系统。其功能包括：数据存储和处理系统；数组运算工具（其向量、矩阵运算方面功能尤其强大）；完整连贯的统计分析工具；优秀的统计制图功能；简便而强大的编程语言：可操纵数据的输入和输出以及可实现分支、循环等用户自定义功能。R不仅是一种统计软件，而且是一种数学计算的环境，因为R不仅仅提供若干统计程序、使用者只需指定数据库和若干参数便可进行统计分析。R的思想是：它可以提供一些集成的统计工具，但更大量的是它提供各种数学计算、统计计算的函数，从而使使用者能灵活地进行数据分析，甚至创造出符合需要的新的统计计算方法。

# 实验步骤 

R可以在[CRAN](http://cran.r-project.org/)（Comprehensive R Archive Network）上免费下载。此外，为了提高书写和执行的简便性以及方便用户调试程序，可以下载GUI（图形用户界面）来使用，比较流行的诸如R Commander， Rattle， RStudio等，本教程主要介绍RStudio。

点击屏幕右上角Application Menu -&gt; development -&gt; rstudio,打开实验环境

RStudio界面的概览如下图所示：

![](https://kfcoding-static.oss-cn-hangzhou.aliyuncs.com/gitcourse-bigdata/1-1-1-1_20171107060508.008.jpg)

如上图所示，RStudio分为4个区域，分别是：

* Scripts：书写和保存R代码的地方
* Environment：列出R环境中的数据集和变量
* Plots：显示图像和导出图像
* Console：显示执行R语句的历史信息和输出，获得帮助信息

R语言的语法简单明了，例如，在Console输入语句plot\(AirPassengers\)可以在Plots输出折线图：
![](https://kfcoding-static.oss-cn-hangzhou.aliyuncs.com/gitcourse-bigdata/1-1-1-2_20171107060834.034.png)
在Console输入语句hist\(mtcars$mpg\)可以在Plots输出直方图：

![](https://kfcoding-static.oss-cn-hangzhou.aliyuncs.com/gitcourse-bigdata/1-1-1-3_20171107060934.034.png)