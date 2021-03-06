# PDF 类库比较
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ShiningRush/PdfComponentComparition/blob/master/LICENSE)

该Demo的目的是为了比较各个组件对Pdf文件支持功能的转化质量，性能以及语法简洁度做对比。同时大家也可以把该Demo作为一个组件使用方法的参考文档。

## 概述

该Demo目前只实现了几种类库（Aspose.Pdf, Spire.Pdf, iText7），其中包含一些商业组件，为什么不多选择一些开源免费的？其实功能最全的，都是收费了，而且开源中最有名的组件应该就属iTextSharp了吧。这里稍微解释一下，iText5是Java系里很有名的Pdf开源类库，而iTextSharp就是它的.Net版本，然后他们重写了iText5，为了拥有更简洁的语法和可修改性。所以我在开源类库中只选择了iText7作为一个研究对象。

不过本Demo的组件调用都采用了接口以达到良好的拓展性，有兴趣的同学可以自己拓展自己感兴趣的组件和想实现的功能。

只要实现 `IPdfComponentFunc` 接口，程序会自动将该实现加载到下拉列表。

## Demo用法简单介绍

`UseComponent` 这个下拉列表用来选择用于转换的组件

`InputFileDir` 选择你需要转换的文件所在文件夹，请注意是所在文件夹，而且不是文件

`OutputFIleDir` 选择你操作后要输出的文件夹路径

`ExecuteTimes` 执行次数，用于性能对比时使用，为空默认执行1次

下面几个按钮应该相当容易懂了，这里只解释一下 `AllRun` 按钮就是说将所有功能都跑一遍。
