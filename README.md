# Android 框架层源码分析

写在前面

>之前看过很多Android框架层的源码以及分析源码的书籍，但都是零零散散的不成系统，作为一个 Android 开发人员，
自上而下的 Android 底层源码的功力还是很重要的，从今天开始我就对整个 Andriod 框架层的源码和原理做个系统的
分析，虽然 对于 Android 源码的分析，很多前辈都写过，但之所以会有这个系列的文章，一来 Android 的源码也在
不断的变化目前已经到 Android 7.0 Nougat，本系列文章会针对最新的代码进行分析，二来就是源码分析的过程是比
较枯燥的，本系列的文章会一种独特的视角来减轻大家在阅读源码时的负担，好了，让我们开始吧。

这是本系列博客的第一篇文章，后续的每篇文章都会配上详尽的类图、时序图、示例代码，每大章节还是设立导读PPT。

Android 的源码是多名伟大工程师智慧的结晶，不可谓博大而精深，所以我们在学习之前，要掌握相关的基本技术，欲工
其事，必先利其器，我们需要掌握以下的技术。


设计模式

推荐这两本书

[Android 源码设计模式解析与实战](https://item.jd.com/11793928.html)：何红辉，关爱民 著

<img src="https://github.com/guoxiaoxing/android-framework-source-code-analysis/raw/master/art/android_source_code_design_pattern.png"/>

[Head First设计模式（中文版）](https://item.jd.com/10100236.html)：[美] 弗里曼（Freeman E.） 等 著；UML China 编；OReilly Taiwan公司 译

<img src="https://github.com/guoxiaoxing/android-framework-source-code-analysis/raw/master/art/head_first_design_pattern.png"/>
