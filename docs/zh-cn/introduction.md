# 介绍

太极是一个能够运行 Xposed 模块的框架，模块能通过它改变系统和应用的行为。太极既能以传统的 Root/刷机方式运作，也能免 Root/ 免刷机运行；并且它支持 Android 5.0 ~ **9.0**。

简单来说，太极就是一个 **类Xposed**框架，它能够加载 Xposed 模块、修改系统和APP、拦截方法，执行 hook 逻辑等。

# 特性

虽然太极是一个 类Xposed 框架，但是它本身与 Xposed 没有任何关系。唯一有点关系的可能是太极能够兼容 Xposed 模块，除此之外，二者从设计思路、实现机制到运作逻辑完全不同。

以下是太极一些独有的特性：

1. 太极**完全支持 Android 9.0**。
2. 太极能**以免 Root/免刷机模式运行**。
3. 太极**不影响全局**。可以只对特定的应用开启 Xposed 功能，无需使用 Xposed 的 APP 运行起来就跟系统没有 Xposed 一样；这意味着太极能轻松绕过SafetyNet检测，完美契合某些金融/银行/奇葩类APP。
4. 在大部分情况下，太极中的模块**无需重启即刻生效**。
5. 太极更**不易被检测**。太极的弱侵入特性不再修改 ART 运行时，也不在全局环境中留下任何踪影；因此只要想要做到，可以轻松逃过各种代码类型的检测。