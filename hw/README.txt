# 2.5kV USB2.0 Isolator with 400mA supply and full speed (12Mbit/s) support

* 本工程是用于验证立创商城 隔离器芯片/ ADUM3160BRWZ（商城编号C108501）的方案验证板设计。
* 本工程是 [立创EDA开源硬件平台](https://oshwhub.com/) [方案验证模块征集令](https://oshwhub.com/rewards/f4bbab6365034e80aadb8f8ebf77c846)工程。

### 简介

在台式机上，USB端口的GND信号通常位于建筑物中电气设备的GND电平上。
因此，即使USB设备具有隔离的电源并与地面隔离，该隔离也会被USB连接绕过。
在某些情况下，这是不希望的，例如 对于测量设备，可能有必要使用电路中的某些电位作为参考而不是共用接地。
此外，如果USB设备发生电气故障，则USB设备与PC之间的5V和GND线直接连接也会出现问题。
例如。 如果测量设备发生灾难性短路，则可能会损坏PC。
因此，有充分的理由使用USB隔离器-只是它们通常很昂贵。 同样，它们中的大多数不能提供连接的USB设备。
通常，您需要在USB从属端（隔离栅后面）连接电源，该电源不是很方便。

### 主要元件

* 电源模块DC-DC/ IB0505S-2W
* 隔离器芯片/ ADUM3160BRWZ
* TVS管、共模电感、磁珠

### 功能描述

* 输入采用typec接口，并带有esd防护
* 输入输出之间采用[隔离器芯片/ ](https://list.szlcsc.com/catalog/581.html "隔离器芯片")[ADUM3160BRWZ](https://item.szlcsc.com/109720.html "ADUM3160BRWZ ")隔离
* 前级通过金升阳隔离电源给后级供电
* 输出采用USB2.0 A母座接口
* 400mA输出能力（MAX）
* TL431做最低负载（40mA）
* 做了抗emi处理，添加了共模电感等器件
### 实物

![IMG_20200516_133739.jpg](//image.lceda.cn/pullimage/A0FzVTbU8QTOf9O2MhxelqNjrobbIrzh5XCb8qxo.jpeg)
![IMG_20200516_13541101.jpeg](//image.lceda.cn/pullimage/FNe7BoBBHX9uh8BG3XZXsQTfQV7rPT5gEGYLBHEP.jpeg)            
How to use：

At editor, open the document via: Top menu - File - Open - EasyEDA... , and select the json file, then open it at the editor, you can save it into a project.


如何使用：

打开编辑器，通过：顶部菜单 - 文件 - 打开 - 立创EDA... ，选择 json 文件打开在编辑器，你可以保存文档进工程里面。