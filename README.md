
# fasteR: Fast Lane to Learning R! 

![alt text](https://raw.githubusercontent.com/matloff/prVis/master/data/SwissRoll/SWwithY.png)

## *"Becoming productive in R, as fast as possible"*

### Norm Matloff, Prof. of Computer Science, UC Davis; [my bio](http://heather.cs.ucdavis.edu/matloff.html)

(See notice at the end of this document regarding copyright.)

这个网站是为那些对R一无所知，甚至对编程一无所知的人而设的，他们寻求*快速、无痛!*踏入R世界。

* **快速**:  你将在你的第一堂课中就开始做一些有用的R数据分析。

* **面向非程序员**: 如果你熟悉浏览网页和查看图表，那就没问题了。这个教程是为你而设计的，而不是针对有经验的C或Python编程者。

* **激发兴趣**: 每一课都围绕着一个要解决的*真实问题*，基于*真实数据*。这些课程不是由一些与现实世界无关的玩具示例组成的。材料以一种对话式、叙事的方式呈现。

* **只是基础知识，没有花哨或争论**:

    - 值得注意的是，在最初的几堂课中，我们不使用集成开发环境（IDEs）。 RStudio、ESS等是很好的工具，但您不应该同时学习R和学习IDE，这会分散注意力，阻碍您尽快在R中变得高效的目标。请注意，即使是由[R-Ladies Sydney](https://threadreaderapp.com/thread/1119025557830684673.html)提供的优秀课程，也在使用RStudio，但对RStudio的评价是**"过于庞大。"**因此，在最初的几堂课中，我们坚持使用R命令行，并专注于数据分析，而不是诸如IDE之类的工具，这将作为中级主题进行讲解。 （本教程的一些读者可能已经在使用RStudio或外部编辑器，这里的处理将在需要时为他们提供特别的说明。）

    - 覆盖范围主要限于基本的R。例如，自诩为“有主张”的Tidyverse并没有得到处理，部分原因是因为它具有争议性质（我是一个[Tidyverse怀疑者](http://github.com/matloff/TidyverseSkeptic)），但主要原因是它会阻碍你快速在R中变得高效。虽然你可以迅速学到一些简单的、"消毒过的"东西，认为你学到了很多，但这些东西的范围相当有限，Tidy学习者通常在将R应用于实际情况时会遇到困难。我们的教程是为那些目标是*在他们自己的数据分析中高效使用R系统*的学习者而设计的。




* **非被动学习方法:** 纯粹观看屏幕是无法学到东西的。编码不是一种"旁观者运动"；你必须以非被动的方式尝试这些概念。因此，会有偶尔出现**轮到你了**的部分，你作为学习者必须设计并尝试自己对所学内容的变体。有时教程会给你一些建议，但即使在这种情况下，你也应该想出自己的变体来尝试。 <span style="color:red">记住：你付出什么，就会得到什么！</span> 你在**轮到你了**部分积极参与的越多，你作为R编码者的能力就会越强大。



## 目录

**第 I 部分**
* [第 1 课：入门](#overview)
* [第 2 课：首次使用R](#firstr)
* [第 3 课：向量和索引](#vecidxs)
* [第 4 课：更多关于向量](#less2)
* [第 5 课：进入数据框！](#less3)
* [第 6 课：R因子类](#less4)
* [第 7 课：从数据框提取行/列](#extractdf)
* [第 8 课：提取行、列的更多示例](#moreextract)
* [第 9 课：tapply函数](#tapply)
* [第 10 课：数据清理](#less5)
* [第 11 课：R列表类](#less6)
* [第 12 课：对尼罗河数据的另一种看法](#less7)
* [第 13 课：暂停反思](#pause1)
* [第 14 课：基础R图形简介](#less8)
* [第 15 课：更多关于基础图形](#less9)
* [第 16 课：编写自己的函数](#less10)
* [第 17 课：`For`循环](#less11)
* [第 18 课：带块的函数](#ftnbl)
* [第 19 课：文本编辑和IDE](#edt)
* [第 20 课：If、Else、Ifelse](#ifelse)
* [第 21 课：职业运动员保持健康吗？](#keepfit)
* [第 22 课：线性回归分析，I](#linreg1)
* [第 23 课：S3类](#s3)
* [第 24 课：棒球球员分析（续）](#less15)
* [第 25 课：R包、CRAN等](#cran)

**第 II 部分**
* [第 26 课：在继续深入研究之前的暂停](#advanced)
* [第 27 课：初探ggplot2](#gg2first)
* [第 28 课：应该使用函数式编程吗？](#appfam)
* [第 29 课：简单文本处理，I](#txt)
* [第 30 课：简单文本处理，II](#txt1)
* [第 31 课：线性回归分析，II](#linreg2)
* [第 32 课：使用R日期类](#dates)
* [第 33 课：有关R编码风格和策略的技巧](#style)
* [第 34 课：逻辑模型](#logit)
* [第 35 课：文件和目录](#fd)
* [第 36 课：R `while` 循环](#whl)
* [了解更多](#forMore)
* [感谢](#thanks)
* [附录：安装和使用RStudio](#rstudio)

## <a name="overview"> </a> 第一课：入门

目前，这个在线课程的主要部分将是这个**README.md**文件。尽管它设置成一个潜在的R包，但我可能会在以后实现这一点。

文件顶部的彩色图是由我们的[**prVis包**](https://github.com/matloff/prVis/)生成的，运行在一个名为*Swiss Roll*的著名数据集上。

### <a name="noteasy"> </a> 
> 📘 请再次注意，并始终记住：  
> 
> * 非被动学习绝对关键！所以，即使在这里显示了一个R命令的输出，也请在你的R控制台中自己运行该命令，通过从本文档复制粘贴到R控制台。再次强调，*你将从这个教程中得到什么，取决于你投入了什么。*
> 
> * 同样，**轮到你了**部分是非常关键的。设计你自己的小例子，然后尝试它们！"当有疑问时，试一试！"是我为教学设计的座右铭。如果你对某些事情感到不清楚或好奇，试一试！只需设计一个小实验，然后输入代码。别担心——你不会"弄坏"东西的。
> 
> * 我不能*教*你如何编程。我只能给你工具，比如R向量，以及一些例子。因此，对于给定的期望的编程任务，你必须创造性地将这些工具组合起来以达到目标。把它当作一个拼图！我认为你会发现，如果你坚持下去，你会发现自己在这方面相当擅长。毕竟，我们都能解决难题。
> 
> * 出于这样的原因，人们必须记住*并不总是有一种简单的方式来编写给定的任务*。随着你在这些课程中的进展，它们会变得越来越复杂。成为一个好的程序员的本质是耐心和坚持。然后你就能完成那些复杂的任务！


### 开始：

您需要[安装R](https://www.datacamp.com/community/tutorials/installing-R-windows-mac-ubuntu)，可以从[R项目站点](https://www.r-project.org)下载。启动R，可以通过点击图标或在终端窗口中键入 `R` 来进行。在这里我们不要求使用RStudio，但如果你已经有了，启动它；你将在R控制台中键入，也就是Console窗格。

正如上面提到的，这个教程将是"基础知识"。特别地，没有脚本来为您键入命令。相反，您将要么从这里的文本复制粘贴到R控制台中，要么手动在那里输入。 （请注意，这里的代码行都将以R交互提示符 `>` 开始；不应该输入它。）

这是一个Markdown文件。您可以在GitHub上直接阅读它，它有自己的Markdown渲染器。或者您可以在Chrome中将其下载到自己的计算机上，并使用Markdown Reader扩展查看它（请确保启用“允许访问文件URL”）。

当您结束R会话时，通过键入 `quit()` 退出。

祝你好运！如果有任何问题，请随时给我发送电子邮件，我的邮箱是matloff@cs.ucdavis.edu

## <a name="firstr"> </a> 第二课：R的第一步

R命令提示符是 `>`。同样，它将在这里显示，但您不需要键入它。它只是在您的R窗口中，让您知道R正在邀请您提交一个命令。（如果您使用的是RStudio，您将在Console窗格中看到它。）

所以，只需输入 `1+1` 然后按Enter。确实，它输出了2（你可能期望的是12108吗？）：

```r
> 1 + 1
[1] 2
```

但这里的 `[1]` 是什么呢？这只是一个行标签。我们稍后会讨论这个，目前还不需要。

### 示例：尼罗河数据

R包含许多内置数据集，主要用于说明目的。其中之一是**Nile**，涉及尼罗河100年的年度流量数据。

让我们找到平均流量：

```r
> mean(Nile)
[1] 919.35
```

这里的**mean**是R的*函数*的一个示例，而在这种情况下，Nile是该函数的一个*参数*，这是一个说法，表示"输入"。输出的919.35被称为*返回值*或简称*值*。运行函数的行为被称为*调用*函数。 （记住这些术语！）

另一个需要注意的地方是，我们不需要调用R的**print**函数；平均流量会自动打印出来。我们将很快看到这样做的原因，但我们也可以键入：

```r
> print(mean(Nile))
```

R（和其他语言中的）中的函数调用是"从内而外"的。在这里，我们要求R找到尼罗数据的平均值（我们的内部调用），然后打印结果（对**print**函数的外部调用）。

但是，无论何时我们在R的 `>` 提示符处，我们键入的任何表达式都会被打印出来，因此不需要调用**print**。

由于这里只有100个数据点，打印它们出来并不难。同样，我们只需键入`Nile`，无需调用**print**：



``` r
> Nile
Time Series:
Start = 1871 
End = 1970 
Frequency = 1 
  [1] 1120 1160  963 1210 1160 1160  813 1230 1370 1140  995  935 1110  994 1020
 [16]  960 1180  799  958 1140 1100 1210 1150 1250 1260 1220 1030 1100  774  840
 [31]  874  694  940  833  701  916  692 1020 1050  969  831  726  456  824  702
 [46] 1120 1100  832  764  821  768  845  864  862  698  845  744  796 1040  759
 [61]  781  865  845  944  984  897  822 1010  771  676  649  846  812  742  801
 [76] 1040  860  874  848  890  744  749  838 1050  918  986  797  923  975  815
 [91] 1020  906  901 1170  912  746  919  718  714  740
```

现在你可以看到行标签是如何工作的。每行有15个数字，所以第二行从第16个开始，用`[16]`表示。第三行从第31个输出数字开始，因此有`[31]`等等。因此，如果我们想找到，比如说，第78个值，我们看一下标记为[76]的第三行中的第三个数字，得到874。

请注意，像**Nile**这样的一组数字被称为*向量*。这个是一种特殊类型的向量，即*时间序列*，向量的每个元素记录了时间上的特定点，在这里由1871年到1970年的年份组成。因此，我们知道这个向量的长度是100个元素。但是一般来说，我们可以通过调用**length**函数来找到任何向量的长度，例如：

```r
> length(Nile)
[1] 100
```

 
如果您对函数的参数不确定，R提供了**args**函数。例如，我们稍后将使用**sort**函数，该函数将一组数字从最低到最高（或反之亦然）进行排序。

例如：

``` r
> sort(Nile)
  [1]  456  649  676  692  694  698  701  702  714  718  726  740  742  744  744
 [16]  746  749  759  764  768  771  774  781  796  797  799  801  812  813  815
 [31]  821  822  824  831  832  833  838  840  845  845  845  846  848  860  862
 [46]  864  865  874  874  890  897  901  906  912  916  918  919  923  935  940
 [61]  944  958  960  963  969  975  984  986  994  995 1010 1020 1020 1020 1030
 [76] 1040 1040 1050 1050 1100 1100 1100 1110 1120 1120 1140 1140 1150 1160 1160
 [91] 1160 1170 1180 1210 1210 1220 1230 1250 1260 1370
```

(Again, the return value from the call to **sort** was printed out
automatically.)

We can query **sort**'s arguments:

``` r
> args(sort)
function (x, decreasing = FALSE, ...) 
NULL
```

我们看到**sort**函数有名为**x**和**decreasing**的参数（实际上还有更多，但暂时放在一边）。

### 第一个图形

R具有出色的图形功能，不仅在基础R中，还在一些出色的用户贡献的包中，如**ggplot2**和**lattice**。但是我们现在将使用基础R图形，将更强大但更复杂的**ggplot2**留到以后的课程。

我们将从一个非常简单、没有花哨的直方图开始：

```r
> hist(Nile)
```

像任何函数一样，**hist**有一个返回值，但在这种情况下，它被设计成在打印时产生一个图形。

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/Nile.png)

> ❄️  轮到你了
>
> 一组数字的*中值*是一个值x，使得一半的数字小于x，另一半大于x（有一些关于相同值的问题，但在这里不重要）。中值可能小于均值，也可能大于均值。确定**Nile**数据的中值属于这两种情况中的哪一种；R中的中值函数当然被命名为**median**。
>
> **hist**函数在直方图中默认为这个数据集绘制了10个柱，但您可以通过为函数指定一个可选的第二个参数**breaks**来选择其他值。例如：
> ```r
> > hist(Nile,breaks=20)
> ```
> 
> 将使用20个柱绘制直方图。尝试使用多个不同的大和小值绘制柱的数量。

**注意：**像**hist**函数这样的函数，就像许多R函数一样，有许多不同的选项，可以通过各种参数指定。现在，我们将保持简单，抵制探索它们的诱惑，但R有很多在线帮助，您可以通过 `?` 访问。例如，键入

```r
> ?hist
```

将告诉您有关**hist**函数的所有选项的完整信息。再次强调，现在对于您来说有太多了（大多数用户从未发现有必要使用更奇特的选项），但这是一个非常重要的资源，值得知道。

> 📘 专业提示
>
> 许多人喜欢通过添加括号来指定函数。例如，他们会写类似于“**length**函数经常很方便”的东西，而不是写“**length()**函数经常很方便”，以确保其他人知道他们正在谈论一个函数。我有时也这样做，但在某些情况下可能会导致麻烦。考虑以下例子：
>
> ```r
> > args(sort)
> function (x, decreasing = FALSE, ...) 
> NULL
> > args(sort())
> Error in sort.default() : argument "x" is missing, with no default
> ```
>
> 出了什么问题？在第一种情况下，我们询问**args**关于一个类型为'function'的对象**sort**的信息。在第二种情况下，我们实际上*调用了* **sort**。而后者函数本身期望一个参数，我们没有提供。 （而且也不合适。）
>
> 这里的问题相当明显，但它可能更微妙地发生。
> 
> 这说明了在编码中，我们必须非常小心地识别微妙的差异，在这种情况下是*函数*和对该函数的*调用*之间的差异。在普通英语中，我们可能会说，“那辆车想左转”而不是“那辆车的*司机*想左转”，但在编码中，我们必须非常挑剔。

> ❄️  轮到你了
>
> 编写代码将**Nile**数据从最大值到最小值进行排序，而不是相反。


## 第三课：向量与索引

假设我们想要找到1950年后的河流平均流量。

上述输出表明**尼罗河**系列始于1871年。这意味着1951年将是第81年，而第100年将是1970年。我们如何指定数据中的第81到100个元素？

可以使用*下标*或*索引*（单数为*索引*）来访问单个元素，使用方括号指定，例如

``` r
> Nile[2]
[1] 1160
```

对于第二个元素（我们之前看到的输出确实显示第二个元素为1160）。这里的值2是索引。

**c**（"连接"）函数构建一个向量，将几个数字串在一起。例如，我们可以获取**尼罗河**的第2、第5和第6个元素：

``` r
> Nile[c(2,5,6)]
[1] 1160 1160 1160
```

如果我们希望构建一个包含*连续*数字的向量，可以使用“冒号”表示法：

``` r
> Nile[c(2,3,4)]
[1] 1160  963 1210
> Nile[2:4]
[1] 1160  963 1210
```

正如你看到的，2:4是指定向量c(2,3,4)的简洁方式。

因此，81:100表示从81到100的所有数字。因此**Nile[81:100]**指定了**Nile**向量中的第81到100个元素。

然后，为了回答关于1951-1971年平均流量的问题，我们可以执行以下操作：

``` r
> mean(Nile[81:100])
[1] 877.05
```

> **注意：**请注意上述推理过程的运作方式。我们有一个目标，即找到1950年后的平均河流流量。我们知道我们有一些可以使用的工具，即**mean**函数和R向量索引。然后，我们必须找出一种将这些工具结合在一起以实现我们目标的方法，我们成功做到了。

这就是R的一般工作方式。在浏览本教程时，您将为R的“工具箱”增加越来越多的内容。然后，对于任何给定的目标，您将在该工具箱中四处寻找，并最终找到适用于手头目标的正确工具集。有时这需要一些耐心，但您会发现，您所做的越多，您就变得越熟练。

如果我们计划在这段时间内进行更多操作，我们应该制作一个副本：

``` r
> n81100 <- Nile[81:100]
> mean(n81100)
[1] 877.05
> sd(n81100)
[1] 125.5583
```

函数**sd**找到标准偏差。

请注意，我们在这里使用了R的*赋值运算符*来将这些特定的**Nile**元素复制（“分配”）到**n81100**中。（在大多数情况下，您可以使用`=`而不是`<-`，但为什么要担心可能存在的例外情况呢？它们是深奥的，因此最好始终使用`<-`。虽然这里可以使用此操作的“键盘快捷键”，但我们现在还是坚持基础知识为好。）

还要注意，尽管我们将上述操作称为“提取”**Nile**的第81到100个元素，但我们实际上只是制作了这些元素的副本。原始向量**Nile**保持不变。

> 📘 专业提示
>
> 我们几乎可以选择任何想要的名称；“n81100”只是为了方便记住这个新向量的来源而选择的名称。（但名称不能包含空格，并且必须以字母开头。）

请注意，**n81100**现在是一个包含20个元素的向量。它的第一个元素现在是**Nile**的第81个元素：

``` r
> n81100[1]
[1] 744
> Nile[81]
[1] 744
```

请记住，尽管**Nile**和**n81100**现在具有相同的内容，它们是*独立*的向量；如果一个发生变化，另一个将不会发生变化。

> ❄️ 轮到你了
>
> 想出并尝试上面的变体，比如找到1945年至1960年的平均值。

请记住，另一个经常使用的函数是**length**，它给出向量的元素数，例如

``` r
> length(Nile)
[1] 100
```

你能猜到**length(n81100)**的值吗？在'>'提示处键入此表达式以检查您的答案。

通过键入'q()'或ctrl-d离开R。 （回答否，不保存工作区。）

### 小结：在这前两课中我们学到了什么？

* 启动和退出R。

* 一些R函数：**mean**，**hist**，**length**。

* R向量和向量索引。

* 提取向量子集。

* 使用**c**和“:”函数形成向量。

对于第一课来说，这还不错！毫无疑问，您将在随后的课程和您对R的使用中频繁使用所有这些。

## 第四课：更多关于向量

沿着尼罗河继续，假设我们想知道有多少年的水位超过了120

0。让我们首先介绍R的**sum**函数：

``` r
> sum(c(5,12,13))
[1] 30
```

这里***c***函数构建了一个包含5、12和13的向量。然后，该向量被输入到**sum**函数中，返回5+12+13=30。

顺便说一下，上面是我们第一个*函数组合*的示例，其中一个函数的输出（在这里是***c***）被作为输入馈送到另一个函数中（在这种情况下是**sum**）。

现在我们可以使用这个来回答我们关于**Nile**数据的问题：

``` r
> sum(Nile > 1200)
[1] 7
```

河流水位在7年内超过了1200。

**但是这是如何运作的呢？**请耐心等待片刻。让我们首先看一个小例子：

``` r
> x <- c(5,12,13)
> x
[1]  5 12 13
> x > 8
[1] FALSE  TRUE  TRUE
> sum(x > 8)
[1] 2
```

首先，请注意这里的表达式**x > 8**中的一些奇怪之处。这里**x**是一个向量，长度为3，但8只是一个数字。询问一个向量是否大于一个数字似乎是没有意义的；它们是不同的动物。

但是R通过将该数字8扩展为一个3元素向量8,8,8，将它们变成“相同类型”的动物。这称为*循环*。这设置了逐个元素的比较：然后，**x**中的5与第一个8进行比较，产生FALSE，即5不大于8。然后，12与第二个8进行比较，产生TRUE，然后13与第三个8进行比较产生另一个TRUE。因此，我们得到了向量FALSE,TRUE,TRUE。

好了，但是**sum**如何将一些TRUE和FALSE相加呢？答案是R，像大多数计算机语言一样，将TRUE和FALSE视为1和0，分别处理。因此，我们对向量（0,1,1）求和，得到2。

回到关于尼罗河流量超过1200年数的问题，让我们再次看看那个表达式：

``` r
> sum(Nile > 1200)
```

由于向量**Nile**的长度为100，那个数字1200将被循环成一个包含一百个1200的向量。然后'>'比较将产生100个TRUE和FALSE，因此求和会给我们TRUE的数量，正是我们想要的。

与*有多少*年流量超过1200有关的问题是哪些年具有该特性。实际上，R实际上有一个**which**函数：

``` r
> which(Nile > 1200)
[1]  4  8  9 22 24 25 26
```

因此，**Nile**中的第4、第8、第9等元素具有查询的特性。（请注意，这些是1875年，1879年等。）

实际上，这为我们提供了另一种获得具有该特性的年份计数的方法：

``` r
> which1200 <- which(Nile > 1200)
> which1200
[1]  4  8  9 22 24 25 26
> length(which1200)
[1] 7
```

当然，像往常一样，我选择的变量名“which1200”是任意的，只是帮助我记住该变量中存储了什么的东西。

R的**length**函数做了它说的事情，即找到向量的长度。在我们的情境中，这给我们提供了流量超过1200的年份计数。

那么，在这7年中，河流的流量是多少？

``` r
> which1200 <- which(Nile > 1200)
> Nile[which1200]
[1] 1210 1230 1370 1210 1250 1260 1220
```

最后，再来点复杂的。我们可以组合上面的步骤：

``` r
> Nile[Nile > 1200]
[1] 1210 1230 1370 1210 1250 1260 1220
```

我们刚刚“消除了中间人”**which1200**。R解释器看到我们的“Nile > 1200”，然后生成相应的TRUE和FALSE。然后，R解释器将这些TRUE和FALSE视为**Nile**中的下标，从而提取所需的数据。

现在，我们可能要在这里补充一句，“孩子们，别在家里尝试这个。”对于初学者来说，将事情分成步骤确实更容易、更舒适。一旦您在R上有经验，您可能希望开始跳过一些步骤。

> ❄️ 该你了
>
> 假设我们对尼罗河在水位低于950时的年份感兴趣。编写代码来确定（a）有多少这样的年份，（b）这些具体是哪些年份，以及（c）这些年份的中位数。
>
> 尝试进行您选择的其他实验，使用**sum**开始可能是个不错的选择。我建议从小向量开始实验，比如（2,1,1,6,8,5），这样您就知道自己的答案是正确的。请记住，您将通过积极参与来更好地学习。开始写代码吧！


非常有用的是负索引的概念，例如：

```r
> x <- c(5,12,13,8)
> x[-1]  
[1] 12 13  8
```

在这里，我们要求获取所有**x**，*除了* **x[1]**。你能猜到**x[c(-1,-4)]**的结果吗？先猜一下，然后试一试。

### 小结：在这节课中我们学到了什么？

在这里，你已经完善了你在R向量上的技能，学到了R的循环利用特性以及R用户用于查找数量的两个技巧。

当你在本教程中继续学习时，你会发现这些东西在R中经常被使用。

## <a name="less3"> </a> 第5课：进入数据框！

在向量之后，R的下一个主要工具是*数据框*。它是一个由每个数据点一行组成的矩形表格。

假设我们有100个人的身高、体重和年龄。我们的数据框将有100行和3列。例如，在第二行和第三列中的条目将是我们数据中第二个人的年龄。整个第二行将是该第二个人的所有数据，即该人的身高、体重和年龄。

**注意该行也被视为一个向量。第三列整体将是我们数据集中所有年龄的向量。**

作为我们第一个例子，考虑R内置的**ToothGrowth**数据集。同样，你可以通过键入以下命令来阅读它：

```r
> ?ToothGrowth
```

数据实际上是关于豚鼠的，使用橙汁或维生素C作为生长补充剂。让我们从命令行快速查看。

```r
> head(ToothGrowth)
   len supp dose
1  4.2   VC  0.5
2 11.5   VC  0.5
3  7.3   VC  0.5
4  5.8   VC  0.5
5  6.4   VC  0.5
6 10.0   VC  0.5
```

R的**head**函数（默认情况下）显示给定数据框的前6行。我们看到有长度、补充剂和剂量列，数据的管理员决定将它们命名为'len'、'supp'和'dose'。每一列都是一个R向量，或者在第二列的情况下，是一个称为*factor*的类似向量的对象，稍后将讨论）。  

> 📘 专业提示
>
> 为了避免反复写出长单词，使用较短的名称制作副本是很方便的。

```r
> tg <- ToothGrowth
```

美元符号用于表示各个列，例如**ToothGrowth$dose**表示剂量列。因此，例如，我们可以打印出牙齿长度的平均值：

```r
> mean(tg$len)
[1] 18.81333
```

数据框中的下标/索引是一对，指定行和列号。要获取第3行第1列的元素：

```r
> tg[3,1]
[1] 7.3
```
这与我们在**head**示例中看到的相符。或者，使用**tg$len**是一个向量的事实：

```r
> tg$len[3]
[1] 7.3
```

在*数据框* **tg** 中的第3行第1列的元素对应于 *向量* **tg$len** 中的第3个元素。R经常在数据框和向量之间的这种二元性上进行操作。

> ❄️  你的回合
>
> 上面的例子对于R来说是基础的，因此这次你应该自己进行一些小实验，稍微变换一下上面的例子。你做得越多，就越好！

对于数据框**d**的任何子集，我们都可以使用以下格式提取我们想要的行和列：

```r
d[我们想要的行，我们想要的列]
```

有些数据框没有列名，但这不是问题。我们可以使用列号，例如：

```r
> mean(tg[,1])
[1] 18.81333
```

注意表达式'[,1]'。由于第二个位置上有个1，我们正在谈论第1列。由于逗号前的第一个位置是空的，没有指定行，因此*所有*行都包括在内。这归结为：所有的第1列。

R的一个关键特性是可以提取数据框的子集，就像我们之前提取向量的子集一样。例如，

```r
> z <- tg[2:5,c(1,3)]
> z
   len dose
2 11.5  0.5
3  7.3  0.5
4  5.8  0.5
5  6.4  0.5
```

在这里，我们提取了第2到第5行和第1到第3列，将结果赋给了**z**。要提取这些列但保留所有行，可以执行：

```r
> y <- tg[ ,c(1,3)]
```

即留下行规范字段为空。

顺便说一下，注意这三列的长度都是相同的，这是数据框的要求。在这种情况下，这个共同的长度是多少？R的**nrow**函数告诉我们任何数据框中的行数：

```r
> nrow(ToothGrowth)
[1] 60
```

啊，60行（60只

豚鼠，每只测量3次）。

或者，也可以这样：

```r
> tg <- ToothGrowth
> length(tg$len)
[1] 60
> length(tg$supp)
[1] 60
> length(tg$dose)
[1] 60
```

所以现在你知道四种做同样事情的方法。但一个不够吗？当然。但在这个熟悉阶段，阅读所有四种方法将有助于强化你现在对R知识的累积。所以，请确保你理解这四种方法是如何产生数字60的。

**head**函数也适用于向量：

```r
>  head(ToothGrowth$len)
[1]  4.2 11.5  7.3  5.8  6.4 10.0
```

像许多R函数一样，**head**有一个可选的第二个参数，指定要打印多少元素：

```r
> head(ToothGrowth$len,10)
 [1]  4.2 11.5  7.3  5.8  6.4 10.0 11.2 11.2  5.2  7.0
```

你可以创建自己的数据框——这对于测试你的理解非常有用——方法如下：

```r
> x <- c(5,12,13)
> y <- c('abc','de','z')
> d <- data.frame(x,y)
> d
   x   y
1  5 abc
2 12  de
3 13   z
```

看看第二行！可以形成由字符字符串组成的向量，具有完整的索引功能，例如

```r
> y <- c('abc','de','z')
> y[2]
[1] "de"
```

正如前面提到的，数据框中的所有列必须具有相同的长度。在这里**x**由3个数字组成，而**y**由3个字符字符串组成。（后者的单位是字符串。每个字符串中的字符数是无关紧要的。）

对于行和列，也可以使用负索引，例如

```r
> z <- tg[,-2]
> head(z)
   len dose
1  4.2  0.5
2 11.5  0.5
3  7.3  0.5
4  5.8  0.5
5  6.4  0.5
6 10.0  0.5
```

> ❄️  你的回合
>
> 想出一些关于**ToothGrowth**数据的小例子。例如，编写代码查找牙齿长度小于16的情况数量，以及VC补充剂所在的行是哪些。 
>
> 此外，尝试使用另一个内置的R数据集**faithful**进行一些示例。这个数据集涉及美国黄石国家公园的老忠实间歇泉。第一列给出了喷发的持续时间，第二列是距上次喷发的等待时间。正如前面提到的，这些操作是R的关键特性，因此尽可能设计并运行尽可能多的示例；最好是偏向做得多一些！

### 小结：在这节课中我们学到了什么？

如前所述，数据框是R的基本工具。它由向量（长度相等）的列组成，这一事实经常很方便。

与向量的单一数字索引不同，数据框中的每个元素都有两个索引，一个是行号，一个是列号。我们可以指定要提取的行和列的集合以提取子框。

可以使用R的**nrow**函数查询数据框中的行数；**ncol**对于列数也是如此。

## <a name="less4"> </a> 第 6 课：R因子类

在R中，每个对象都有一个*类*。数字3的类是**'numeric'**，字符字符串'abc'的类是**'character'**等等。 （在R中，类名需要引号；可以使用单引号或双引号。）请注意，数字向量也是**'numeric'**类；实际上，单个数字被认为是长度为1的向量。因此，例如**c('abc','xw')**也是**'character'**。

> 📘 专业提示
>
> 计算机要求人非常小心，非常精确。在上面的**c('abc','xw')**表达式中，人们可能会想知道为什么它没有评估为'abcxw'。毕竟，我不是说过'c'代表"连接"吗？是的，但是**c**函数连接*向量*。这里'abc'是长度为1的向量——我们有*一个*字符字符串，它由3个字符组成是无关紧要的——同样，'xw'也是一个字符字符串。因此，我们正在连接一个包含1个元素的向量与另一个包含1个元素的向量，结果是一个包含2个元素的向量。

那么在上面的维生素C的例子中**tg**和**tg$supp**的类是什么？

```r
> class(tg)
[1] "data.frame"
> class(tg$supp)
[1] "factor"
```

当我们有*分类*变量时，R因子就会派上用场。例如，在一项基因研究中，我们可能有一个关于头发颜色的变量，它可能包括四个类别：黑色、棕色、红色、金色。我们可以通过以下方式找到**tg$supp**的类别列表：

```r
> levels(tg$supp)
[1] "OJ" "VC"
```

这里的分类变量是**supp**，这是数据集创建者为补充列选择的名称。我们看到有两个类别（*levels*），即橙汁或维生素C。

请注意，R因子的值必须用引号括起来。可以使用单引号或双引号都可以（尽管在使用**head**时不显示引号）。

> 📘 专业提示
>
> R的**factor**类是R中最强大的方面之一。在接下来的课程中，我们将逐渐掌握这项技能。确保真正熟练掌握它。

> ❄️  你的回合
>
> 如前所述，R包含许多内置数据集，可以通过调用**data()**获取列表。浏览其中一些数据集，并找到一个你认为将包含一个因子列的数据集；然后进行验证。

## <a name="extractdf"> </a> 第 7 课：从数据框中提取行/列

（读者应该特别慢慢而仔细地阅读这一课程。概念很简单，但将它们组合起来需要仔细检查。）

首先，让我们回顾一下前面一课中看到的内容：

```r
> which1200 <- which(Nile > 1200)
> Nile[which1200]
[1] 1210 1230 1370 1210 1250 1260 1220
```

在这里，我们学习了如何提取*向量元素*。我们可以类似地提取*数据框的行或列*。以下是方法：

继续使用维生素C的例子，让我们比较两种补充剂类型的平均牙齿长度。以下是代码：

```r
> whichOJ <- which(tg$supp == 'OJ')
> whichVC <- which(tg$supp == 'VC')
> mean(tg[whichOJ,1])
[1] 20.66333
> mean(tg[whichVC,1])
[1] 16.96333
```

在上述的前两行中，我们找到了**tg**（或等效地，**tg$supp**）中具有OJ补充剂的行，将这些行号记录在**whichOJ**中。然后我们对VC做了同样的事情。

现在，看一下表达式**tg[whichOJ,1]**。记住，数据框是用两个下标表达式访问的，一个是用于行，一个是用于列，格式如下：

```r
d[the rows we want, the columns we want]
```

因此，**tg[whichOJ,1]** 表示只关注OJ行，而且只有第1列，即牙齿长度。然后我们找到这些受限制的数字的平均值。结果是20.66333。然后对VC进行同样的操作。

同样，如果我们经验丰富，我们可以跳过一些步骤：

```r
> tgoj <- tg[tg$supp == 'OJ',]
> tgvc <- tg[tg$supp == 'VC',]
> mean(tgoj$len)
[1] 20.66333
> mean(tgvc$len)
[1] 16.96333
```

无论哪种方式，我们都得到了我们最初问题的答案：橙汁似乎比维生素C产生更多的生长。 （当然，可以为差异等形成置信区间。）

### 小结：在这节课中我们学到了什么？

正如我们之前学习如何使用TRUE和FALSE值序列提取向量的部分一样，我们现在看到了如何对数据框进行类似的操作：**我们可以使用TRUE和FALSE值序列从数据框

中提取某些行或列。**

在继续之前，读者必须充分理解这一课程，在自己进行一些上述示例的变化之前。我们将在本教程中经常使用这项技术，它对于在实际世界中使用R是至关重要的。

> ❄️  你的回合
>
> 尝试在R的内置**faithful**数据集上进行一些操作。例如，找出等待时间超过80分钟的喷发次数。


## <a name="moreextract"> </a> 第 8 课：更多提取行和列的例子

通常，我们需要根据多个条件提取数据框的行或列。例如，假设我们希望从**tg**中提取由OJ和长度小于8.8组成的子数据框。

我们可以使用与符号'&'，它表示逻辑AND操作：

```r
> tg[tg$supp=='OJ' & tg$len < 8.8,]
   len supp dose
37 8.2   OJ  0.5
```

啊，结果表明只有一个案例同时满足两个条件。

如果我们想要满足至少一个条件的所有行，而不一定是两者，那么我们使用OR运算符'|'。例如，我们想要获取所有长度大于28或治疗剂剂量为1.0或两者的行：

```r
> tg[tg$len > 28 | tg$dose == 1.0,]
    len supp dose
11 16.5   VC    1
12 16.5   VC    1
13 15.2   VC    1
14 17.3   VC    1
15 22.5   VC    1
16 17.3   VC    1
17 13.6   VC    1
18 14.5   VC    1
19 18.8   VC    1
20 15.5   VC    1
23 33.9   VC    2
26 32.5   VC    2
30 29.5   VC    2
41 19.7   OJ    1
42 23.3   OJ    1
43 23.6   OJ    1
44 26.4   OJ    1
45 20.0   OJ    1
46 25.2   OJ    1
47 25.8   OJ    1
48 21.2   OJ    1
49 14.5   OJ    1
50 27.3   OJ    1
56 30.9   OJ    2
59 29.4   OJ    2
```

顺便说一下，原始的行号也被显示了。例如，满足条件的第一个案例在原始数据框**tg**中是第11行。

通常，我们不仅想提取数据框的一部分，还想保存结果：

```r
> w <- tg[tg$len > 28 | tg$dose == 1.0,]
```

再次强调，我随意选择了名字'w'。名称必须以字母开头，并且只能由字母，数字和一些特殊字符（例如'-'或'_'）组成。

请注意，**w**是一个新的数据框，我们可以对其执行通常的操作，例如

```r
> head(w)
    len supp dose
11 16.5   VC    1
12 16.5   VC    1
13 15.2   VC    1
14 17.3   VC    1
15 22.5   VC    1
16 17.3   VC    1
> nrow(w)
[1] 25
```

我们可能只对例如满足给定条件的*数量*感兴趣。与之前一样，我们可以使用**nrow**来实现，如下所示。

正如前面所看到的，我们还可以提取列。例如，我们的分析将仅使用牙齿长度和剂量。我们在“要提取的列是什么”位置写入'c(1,3)'，表示列1和3：

```r
> lendose <- tg[,c(1,3)]
> head(lendose)
   len dose
1  4.2  0.5
2 11.5  0.5
3  7.3  0.5
4  5.8  0.5
5  6.4  0.5
6 10.0  0.5
```

从现在开始，我们将使用**lendose**而不是**tg**。

不过，使用列名而不是数字指定列会更好一些：

```r
> lendose <- tg[,c('len','dose')]
> head(lendose)
   len dose
1  4.2  0.5
2 11.5  0.5
3  7.3  0.5
4  5.8  0.5
5  6.4  0.5
6 10.0  0.5
```

逻辑操作也适用于向量。例如，在**Nile**数据中，假设我们想知道有多少年的流量在极端值以下，例如低于800或高于1300：

```r
> exts <- Nile[Nile < 800 | Nile > 1300]
> head(exts)
[1] 1370  799  774  694  701  692
> length(exts)
[1] 27
```

顺便说一下，如果这个计数是我们唯一关心的，即我们对**exts**没有进一步的用途，我们可以跳过对**exts**的分配，直接进行操作：

```r
> length(Nile[Nile < 800 | Nile > 1300])
[1] 27
```

这对于经验丰富的R用户来说是可以的

，但实际上，“一步一步”对于初学者来说更好。它更清晰，最重要的是，如果发生错误，调试起来更容易。

### 小结：在本课中我们学到了什么？

在这里，我们有更多的练习操作数据框，并介绍了逻辑运算符'&'和'|'的另一个示例。我们还看到了使用**nrow**作为计算满足给定条件的行数的一种方法的另一个示例。

这些都是实际世界中R使用中经常遇到的“基本”操作。

顺便说一下，要注意R的本质是“将小事物组合起来以完成大事物”，例如将子集操作、'&'运算符和**nrow**结合起来以获取满足给定条件的行数。这也是R的“基本”之一。由你作为R用户创造性地组合R的小操作（以后还有一些大操作）以实现你对数据的任何目标的能力。*编程是一个创造性的过程*。就像杂货店和烹饪一样：商店有很多不同的潜在配料，你决定购买哪些并将它们组合成一顿饭。

> ❄️ 你的回合

> 尝试在 R 内置的 "faithful" 数据集上执行一些操作。例如，查找其中喷发时间大于 3 分钟且等待时间超过 80 分钟的行数。同时，编写代码打印出这些满足条件的行的行号。

# 第9课：`tapply` 函数

**专业提示：**
在R中，通常有一种更短、更紧凑的做法。这在这里也是适用的；我们可以在上面的例子中使用神奇的 **tapply** 函数。实际上，我们可以在一行中完成。

调用 **tapply** 的一般形式为：

``` r
tapply(要拆分的内容, 用于拆分的标准, 对结果进行分组的操作)
```

``` r
> tapply(tg$len, tg$supp, mean)
      OJ       VC 
20.66333 16.96333 
```

简单来说：“根据 **tg$supp** 的值，将向量 **tg$len** 分为两组，然后对每组应用 **mean**。” 请注意，结果被返回为一个向量，我们可以通过将其赋值给比如 **z** 来保存：

``` r
> z <- tapply(tg$len, tg$supp, mean)
> z[1]
      OJ 
20.66333 
> z[2]
      VC 
16.96333 
```

顺便说一下，**z** 不仅是一个向量，还是一个具有名称的向量，这意味着它的元素有名称，此处为'OJ'和'VC'。

保存对于后续的代码很有用。

为了确保这是如何工作的，让我们看一个小的人造示例：

``` r
> x <- c(8, 5, 12, 13)
> g <- c('M', "F", 'M', 'M')
```

假设 **x** 是一些儿童的年龄，一个男孩，一个女孩，然后是两个男孩，如 **g** 中所示。例如，5岁的是一个女孩。

让我们调用 **tapply**：

``` r
> tapply(x, g, mean)
 F  M 
 5 11 
``` 

这个调用表示：“根据 **g** 中相应元素的值，将 **x** 分成两组，然后在每组中找到平均值。

请注意，**x** 和 **g** 上面的元素数量相同，各为4。相反，如果 **g** 有5个元素，那么第五个元素将是无用的——在 **x** 中不存在的第五个孩子的年龄的性别。类似地，如果 **g** 只有3个元素，似乎第四个孩子没有指定性别也是不对的。

**专业提示：**
如果 **g** 的长度不对，我们会得到一个错误，"Arguments must be of the same length." 这是R代码中的常见错误，因此要注意它，要知道为什么长度必须相同。

除了 **mean**，我们可以在 **tapply** 中的第三个参数使用任何函数。这里是另一个示例，使用内置数据集 **PlantGrowth**：

``` r
> tapply(PlantGrowth$weight, PlantGrowth$group, length)
ctrl trt1 trt2 
  10   10   10 
```

这里，**tapply** 将 **weight** 向量根据 **group** 变量拆分为子集，然后在每个子集上调用 **length** 函数。我们看到每个子集的长度都为10，即实验为对照组分配了10个植物，对待疗法1分配了10个植物，对待疗法2分配了10个植物。

> ❄️  你的机会
>
> R中最著名的内置数据集之一是 **mtcars**，其中包含60年代和70年代汽车的各种测量数据。在这里，你有很多机会来尝试一些小实验！
>
> 你可能希望从比较4缸、6缸和8缸汽车的平均每加仑英里数开始。另一个建议是使用 **table** 找出每个气缸类别中有多少辆汽车。像往常一样，你在这里尝试的示例越多，越好！

顺便说一下，**mtcars** 数据框有一列是“幻影”列。

``` r
> head(mtcars)
                   mpg cyl disp  hp drat    wt  qsec vs am gear carb
Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

这第一列似乎给出了汽车的制造商和型号。是的，它确实是——但它不是一列。瞧：

``` r
> head(mtcars[,1])
[1] 21.0 21.0 22.8 21.4 18.7 18.1
```

确实，第一列是mpg数据，而不是汽车名称。但我们在最左边看到了名称！这个看似矛盾的解决之道是，这些汽车名称是此数据框的 *行名称*：

``` r
> row.names(mtcars)
 [1] "Mazda RX4"           "Mazda RX4 Wag"       "Datsun 710"         
 [4] "Hornet 4 Drive"      "Hornet Sportabout"   "Valiant"            
 [7] "Duster 360"          "Merc 240D"           "Merc 230"           
[10] "Merc 280"            "Merc 280C"           "Merc 450SE"         
[13] "Merc 450SL"          "Merc 450SLC"         "Cadillac Fleetwood" 
[16] "Lincoln Continental" "Chrysler Imperial"   "Fiat 128"           
[19] "Honda Civic"         "Toyota Corolla"      "Toyota Corona"      
[22] "Dodge Challenger"    "AMC Javelin"         "Camaro Z28"         
[25] "Pontiac Firebird"    "Fiat X1-9"           "Porsche 914-2"      
[28] "Lotus Europa"        "Ford Pantera L"      "Ferrari Dino"       
[31] "Maserati Bora"       "Volvo 142E"         
```

因此，'Mazda RX4'是第1行的 *名称*，但不是行的一部分。

与其他一切一样，**row.names** 是一个函数，正如你在上面看到的那样，它在这里的返回值是一个32元素的向量（数据框有32行，因此有32个行名称）。该向量的元素是 **'character'** 类型的，就像向量本身一样。

你甚至可以对该向量进行赋值：

``` r
> row.names(mtcars)[7]
[1] "Duster 360"
> row.names(mtcars)[7] <- 'Dustpan'
> row.names(mtcars)[7]
[1] "Dustpan"
```

顺便说一下，这是一个内部玩笑。是的，这个例子是真实而重要的，但 "Dustpan" 的梗来源于当时一则有趣的电视广告。

（如果你在编程方面有一些背景，可能会觉得在赋值的左侧使用函数调用有些奇怪。这实际上在R中很常见。这源自于 '<-' 实际上是一个函数！但这不是深入讨论的地方。）

**专业提示：**
> 作为一个初学者（实际上是在以后的学习中），你不应该过于追求总是以 "最佳" 方式编写代码，包括代码的紧凑性。更重要的是，写出可行且清晰的代码；可以随时稍作调整。在这种情况下，**tapply** 实际上有助于提高清晰度，并且它非常普遍有用，因此我们在本教程的早期引入了它。我们将在以后的课程中更多地使用它。


## <a name="less5"> </a> Lesson 10:  Data Cleaning

Most real-world data is "dirty," i.e. filled with errors.  The famous
[New York taxi trip
dataset](https://data.cityofnewyork.us/Transportation/2017-Yellow-Taxi-Trip-Data/biws-g3hs),
for instance, has one trip destination whose lattitude and longitude
place it in Antartica! The impact of such erroneous data on one's statistical
analysis can be anywhere from mild to disabling.  Let's see below how one
might ferret out bad data.  And along the way, we'll cover several new R
concepts.

We'll use the famous Pima Diabetes dataset.  Various versions exist, but
we'll use the one included in **faraway**, an R package compiled
by Julian Faraway, author of several popular books on statistical
regression analysis in R.

I've placed the data file, **Pima.csv**, on
[my Web site](http://heather.cs.ucdavis.edu/FasteR/data/Pima.csv). Here
is how you can read it into R:

``` r
> pima <- read.csv('http://heather.cs.ucdavis.edu/FasteR/data/Pima.csv',header=TRUE)
```

The dataset is in a CSV ("comma-separated values") file.  Here we read
it, and assigned the resulting data frame to a variable we chose to name
**pima**.

Note that second argument, **header=TRUE**.  A header in a file, if one
exists, is in the first line in the file.  It states what names the
columns in the data frame are to have.  If the file doesn't have one,
set **header** to FALSE.  You can always add names to your data frame
later (future lesson).

> 📘 Pro Tip
>
> It's always good to take a quick look at a newly loaded or construced
> data frame:

``` r
> head(pima)
  pregnant glucose diastolic triceps insulin  bmi diabetes age test
1        6     148        72      35       0 33.6    0.627  50    1
2        1      85        66      29       0 26.6    0.351  31    0
3        8     183        64       0       0 23.3    0.672  32    1
4        1      89        66      23      94 28.1    0.167  21    0
5        0     137        40      35     168 43.1    2.288  33    1
6        5     116        74       0       0 25.6    0.201  30    0
> dim(pima)
[1] 768   9
```

The **dim** function tells us that there are
768 people in the study, 9 variables measured on each, i.e. the data has
768 rows and 9 columns.

Since this is a study of diabetes, let's take a look at the glucose
variable.  R's **table** function is quite handy.

``` r
> table(pima$glucose)

  0  44  56  57  61  62  65  67  68  71  72  73  74  75  76  77  78  79  80  81 
  5   1   1   2   1   1   1   1   3   4   1   3   4   2   2   2   4   3   6   6 
 82  83  84  85  86  87  88  89  90  91  92  93  94  95  96  97  98  99 100 101 
  3   6  10   7   3   7   9   6  11   9   9   7   7  13   8   9   3  17  17   9 
102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 
 13   9   6  13  14  11  13  12   6  14  13   5  11  10   7  11   6  11  11   6 
122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 
 12   9  11  14   9   5  11  14   7   5   5   5   6   4   8   8   5   8   5   5 
142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 
  5   6   7   5   9   7   4   1   3   6   4   2   6   5   3   2   8   2   1   3 
162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 
  6   3   3   4   3   3   4   1   2   3   1   6   2   2   2   1   1   5   5   5 
182 183 184 186 187 188 189 190 191 193 194 195 196 197 198 199 
  1   3   3   1   4   2   4   1   1   2   3   2   3   4   1   1 
```

Be careful here; the first, third, fifth and so on lines are the glucose
values, while the second, fourth, sixth and so on lines are the counts
of women having those values.  For instance, 3 women had glucose = 68.

Uh, oh!  5 women in the study had glucose level 0.  And 1 had level 44,
etc.  Presumably 0 is not physiologically possible, and maybe not 44
either.

Let's consider a version of the glucose data that at least excludes these 0s.

``` r
> pg <- pima$glucose
> pg1 <- pg[pg > 0]
> length(pg1)
[1] 763
```

As before, the expression **pg > 0** creates a vector of TRUEs and FALSEs.
The filtering **pg[pg > 0]** will only pick up the TRUE cases, and sure
enough, we see that **pg1** has only 763 cases, as opposed to the
original 768; the 5 with glucose = 0 are now gone.

Did removing the 0s make much difference?  Turns out it doesn't:

``` r
> mean(pg)
[1] 120.8945
> mean(pg1)
[1] 121.6868
```

But still, these things can in fact have  major impact in many
statistical analyses.

R has a special code for missing values, NA, for situations like this.
Rather than removing the 0s, it's better to recode them as NAs.  Let's
do this, back in the original dataset so we keep all the data in
one object:

``` r
> pima$glucose[pima$glucose == 0] <- NA
```

This is a bit complicated.  Here is the same action, but broken into
smaller steps:

``` r
> glc <- pima$glucose
> z <- glc == 0
> glc[z] <- NA
> pima$glucose <- glc
```

Here is what the code does:

- That first line just makes a copy of the original vector, to avoid
clutter in the code.  
- The second line determines which elements of **glc**
are 0s, resulting in **z** being a vector of TRUEs and FALSEs.  
- The third line then assigns NA to those elements in **glc** corresponding to
the TRUEs. (Note the recycling of NA.)
- Finally, we need to have the changes in the original data, so we copy
  **glc** to it.

> 📘 Pro Tip
>
> We broke our original 1 line of code into 4 simpler lines.
> This is MUCH clearer, and by the way, easier to debug. 
> I recommend this especially for beginners, but also for everyone, and
> I use this approach a lot in my own code.
>
> There is an advanced R concept, *pipes*, that also breaks longer
> computations into smaller steps.  I do not use pipes (either the
> Tidyverse version or the newer base-R pipes), as I believe they are
> less clear and, very important, hard to debug.  You may find you like
> them, which of course is fine, but we will not use them here.

> 📘 Pro Tip
>
> Note again the double-equal sign in the above code!  If we wish to
> test whether, say, ***a*** and ***b*** are equal, the expression must
> be "a == b", not "a = b"; the latter would do "a <- b".  This is a
> famous beginning programmer's error.

As a check, let's verify that we now have 5 NAs in the glucose variable:

``` r
> sum(is.na(pima$glucose))
[1] 5
```

Here the built-in R function **is.na** will return a vector of TRUEs and
FALSEs.  Recall that those values can always be treated as 1s and 0s,
thus summable.  Thus we got our count, 5.

Let's also check that the mean comes out right:

``` r
> mean(pima$glucose)
[1] NA
```

What went wrong?  By default, the **mean** function will *not* skip over
NA values; thus the mean was reported as NA too.  But we can instruct
the function to skip the NAs:

``` r
> mean(pima$glucose,na.rm=TRUE)
[1] 121.6868
```

> ❄️  Your Turn
>
> Determine which other columns in **pima** have
> suspicious 0s, and replace them with NA values.  
> 
> Now, look again at the plot we made earlier of the Nile flow histogram.
> There seems to be a gap between the numbers at the low end and the rest.
> What years did these correspond to?  Find the mean of the data,
> excluding these cases.

## <a name="less6"> </a> Lesson 11:  The R List Class

We saw earlier how handy the **tapply** function can be.  Let's look at
a related one, **split**.  The general call form of the latter is

``` r
split(what to split, what criterion to use for splitting) 
```

This looks similar to the form for **tapply** that we saw earlier,

``` r
tapply(what to split, what criterion to use for splitting, 
   what to do with the resulting grouped data)
```

But this is no surprise, because the internal code for **tapply**
actually calls **split**.  (You can check this via **edit(tapply)**.)


Earlier we mentioned the built-in dataset **mtcars**, a data frame.
Consider **mtcars$mpg**, the column containing the miles-per-gallon
data.  Again, to save typing and avoid clutter in our code, let's make a
copy first:

``` r
> mtmpg <- mtcars$mpg
```

Suppose we wish to split the original vector into three vectors, 
one for 4-cylinder cars, one for 6 and one for 8.  We *could* do

``` r
> mt4 <- mtmpg[mtcars$cyl == 4]
```

and so on for **mt6** and **mt8**.

> ❄️  Your Turn
>
> In order to keep up, make sure you understand how that
> line of code works, with the TRUEs and FALSEs etc.  First print out the
> value of **mtcars$cyl == 4**, and go from there.


But there is a cleaner way:

``` r
> mtl <- split(mtmpg,mtcars$cyl)
> mtl
$`4`
 [1] 22.8 24.4 22.8 32.4 30.4 33.9 21.5 27.3 26.0 30.4 21.4

$`6`
[1] 21.0 21.0 21.4 18.1 19.2 17.8 19.7

$`8`
 [1] 18.7 14.3 16.4 17.3 15.2 10.4 10.4 14.7 15.5 15.2 13.3 19.2 15.8 15.0
> class(mtl)
[1] "list"
```

In English, the call to **split** said, "Split **mtmpg** into multiple
vectors, with the splitting criterion being the correspond
values in **mtcars$cyl**."


Now **mtl**, an object of R class **"list"**, contains the 3 vectors.
We can access them individually with the dollar sign notation:

``` r
> mtl$`4`
 [1] 22.8 24.4 22.8 32.4 30.4 33.9 21.5 27.3 26.0 30.4 21.4
```

Or, we can use indices, though now with double brackets:

``` r
> mtl[[1]]
 [1] 22.8 24.4 22.8 32.4 30.4 33.9 21.5 27.3 26.0 30.4 21.4
```

Looking a little closer:

``` r
> head(mtcars$cyl)
[1] 6 6 4 6 8 6 
``` 

We see that the first car had 6 cylinders, so the
first element of **mtmpg**, 21.0, was thrown into the `6` pile, i.e.
**mtl[[2]]** (see above printout of **mtl**), and so on.

And of course we can make copies for later convenience:

``` r
> m4 <- mtl[[1]]
> m6 <- mtl[[2]]
> m8 <- mtl[[3]]
```

Lists are especially good for mixing types together in one package:

``` r
> l <- list(a = c(2,5), b = 'sky')
> l
$a
[1] 2 5

$b
[1] "sky"
```

Note that here we can give names to the list elements, 'a' and 'b'.  In
forming **mtl** using **split** above, the names were assigned
according to the values of the vector beiing split.  (In that earlier
case, we also needed backquotes ``   ``, since the names were numbers.)


If we don't like those default names, we can change them:

``` r
> names(mtl) <- c('four','six','eight')
> mtl
$four
 [1] 22.8 24.4 22.8 32.4 30.4 33.9 21.5 27.3 26.0 30.4 21.4

$six
[1] 21.0 21.0 21.4 18.1 19.2 17.8 19.7

$eight
 [1] 18.7 14.3 16.4 17.3 15.2 10.4 10.4 14.7 15.5 15.2 13.3 19.2 15.8
15.0
```

What if we want, say, the MPG for the third car in the 6-cylinder
category?

``` r
> mtl[[2]][3]
[1] 21.4
```

The point is that **mtl[[2]]** is a vector, so if we want element 3 of
that vector, we tack on [3].

Or,

``` r
> mtl$six[3]
[1] 21.4
``` 

By the way, it's no coincidence that a dollar sign is used for
delineation in both data frames and lists; data frames *are* lists.
Each column is one element of the list.  So for instance,

``` r
> mtcars[[1]]
 [1] 21.0 21.0 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 17.8 16.4 17.3 15.2 10.4
[16] 10.4 14.7 32.4 30.4 33.9 21.5 15.5 15.2 13.3 19.2 27.3 26.0 30.4 15.8 19.7
[31] 15.0 21.4
```

Here we used the double-brackets list notation to get the first element
of the list, which is the first column of the data frame.

> ❄️  Your Turn
>
> Try using **split** on the ToothGrowth data, say splitting
> into groups according to the supplement, and finding various quantities.

## <a name="less7"> </a> Lesson 12:  Another Look at the Nile Data

Here we'll learn several new concepts, using the **Nile** data as our
starting point.

If you look again at the histogram of the Nile we generated, you'll see
a gap between the lowest numbers and the rest.  In what year(s) did
those really low values occur?  Let's plot the data against time:

``` r
> plot(Nile)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/NileOverTime.png)

Looks like maybe 1912 or so was much lower than the rest.  Is this an
error?  Or was there some big historical event then?  This would require
more than R to track down, but at least R can tell us which exact year or
years correspond to the unusually low flow.  Here is how:

We see from the graph that the unusually low value was below 600.  We
can use R's **which** function to see when that occurred:

``` r
> which(Nile < 600)       
[1] 43
```

As before, make sure to understand what happened in this code.  The
expression **Nile < 600** yields 100 TRUEs and FALSEs.  The **which**
then tells us which of those were TRUEs.

So, element 43 is the culprit here, corresponding to year 1871+42=1913.
Again, we would have to find supplementary information in order to
decide whether this is a genuine value or an error, but at least now we
know the exact year.

Of course, since this is a small dataset, we could have just printed out the
entire data and visually scanned it for a low number.  But what if the
length of the data vector had been 100,000 instead of 100?  Then the
visual approach wouldn't work.  

> 📘 Pro Tip
>
> Remember, a goal of programming is to automate tasks, rather 
> than doing them by hand.

> ❄️  Your Turn
>
> There appear to be some unusually high values as well,
> e.g. one around 1875.  Determine which year this was, using the
> techniques presented here.  
>
> Also, try some similar analysis on the
> built-in **AirPassengers** data.  Can you guess why those peaks are
> occurring?

Here is another point:  That function **plot** is not quite so innocuous
as it may seem.  Let's run the same function, **plot**, but with two
arguments instead of one:

``` r
> plot(mtcars$wt,mtcars$mpg)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/MTCarsWtMPG.png)

In contrast to the previous plot, in which our data were on the vertical
axis and time was on the horizontal, now we are plotting *two* vectors,
against each other.  This enables us to explore the relation between
car weight and gas mileage.  

There are a couple of important points here.  First, as we might guess,
we see that the heavier cars tended to get poorer gas mileage.  But
here's more:  That **plot** function is pretty smart!

Why?  Well, **plot** knew to take different actions for different input
types.  When we fed it a single vector, it plotted those numbers against
time (or, against index).  When we fed it two vectors, it knew to do a scatter plot.

In fact, **plot** was even smarter than that.  It noticed that **Nile**
is not just of **'numeric'** type, but also of another class, **'ts'**
("time series"):

``` r
> is.numeric(Nile)
[1] TRUE
> class(Nile)
[1] "ts"
```

So, **plot** put years on the horizontal axis, instead of indices 1,2,3,...

And one more thing:  Say we wanted to know the flow in the year 1925.
The data start at 1871, so 1925 is 1925 - 1871 = 54 years later.  Since
the 1871 number is in element 1 of the vector, that means the flow for
the year 1925 is in element 1+54 = 55.
``` r
> Nile[55]
[1] 698
```

OK, but why did we do this arithmetic ourselves?  We should have R do
it:

``` r
> Nile[1 + 1925 - 1871]
[1] 698
```

R did the computation 1925 - 1871 + 1 itself, yielding 55, then looked
up the value of **Nile[55]**.  This is the start of your path to
programming -- we try to automate things as much as possible, doing
things by hand as little as possible.

## <a name="pause1"> </a> Lesson 13:  Pause to Reflect

> 📘 Pro Tip
>
> Repeating an earlier point:
> How does one build a house?  There of course is no set formula.  One has
> various tools and materials, and the goal is to put these together in a
> creative way to produce the end result, the house.
> 
> It's the same with R.  The tools here are the various functions, e.g.
> **mean** and **which**, and the materials are one's data.  One then must
> creatively put them together to achieve one's goal, say ferreting out
> patterns in ridership in a public transportation system.  Again, it is a
> creative process; there is no formula for anything.  But that is what
> makes it fun, like solving a puzzle.
> 
> And...we can combine various functions in order to build *our own*
> functions.  This will come in future lessons.

## <a name="less8"> </a> Lesson 14:  Introduction to Base R Graphics

One of the greatest things about R is its graphics capabilities.  There
are excellent graphics features in base R, and then many contributed
packages, with the best known being **ggplot2** and **lattice**.  These
latter two are quite powerful, and will be the subjects of future
lessons, but for now we'll concentrate on the base.

As our example here, we'll use a dataset I compiled on Silicon Valley 
programmers and engineers, from the US 2000 census.  Let's read 
in the data and take a look at the first records:

``` r
> load(url('https://github.com/matloff/fasteR/blob/master/data/prgeng.RData?raw=true'))
> head(prgeng)
       age educ occ sex wageinc wkswrkd
1 50.30082   13 102   2   75000      52
2 41.10139    9 101   1   12300      20
3 24.67374    9 102   2   15400      52
4 50.19951   11 100   1       0      52
5 51.18112   11 100   2     160       1
6 57.70413   11 100   1       0       0
```

Here we use **load** to input the data, which was stored in R's
compressed form.  This a function will be explained in [Lesson
16](#less10), but for now, the point is that this was necessary to
preserve the R factor structure of some of the variables.

Here **educ** and **occ** are codes, for levels of education and
different occupations.  For now, let's not worry about the specific
codes.  (You can find them in the
[Census Bureau document](https://www.census.gov/prod/cen2000/doc/pums.pdf).
For instance, search for "Educational Attainment" for the **educ**
variable.)

Let's start with a scatter plot of wage vs. age:

``` r
> plot(prgeng$age,prgeng$wageinc)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WageVsAge1.png)

Oh no, the dreaded Black Screen Problem!  There are about 20,000 data
points, thus filling certain parts of the screen.  So, let's just plot a
random sample, say 2500.  (There are other ways of handling the problem,
say with smaller dots or *alpha blending*.)

``` r
> rowNumbers <- sample(1:nrow(prgeng),2500)
> prgeng2500 <- prgeng[rowNumbers,]
```

Recall that the **nrow** function returns the number of rows in the
argument, which in this case is 20090, the number of rows in **prgeng**.

R's **sample** function does what its name implies.  Here it randomly
samples 2500 of the numbers from 1 to 20090.  We then extracted those
rows of **prgeng**, in a new data frame **prgeng2500**.  

> 📘 Pro Tip
>
> Note again that it's usually clearer to break complex operations into 
> simpler, smaller ones.  I could have written the more compact
> 
> ``` r
> > prgeng2500 <- prgeng[sample(1:nrow(prgeng),2500),]
> ```
> 
> but it would be hard to read that way.  I also use direct function
> composition sparingly, preferring to break
> 
> ``` r
> h(g(f(x),3)
> ```
> 
> into
> 
> ``` r
> y <- f(x) 
> z <- g(y,3) 
> h(z) 
> ```
> 
> (As noted earlier, my personal view is that pipes, though also breaking
> complex statements into smaller ones, is less clear and harder to debug,
> so I don't use them.)

So, here is the new plot:

``` r
> plot(prgeng2500$age,prgeng2500$wageinc)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WageVsAge2.png)

Note that since I plotted a random sample of rows, the ones you get may
differ from the ones I got.  The resulting graph will be largely similar
but probably  not identical.  

OK, now we are in business.  A few things worth noting:

* The relation between wage and age is not linear, indeed not even
monotonic.  After the early 40s, one's wage tends to decrease.  As with
any observational dataset, the underlying factors are complex, but it
does seem there is an age discrimination problem in Silicon Valley.
(And it is well documented in various studies and litigation.)

* Note the horizontal streaks at the very top and very bottom of the
  picture.  Some people in the census had 0 income (or close to it), as
they were not working.  And the census imposed a top wage limit of
$350,000 (probably out of privacy concerns), so that higher numbers were
truncated to that value.

We can break things down by gender, via color coding:

``` r
> plot(prgeng2500$age,prgeng2500$wageinc,col=prgeng2500$sex)
```

The **col** argument indicates we wish to color code, in this case by
gender.  It is required to be an R factor. 

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WageVsAge3.png)

The red dots are the women.  (Details below.) Are they generally paid
less than men?  There seems to be a hint of that, but detailed
statistical analysis is needed (a future lesson).  

It would be good to have better labels on the axes, and maybe smaller
dots:

``` r
> plot(pe2500$age,pe2500$wageinc,col=as.factor(pe2500$sex),xlab='age',ylab='wage',cex=0.6)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WageVsAge4.png)

Here 'xlab' meant "X label" and similarly for 'ylab'.  The argument 'cex
= 0.6' means "Draw the dots at 60% of default size."

Now, how did the men's dots come out black and the women's red?  The men
were coded 1, the women 2.  So men got color 1 in the default palette,
black, and the women color 2, red.

There are many, many other features.  More in a future lesson.

> ❄️  Your Turn
>
> Try some scatter plots on various datasets.  I suggest
> first using the above data with wage against age again, but this time
> color-coding by education level.  (By the way, 1-9 codes no college;
> 10-12 means some college; 13 is a bachelor's degree, 14 a master's, 15 a
> professional degree and 16 is a doctorate.)

## <a name="less9"> </a> Lesson 15:  More on Base Graphics

We can also plot multiple histograms on the same graph.  But the
pictures are more effective using a smoothed version of histograms,
available in R's **density** function.  Let's compare men's and women's
wages in the census data.

First we use **split** to separate the data by gender:

``` r
> wageByGender <- split(prgeng$wageinc,prgeng$sex)
> dm <- density(wageByGender[[1]])
> dw <- density(wageByGender[[2]])
```

So, **wageByGender[[1]]** will now be the vector of men's wages,
and similarly **wageByGender[[2]]** will have the women's wages.

The **density** function does not automatically draw a plot; it has the
plot information in a return value, which we've assigned to **dm** and
**dw** here.  We can now plot the graph:

``` r
> plot(dw,col='red')
> points(dm,cex=0.2)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/MWWages.png)

Why did we call the **points** function instead of **plot** in that
second line?  The issue is that calling **plot** again would destroy the
first plot; we merely want to *add points* to the existing graph.

And why did we plot the women's data first?  As you can see, the women's
curve is taller, so if we plotted the men first, part of the women's
curve would be cut off.  Of course, we didn't know that ahead of time,
but graphics often is a matter of trial-and-error to get to the picture
we really want.  (In the case of **ggplot2**, this is handled
automatically by the software.)

Well, then, what does the graph tell us?  The peak for women, occurring
at a little less than $50,000, seems to be at a lower wage than that for
men, at something like $60,000.  At salaries around, say, $125,000,
there seem to be more men than women.  (Black curve higher than red
curve.  Remember, the curves are just smoothed histograms, so, if a
curve is really high at, say 168.0, that means that 168.0 is a very
frequently-occurring value.)

> ❄️  Your Turn
>
> Try plotting multiple such curves on the same graph, for other
> data.

## <a name="less10"> </a> Lesson 16:  Writing Your Own Functions

We've seen a number of R's built-in functions so far, but here comes the
best part -- you can write your *own* functions.

Recall a line we had earlier:

``` r
> sum(Nile > 1200)
```

This gave us the count of the elements in the **Nile** data larger than 1200.  
Now, say we want the mean of those elements:

``` r
> gt1200 <- which(Nile > 1200)
> nileSubsetGT1200 <- Nile[gt1200]
> mean(nileSubsetGT1200)
[1] 1250
```

As before, we could instead write a more compact version,

``` r
> mean(Nile[Nile > 1200])
[1] 1250
```

But it's best to do it step by step at first.  Let's see how those steps
work.  Writing the code with line numbers for reference, the code is

``` r
1  gt1200Indices <- which(Nile > 1200)
2  nileSubsetGT1200 <- Nile[gt1200Indices]
3  mean(nileSubsetGT1200)
```

Let's review how this works:  

* In line 1, we find the indices in **Nile** for the elements larger than 1200.

* In line 2, we extract the subset of **Nile** consisting of those
  elements.

* In line 3, we compute the desired mean.

But we may wish to do this kind thing often, on many datasets etc.  Then
we have:

> 📘 Pro Tip
>
> If we have an operation we will use a lot, we should consider writing a
> function for it.
>
> Say we want to do the above again, but with 1350 instead of 1200.  Or,
> with the **tg$len** vector from our ToothGrowth example, with 10.2 as
> our lower bound.  We *could* keep typing the same pattern as above,
> but if we're going to do this a lot, it's better to write a function
> for it:
> 
> Here is our function:
> 
> ``` r
> > mgd <- function(x,d) mean(x[x > d])
> ```
> 
> Here I've used a compact form for convenience.  (Otherwise I'd
> need to use *blocks* to be covered in a later lesson.)  I named it 'mgd'
> for "mean of elements greater than d," but any name is fine.
> 
> Let's try it out, then explain:
> 
> ``` r
> > mgd(Nile,1200)
> [1] 1250
> > mgd(tg$len,10.2)
> [1] 21.58125
> ```
> 
> This saved me typing.  In the second call, I would have had to type
> 
> ``` r
> mean(tg$len[tg$len > 10.2])
> ```
> 
> considerably longer.  But even more importantly, I'd have to think about
> the operation each time I used it; by making a function out of it, I've
> got it ready to go, all debugged, whenever I need it.

So, how does all this work?  Again, look at the code:

``` r
> mgd <- function(x,d) mean(x[x > d])
> class(mgd)
[1] "function"
```

There is a lot going on here.  Bear with me for a moment, as I bring in
a little of the "theory" of R:
 
Odd to say, but there is a built-in function in R itself named
'function'!  We've already seen several built-in R functions, e.g.
**mean**, **sum** and **plot**.  Well, here is another,
**function**.  We're calling it here.  And its job is to build a
function. Yes, as I like to say, to my students' amusement,

> "The function of the function named **function** is to build functions!
> And the class of object returned by **function** is 'function'!"

So, in the line

``` r
> mgd <- function(x,d) mean(x[x > d])
```

we are telling R, "R, I want to write my own function.  I'd like to name
it 'mgd'; it will have arguments 'x' and 'd', and it will do 'mean(x[x >
d])'. Please build the function for me. Thanks in advance, R!"

Here we called **function** to build and return a 'function' object, and
then assigned that returned object to **mgd**.  We can then call the
latter, as we saw above, repeated here for convenience:

``` r
> mgd(Nile,1200)
[1] 1250
```

In executing

``` r
> mgd <- function(x,d) mean(x[x > d])
```


***x*** and ***d*** are known as *formal* arguments, meaning
that they are just placeholders.  For example, in 

``` r
> mgd(Nile,1200)
```

we said, "R, please execute **mgd** with **Nile** playing the role of
***x***, and 1200 playing the role of ***d***."  Here **Nile** and 1200 are
known as the *actual* arguments.

As with variables, we can pretty much name functions and their arguments
as we please.

As you have seen with R's built-in functions, a function will typically
have a return value.  In our case here, we could arrange that by writing

``` r
> mgd <- function(x,d) return(mean(x[x > d]))
```

a bit more complicated than the above version.  But the call to
**return** is not needed here, because in any function, R will return the
last value computed, in this case the requested mean.

And we can save the function for later use.  One way to do this is to
call R's **save** function, which can be used to save any R object:

``` r
> save(mgd,file='mean_greater_than_d')
```

The function has now been saved in the indicated file, which will be in
whatever folder R is running in right now.  We can leave R, and say,
come back tomorrow.  If we then start R from that same folder, we then
run

``` r
> load('mean_greater_than_d')
```

and then **mgd** will be restored, ready for us to use again.
(Typically this is not the way people save code, but this is
the subject of a later lesson.)

Let's write another function, this one to find the range of a vector,
i.e. the difference between the minimal and maximal values.  (Actually,
there is already such a function in R, unsurprisingly named 'range', but
just as an example, let's write our own.)

``` r
> rng <- function(y) max(y) - min(y)
> rng(Nile)
[1] 914
```

Here we made use of the built-in R functions **max** and **min**.

Again, the last item computed in **rng** is the subtraction, so it will
be automatically returned, just what we want.  I chose to name the
argument **y**, but it could be anything.  

> ❄️  Your Turn
>
> Try your hand at writing some simple functions along
> the lines seen here.  You might start by writing a function **cgd**,
> like **mgd** above, but returning the count of the number of
> elements in **x** that are greater than **d**.  Then may try writing a
> function **n0(x)**, that returns the number of 0s in the vector
> ***x***.  (Hint:  Make use of R's **==** and **sum**.) Another
> suggestion would be a function **hld(x,d)**, which draws a histogram
> for those elements in the vector ***x*** that are less than ***d***.
> Write at least 4 or 5 functions; the more you write, the easier it
> will be in later lessons.

Functions are R objects, just as are vectors, lists and so on.  Thus, we
can print them by just typing their names!

``` r
> mgd <- function(x,d) mean(x[x > d])
> mgd
function(x,d) mean(x[x > d])
```

For that matter, we can assign them, e.g.

``` r
> crazynamedfunction <- mgd
> crazynamedfunction(Nile,1200)
[1] 1250
```

## <a name="less11"> </a> Lesson 17:  'For' Loops

Recall that earlier we found that there were several columns in the
Pima dataset that contained values of 0, which were physiologically
impossible.  These should be coded NA.  We saw how to do that recoding
for the glucose variable:

``` r
> pima$glucose[pima$glucose == 0] <- NA
```

But there are several columns like this, and we'd like to avoid doing
this all repeatedly by hand.  (What if there were several *hundred* such
columns?) Instead, we'd like to do this *programmatically*.  This can be
done with R's **for** loop construct (which by the way most programming
languages have as well).

Let's first check which columns seem appropriate for recoding.  Recall
that there are 9 columns in this data frame.

``` r
> for (i in 1:9) print(sum(pima[,i] == 0))
[1] 111
[1] 5
[1] 35
[1] 227
[1] 374
[1] 11
[1] 0
[1] 0
[1] 500
```

This is known in the programming world as a *'for' loop*.  

The 'print(etc.)' is called the *body* of the loop.  The 'for (i in
1:9)' part says, "Execute the body of the loop with i = 1, then execute
it with i = 2, then i = 3, etc. up through i = 9."

In other words, the above code instructs R to do the following:

``` r
i <- 1
print(sum(pima[,i] == 0))
i <- 2
print(sum(pima[,i] == 0))
i <- 3
print(sum(pima[,i] == 0))
i <- 4
print(sum(pima[,i] == 0))
i <- 5
print(sum(pima[,i] == 0))
i <- 6
print(sum(pima[,i] == 0))
i <- 7
print(sum(pima[,i] == 0))
i <- 8
print(sum(pima[,i] == 0))
i <- 9
print(sum(pima[,i] == 0))
```

And this amounts to doing

``` r
print(sum(pima[,1] == 0))
print(sum(pima[,2] == 0))
print(sum(pima[,3] == 0))
print(sum(pima[,4] == 0))
print(sum(pima[,5] == 0))
print(sum(pima[,6] == 0))
print(sum(pima[,7] == 0))
print(sum(pima[,8] == 0))
print(sum(pima[,9] == 0))
```

Now, it's worth reviewing what those statements do, say the first.  Once
again, **pima[,1] == 0** yields a vector of TRUEs and FALSEs, each
indicating whether the corresponding element of column 1 is 0.  When we
call **sum**, TRUEs and FALSEs are treated as 1s and 0s, so we get the
total number of TRUEs -- which is a count of the number of elements in that
column that are 0, exactly what we wanted.

The variable **i** in "for (i in 1:9)..." is known as the *index* of the
loop.  It's just an ordinary R variable, so name it what you wish.
Instead of **i**, we might name it, say, **colNumber**.

``` r
for (colNumber in 1:9) print(sum(pima[,colNumber] == 0))
```

A technical point:  Why did we need the explicit call to **print**?
Didn't we say earlier that just typing an expression at the R '>' prompt
will automatically print out the value of the expression?  Ah yes -- but
we are not at the R prompt here!  Yes, in the expanded form we see
above,

``` r
print(sum(pima[,1] == 0))
print(sum(pima[,2] == 0))
print(sum(pima[,3] == 0))
print(sum(pima[,4] == 0))
print(sum(pima[,5] == 0))
print(sum(pima[,6] == 0))
print(sum(pima[,7] == 0))
print(sum(pima[,8] == 0))
print(sum(pima[,9] == 0))
```

each command would be issued at the prompt.  But in the 
**for** loop version

``` r
for (i in 1:9) print(sum(pima[,i] == 0))
```

we are calling **print** from *within the loop*, not at the prompt.
So, the explicit call to **print** is needed.

We see in the output of the loop that there are a lot of erroneous 0s in
this dataset, e.g. 35 of them in column 3.  We probably have forgotten
which column is which, so let's see, using yet another built-R function:

 
``` r
> colnames(pima)
[1] "pregnant"  "glucose"   "diastolic" "triceps"   "insulin"   "bmi"      
[7] "diabetes"  "age"       "test"     
```

Ah, so column 3 was 'diastolic'.

Since some women will indeed have had 0 pregnancies, that column should
not be recoded.  And the last column states whether the test for
diabetes came out positive, 1 for yes, 0 for no, so those 0s are
legitimate too.  

But 0s in columns 2 through 6 ought to be recoded as NAs.  And the fact
that it's a repetitive action suggests that a **for** loop can be used
there too:

``` r
> for (i in 2:6) pima[pima[,i] == 0,i] <- NA
```

You'll probably find this line quite challenging, but be patient and, as
with everything in R, you'll find you can master it.  Here goes:

First, let's write it in more easily digestible form:

``` r
> for (i in 2:6) {
+    zeroIndices <- which(pima[,i] == 0)
+    pima[zeroIndices,i] <- NA
+ }
```

You can enter the code for a loop or function etc. line by line at the
prompt, as we've done here.  R helpfully uses its '+' prompt (which I
did *not* type) to remind me that I am still in the midst of typing the
code. (After the '}' I simply hit Enter to tell R that I'm done.)

Here I intended the body of the loop to consist of a *block* of two
statements, not one, so I needed to tell R that, by enclosing them with
'{' and '}.

For your convenience, below is the code itself, no '+' symbols.  You can
copy-and-paste into R, with the result as above.

```
for (i in 2:6) {
   zeroIndices <- which(pima[,i] == 0)
   pima[zeroIndices,i] <- NA
}
```

So, the block (two lines here) will be executed with **i** = 2, then 3,
4, 5 and 6.  The line 

``` r
zeroIndices <- which(pima[,i] == 0)
```

determines where the 0s are in column **i**, and then the line

``` r
 pima[zeroIndices,i] <- NA
```

replaces those 0s by NAs.

> 📘 Pro Tip
>
> Note that I have indented the two lines in the block.  This is not
> required but is considered good for clear code, in order to easily
> spot the block when you or others read the code. 

Sometimes our code needs to leave a loop early, which we can do using
the R **break** construct.  Say we are adding cubes of numbers
1,2,3,..., and for some reason want to determine which sum--if any-- is
the first to exceed **s**:

``` r
> f
function(n,s) 
{
   tot <- 0
   for (i in 1:n) {
      tot <- tot + i^3
      if (tot > s) {
         print(i)
         break
      }
      if (i == n) print('failed')
   }
}
> f(100,345)
[1] 6
> f(5,345)
[1] "failed"

```

If our accumulated total meets our goal, we leave the loop.

A better approach is to use 'while' loops, covered later in this
tutorial.

> 📘 Pro Tip
>
> There is a school of thought among some R enthusiasts that one should
> avoid writing loops, using something called *functional programming*.
> We will cover this in Lesson 28, but I do not recommend it for R
> beginners.  
>
> As the name implies, functional programming uses functions, and it
> takes a while for most R beginners to master writing functions.  It
> makes no sense to force beginners to use functional programming before
> they really can write function code well.  I myself, with my several
> decades as a coder, write some code with loops and some with
> functional programming.  
>
> I've seen some beginning R coders actually apologize on Twitter for
> using a loop!  Write in whatever style you feel comfortable
> with, rather than being a "slave to fashion."

## <a name="ftnbl"> </a> Lesson 18:  Functions with Blocks 

Blocks are usually key in defining functions.  Let's generalize the
above code in the Loops lesson, writing a function that replaces 0s by
NAs in specified columns in general data frames, not just **pima** as
before.

``` r
     1	zerosToNAs <- function(d,cols)
     2	{
     3	   for (j in cols) {
     4	      NArows <- which(d[,j] == 0)
     5	      d[NArows,j] <- NA
     6	   }
     7	   d
     8	}
```

(We've added line numbers to this display for convenence.)

Here the formal argument **d** is the data frame to be worked on, and
**cols** specifies the columns in which 0s are to be replaced.

The loop goes through **d**, one column at a time.  Since **d[,j]**
means all of column **j** of **d**, then **which(d[,j] == 0)** will give
us the indices in that column of elements that are 0s.  Those indices in
turn are row numbers in **d**.  In other words, **NArows** is a vector
cntaining the row numbers of the 0s in column **j**.  In line 5, then,
we replace the 0s we've found in column **j** by NAs.  Before
continuing, work through this little example in your mind:

``` r
> d <- data.frame(x=c(1,0,3),y=c(0,0,13)) 
> d
  x  y
1 1  0
2 0  0
3 3 13
> which(d[,2] == 0)
[1] 1 2  # ah yes; the 0 elements in column 2 are at indices 1 and 2
```

Returning to the above loop code, note that when we reach line 7, we've
already finished the loop, and exited from it.  So, we are ready to
return the new value of **d**.  Recall that we could do this via the
expression **return(d)**, but we can save ourselves some typing by
simply writing 'd'.  That value becomes the last value computed, and R
automatically returns that last value.

We could use this in the Pima data:

``` r
> pima <- zerosToNAs(pima,2:6)
```

There is an important subtlety here.  All of this will produce a new
data frame, rather than changing **pima** itself.  That does look odd;
isn't **d** changing, and isn't **d** the same as **pima**?  Well, no;
**d** is only a *separate copy* of **pima**. So, when **d** changes,
**pima** does not.  So, if we want **pima** to change, we must reassign
the output of the function back to **pima**, as we did above.

> ❄️  Your Turn
>
> Write a function with call form **countNAs(dfr)**,
> which prints the numbers of NAs in each column of the data frame
> **dfr**.  You'll need to use the built-in **is.na** functon; execute
> **is.na(c(5,NA,13,28,NA))** at the R command prompt to see what it
> does.  Test it on a small artificial dataset that you create.

## <a name="edt"> </a> Lesson 19:  Text Editing and IDEs

In trying out our function **zeroToNAs** above, you probably used your
computer's mouse to copy-and-paste from this tutorial into your machine.
Your screen would then look like this:

```
> zerosToNAs <- function(d,cols) 
+ {
+    zeroIndices <- which(d[,cols] == 0)
+    d[zeroIndices,cols] <- NA
+    d
+ }
```

But this is unwieldy.  Typing it in line by line is laborious and
error-prone.  And what if we were to change the code?  Must we type in
the whole thing again?  We really need a *text editor* for this.  Just
as we edit, say, reports, we do the same for code.  

Here are your choices:

1. If you are already using an IDE, say RStudio, you simply edit
in the designated pane.

2.  If you are using an external editor, say vim or emacs,
just open a new file and use that workspace.

3.  For  those not using these, we'll just use R's built-in **edit**
    function.  

Option 3 is fine for now, but eventually you'll want to use either
Option 1 or 2.  You may wish to start with one of those options now,
before going further. 

We have details on getting start with RStudio in the <a
href="#ide">Appendix</a> at the end of this document.  **Warning:** 
As noted earlier, one major R Users Group described RStudio as
"overwhelming." But it is quite easy if you resist the temptation (or
the exhortations of others) to learn it all at once.  As long as you
stick to the basics in the Appendix, you'll find it quite easy; you can
learn the advanced tricks later.

Consider the following toy example:

``` r
f <- function(x,y)
{
   s <- x + y
   d <- x - y
   c(s,d)
}
```

It finds the sum and difference of the inputs, and returns them as a
two-element vector.

If you are using RStudio or an external editor, copy-and-paste the above
code into the workspace of an empty file.  

Or, to create **f** using **edit**, we would do the following:

``` r
> f <- edit()
```

This would invoke the text editor, which will depend on your machine.
It will open your text editor right there in your R window.  Type the
function code, then save it, using the editor's Save command.  

**IMPORTANT:** Even if you are not using **edit**, it's important to
know what is happening in that command above.

a.  **edit** itself is a function.  Its return value is the code you
typed in!  

b.  That code is then assigned to **f**, which you can now call

If you want to change the function, in the RStudio/external editor case,
just edit it there.  In the **edit** case, type

``` r
> f <- edit(f)
```

This again opens the text editor, but this time with the current **f**
code showing.  You edit the code as desired, then as before, the result
is reassigned to **f**.

How do you then run the code, say for computing **f(5,2)**?

* If you had created **f** using **edit**, then execute as usual:


``` r
> f(5,2)
```

* If you had used an external text editor, say saving the code into the
  file **a.R**, then

``` r
> source('a.R')
``` 

loads file, and then you run as above.

* In RStudio, click on Source, then run as above.

## <a name="ifelse"> </a> Lesson 20:  If, Else, Ifelse

In our Census data example above, it was stated that education codes 0-9
all corresponded to having no college education at all.  For instance, 9
means high school graduate, while 6 means schooling through the 10th
grade.  (Of course, few if any programmers and engineers have
educational attainment level below college, but this dataset was
extracted from the general data.)  13 means a bachelor's degree.

Suppose we wish to color-code the wage-age graph in an earlier lesson by
educational attainment. Let's amalgamate all codes under 13, giving them
the code 12.

The straightforward but overly complicated, potentially slower way would
be this:

``` r
> head(pe$educ,15)
 [1] 13  9  9 11 11 11 12 11 14  9 12 13 12 13  6
> for (i in 1:nrow(pe)) {
+    if (pe$educ[i] < 13) pe$educ[i] <- 12 
+ }
> head(pe$educ,15)
 [1] 13 12 12 12 12 12 12 12 14 12 12 13 12 13 12
```

For pedagogical clarity, I've inserted "before and after" code, using
**head**, to show the **educ** did indeed change where it should.

The **if** statement works pretty much like the word "if" in English.
First **i** will be set to 1 in the loop, so R will test whether
**pe$educ[1]** is less than 13.  If so, it will reset that element to
12; otherwise, do nothing.  Then it will do the same for **i** equal to
2, and so on.  You can see above that, for instance, **pe$educ[2]** did
indeed change from 9 to 12.

But there is a slicker (and actually more standard) way to do this
(re-read the data file before running this, so as to be sure the code
worked):

``` r
> edu <- pe$educ
> pe$educ <- ifelse(edu < 13,12,edu)
```

(Once again, we've broken what could have been one line into two, for
clarity.)

Now how did that work?  As you see above, R's **ifelse** function
has three arguments, and its return value is a new vector, that in this
case we've reassigned to **pe$educ**.  Here, **edu < 12** produces a vector
of TRUEs and FALSEs.  For each TRUE, we set the corresponding element of
the output to 12; for each FALSE, we set the corresponding element of
the output to the corresponding element of **edu**.  That's exactly what
we want to happen.

So, we can now produce the desired graph:

``` r
> plot(pe$age,pe$wageinc,col=edu)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WageAgeEdu.png)

By the way, an ordinary **if** can be paired with **else** too.  For
example, say we need to set **y** to either -1 or 1, depending on
whether **x** is less than 3.  We could write

``` r
if (x < 3) y <- -1 else y <- 1
```

One more important point:  Using **ifelse** instead of a loop in the
above example is termed *vectorization*.  The name comes from the fact
that **ifelse** operates on vectors, while in the loop we operate on one
individual element at a time.

Vectorized code is typically much more compact than loop-based code, as
was the case here.  In some cases, though certainly not all, the
vectorized version will be much faster.

By the way, note the remark above, "**ifelse** operates on vectors."
Let's revisit the above statement with this point in mind.

``` r
> pe$educ <- ifelse(edu < 13,12,edu)
```

It would be helpful to keep in mind that both the 13 and the 12 will be
recycled, as expained before.  The **edu** vector is 20090 elements
long, so in order to be compared on an element-to-element basis, the 13
has to be recycled to a vector consisting of 20090 elements that are
each 13.  The same holds for the 12.

Here's another example.  Say we wish to recode the **Nile** data to a
new vector **nile**, with values 1, 2 and 3, for the cases in which the
value is less than 800, between 800 and 1150 inclusive, or greater than
1150.  We could do this:

``` r
> nile <- ifelse(Nile > 1150,3,2)
> nile <- ifelse(Nile < 800,1,nile)
# check it 
> table(nile)
nile
 1  2  3 
26 62 12 
```

After the first call to **ifelse**, the vector **nile** (not **Nile**;
variable names etc. are case-sensitive) consists of 2s and 3s.  The 3s
are right, but the 2s need further work, hence the second call.  

But let's look closely at the second call, to review some things we've
seen before:

1. The expression **Nile > 1150** evaluates to a vector of 100 TRUEs and
   FALSEs.  

2. The singleton value 800 is then recycled to one hundred
800s, to set up the '<'.  Let's call the result of that '<' operation w.

3. Then **ifelse(Nile < 800,1,nile)** says, "For each element in the vector
w that is TRUE, write down a 1; for each element that is FALSE, write
down whatever the corresponding value is in **nile**."

Well, congratulations!  With **for** and now **ifelse**, you've really
gotten into the programming business.  We'll be using them a lot in the
coming lessons.

> ❄️  Your Turn
>
> Write a **for** loop version of the **Nile** example
> above.

## <a name="keepfit"> </a> Lesson 21:  Do Professional Athletes Keep Fit?

Many people gain weight as they age.  But what about professional
athletes?  They are supposed to keep fit, after all.  Let's explore this
using data on professional baseball players.  (Dataset courtesy of the
UCLA Statistics Dept.)

``` r
> load(url('https://github.com/matloff/fasteR/blob/master/data/mlb.RData?raw=true'))
> head(mlb)
             Name Team       Position Height Weight   Age PosCategory
1   Adam_Donachie  BAL        Catcher     74    180 22.99     Catcher
2       Paul_Bako  BAL        Catcher     74    215 34.69     Catcher
3 Ramon_Hernandez  BAL        Catcher     72    210 30.78     Catcher
4    Kevin_Millar  BAL  First_Baseman     72    210 35.43   Infielder
5     Chris_Gomez  BAL  First_Baseman     73    188 35.71   Infielder
6   Brian_Roberts  BAL Second_Baseman     69    176 29.39   Infielder
> class(mlb$Height)
[1] "integer"
> class(mlb$Name)
[1] "factor"
```

(As usual, after reading in the data, we took a look around, glancing at
the first few records, and looking at a couple of data types.)

Now, as a first try in assessing the question of weight gain over time,
let's look at the mean weight for each age group.  In order to have
groups, we'll round the ages to the nearest integer first, using the R
function, **round**, so that e.g.  21.8 becomes 22 and 35.1 becomes 35.

Let's explore the data using R's **table** function.

``` r
> age <- round(mlb$Age)
> table(age)
age
 21  22  23  24  25  26  27  28  29  30  31  32  33  34  35  36  37  38  39  40 
  2  20  58  80 103 104 106  84  80  74  70  44  44  32  32  22  20  12   6   7 
 41  42  43  44  49 
  9   2   2   1   1 
```

Not surprisingly, there are few players of extreme age -- e.g. only two of
age 21 and one of age 49.  So we don't have a good sampling at those age
levels, and may wish to exclude them (which we will do shortly).

Now, how do we find group means?  It's a perfect job for the **tapply**
function, in the same way we used it before:

``` r
> taout <- tapply(mlb$Weight,age,mean)
> taout
      21       22       23       24       25       26       27       28 
215.0000 192.8500 196.2241 194.4500 200.2427 200.4327 199.2925 203.9643 
      29       30       31       32       33       34       35       36 
199.4875 204.1757 202.8429 206.7500 203.5909 204.8750 209.6250 205.6364 
      37       38       39       40       41       42       43       44 
203.2000 200.6667 208.3333 207.8571 205.2222 230.5000 229.5000 175.0000 
      49 
188.0000 
```

To review:  The call to **tapply** instructed R to split the
**mlb$Weight** vector according to the corresponding elements in the
**age** vector, and then find the mean in each resulting group.  This
gives us exactly what we want, the mean weight in each age group.

So, do we see a time trend above?  Again, we should dismiss the extreme
low and high ages, and we cannot expect a fully consistent upward trend over
time, because each mean value is subject to sampling variation.  (We
view the data as a sample from the population of all professional
baseball players, past, present and future.)  That said, it does seem
there is a slight upward trend; older players tend to be heavier!

By the way, note that **taout** is vector, but with additional
information, in that the elements have names, in this case the ages.  In
fact, we can extract the names into its own vector if needed:

``` r
> names(taout)
 [1] "21" "22" "23" "24" "25" "26" "27" "28" "29" "30" "31" "32" "33"
"34" "35"
[16] "36" "37" "38" "39" "40" "41" "42" "43" "44" "49"
```

Let's plot the means against age.  We'll just plot the means that are
based on larger amounts of data.  So we'll restrict it to, say, ages 23
through 35, all of whose means were based on at least 30 players.  That
age range corresponded to elements 3 through 15 of **taout**, so here is
the code for plotting:

``` r
> plot(23:35,taout[3:15])
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/MLB.png)

There does indeed seem to be an upward trend in time.  Ballplayers
should be more careful!  

(Though it is far beyond the scope of this tutorial, which is on R
rather than statistics, it should be pointed out that interpretation of
the regression coefficients must be done with care.  It may be, for
instance, that heavier players tend to have longer careers.  If so,
fitting our linear form to data that has many older, heavier players may
misleadingly imply that most individual players gain weight as they age.
And of course, they would insist the gained weight
is all muscle. :-) )

Note again that the **plot** function noticed that we supplied it with
two arguments instead of one, and thus drew a two-dimensional scatter
plot.  For instance, in **taout** we see that for age group 25, the mean
weight was 200.2427, so there is a dot in the graph for the point
(25,200.2427).

> ❄️  Your Turn
>
> There are lots of little experiments you can do on this
> dataset.  For instance, use **tapply** to find the mean weight for
> each position; is the stereotype of the "beefy" catcher accurate, i.e.
> is the mean weight for that position higher than for the others?
> Another suggestion:  Plot the number of players at each age group, to
> visualize the ages at which the bulk of the players fall.
 
## <a name="linreg1"> </a> Lesson 22:  Linear Regression Analysis, I

Looking at the picture in the last lesson, it seems we could draw a
straight line through that cloud of points that fits the points pretty
well.  Here is where linear regression analysis comes in. 

We of course cannot go into the details of statistical methodology here,
but it will be helpful to at least get a good definition set:

> As mentioned, we treat the data as a sample from the (conceptual)
> population of all players, past, present and future.  Accordingly,
> there is a population mean weight for each age group.  It is assumed
> that those population means, when plotted against age, lie on some
> straight line.

In other words, our model is 

mean weight = &beta;<sub>0</sub> + &beta;<sub>1</sub> height

where &beta;<sub>0</sub> and &beta;<sub>1</sub> are the 
intercept and slope of the population regression line.

So, we need to use the data to estimate the slope and intercept of that
straight line, which R's **lm** ("linear model") function does for us.
We'll use the original dataset, since the one with rounded ages was just
to guide our intuition.

``` r
> lm(Weight ~ Age,data=mlb)

Call:
lm(formula = Weight ~ Age, data = mlb)

Coefficients:
(Intercept)          Age  
   181.4366       0.6936  
```
Here the call instructed R to estimate the regression line of weight
against age, based on the **mlb** data.

So the estimated slope and intercept are 0.6936 and 181.4366,
respectively.  (Remember, these are just sample estimates.  We don't
know the population values.) R has a provision by which we can draw the
line, superimposed on our scatter plot:

``` r
> abline(181.4366,0.6936)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/Add_abline.png)

> ❄️  Your Turn
>
> In the **mtcars** data, fit a linear model of the
> regression of MPG against weight; what is the estimated
> effect of 100 pounds of extra weight?

## <a name="s3"> </a> Lesson 23:  S3 classes

> 📘 Pro Tip
>
> Remember, the point of computers is to alleviate us of work.  We should
> avoid doing what the computer could do.  For instance,
> consider the graph in the last lesson: We had typed
> 
> ``` r
> > abline(181.4366,0.6936)
> ```
> 
> but we really shouldn't have to type those numbers in by hand -- and we
> don't have to.  Here's why:

As mentioned earlier, R is an *object-oriented language*. Everthing is
an *object*, and every object has a *class*.  One of the most common
class structures is called 'S3'.  

When we call **lm**, the latter returns an S3 object of 'lm' class:

``` r
> lmout <- lm(Weight ~ Age,data=mlb)
> class(lmout)
[1] "lm"
```

A handy way to take a quick glance at the contents of an object is
via the **str** function:

``` r
> str(lmout)
List of 12
 $ coefficients : Named num [1:2] 181.437 0.694
  ..- attr(*, "names")= chr [1:2] "(Intercept)" "Age"
...
...
 - attr(*, "class")= chr "lm"
```

Our use of ... here is to indicate that we've omitted a lot of the
output.  But a couple of things stand out even in this excerpt:

1. Our **lmout** object here is an R list (which is the nature of S3
   objects).  That R list here has 12 elements.

2. But it has an extra *attribute*, which is the class name, in this
   case **'lm'**.  (So the designers of R simply chose to name the class
after the function, which is not always the case.)

3. The first of the elements of this R list is named 'coefficients', and it
   is a vector containing the slope and intercept.

So, we don't have to type the slope and intercept in by hand after all.

``` r
> cfs <- lmout$coefficients
> abline(a = cfs[1], b = cfs[2])
```

By the way, **abline** is actually a *generic* function, like **print**
and **plot**.  That is, it works on various kinds of object classes.
One such class is 'lm'!  So if we want to be clever, we can add our line
to the graph using this approach:

``` r
> abline(lmout)
```

The internal code for **abline** recognizes that **lmout** is of 'lm'
class, and thus knows it can find the coefficients in the **coefficients**
element of the **lmout** list.  Saves us a lot of work!

Now, what about our original question -- do baseball players gain weight
as they age?  The answer appears to be yes; for each additional year of
age, the estimated mean age increases by about 0.7 pound.  That's about
7 pounds in 10 years, rather remarkable.

Again, this is only an estimate -- 181.437 and 0.694 are estimates of
the unknown population values &beta;<sub>0</sub> and &beta;<sub>1</sub>.
-- generated from sample data.  We can get an idea of the accuracy of
this estimate by calculating a *confidence interval*, but we'll leave
that for statistics courses.

But we can do more right now.  One might ask, Shouldn't we also account
for a player's height, not just his age?  After all, taller people tend
to be heavier.  Yes, we should do this:

``` r
> lmo <- lm(Weight ~ Height + Age, data=mlb)
> lmo

Call:
lm(formula = Weight ~ Height + Age, data = mlb)

Coefficients:
(Intercept)       Height          Age  
  -187.6382       4.9236       0.9115  
```

Here we instruct R to find the estimated regression function of weight,
using both height and age as predictors.  The '+' doesn't mean addition; it
is simply a delimiter between the predictors height and age in our regression
specification.

So the new model is 

mean weight = &beta;<sub>0</sub> + &beta;<sub>1</sub> height  + &beta;<sub>2</sub> age


This says:

    estimated mean weight = -187.6382 + 4.9236 height + 0.9115 age

So, under this more refined analysis, things are even more pessimistic;
players on average gain about 0.9 pounds per year.  And by the way, an
extra inch of height corresponds on average to about 4.9 pounds of extra
weight; taller players are indeed heavier, as we surmized.

<span style="color:red">Warning:</span>
Though this is not a statistics tutorial *per se*, an important point
should be noted.  Regression analysis has two goals, Description and
Prediction.  Our above analysis was aimed at the former -- we want to
*describe* the nature of fitness issues in pro baseball players. As we
saw, a coefficient can change quite a lot when another predictor is
added to the model, and in fact can even change sign ("Simpson's
Paradox").  Suppose for instance the shorter players tend to have longer
careers.  If we do *not* include height in our model, that omission
might bias the age coefficient downward.  Thus great care must be taken
in interpreting coefficients in the Description setting.  For
Prediction, it is not as much of an issue.

> ❄️  Your Turn
>
> In the **mtcars** data, fit a linear model of the
> regression of MPG against weight and horsepower; what is the estimated
> effect of 100 pounds of extra weight, for fixed horsepower?

## <a name="less15"> </a> Lesson 24:  Baseball Player Analysis (cont'd.)

This lesson will be a little longer and more detail-oriented.  But it
will give you more practice on a number of earlier topics, and will also
bring in some new R functions for you.  Spending extra time on
this lesson will pay substantial dividends.

We might wonder whether the regression lines differ much among player
positions.  (A more statistical approach would be to include
*interaction terms* in the model.) Let's first see what positions are
tabulated:

``` r
> table(mlb$PosCategory)
   Catcher  Infielder Outfielder    Pitcher 
        76        210        194        535 
```

Let's fit the regression lines separately for each position type. 

There are various ways to do this, involving avoidance of loops to
various degrees.  But we'll keep it simple, which will be clearer.

First, let's split the data by position.  You might at first think this
is easily done using the **split** function, but that doesn't work,
since that function is for splitting vectors.  Here we wish to split a
data frame.

So what can be done instead?  We need to think creatively here.  One
solution is this:

We need to determine the row numbers of the catchers, the row numbers of
the infielders and so on.  So we can take all the row numbers,
**1:nrow(mlb)**, and apply **split** to that vector!

``` r
> rownums <- split(1:nrow(mlb),mlb$PosCategory)
```

There are 1015 rows in **mlb**, so this says, "Take the row numbers
1:1015, and split them according to the **PosCategory** column of **mlb**."
The resulting piles of row numbers will be the row numbers for catchers,
then the row numbers for infielders and so on.

As usual, following an intricate operation like this, we should glance
at the result:

``` r
> str(rownums)
List of 4
 $ Catcher   : int [1:76] 1 2 3 35 36 66 67 68 101 102 ...
 $ Infielder : int [1:210] 4 5 6 7 8 9 37 38 39 40 ...
 $ Outfielder: int [1:194] 10 11 12 13 14 15 16 43 44 45 ...
 $ Pitcher   : int [1:535] 17 18 19 20 21 22 23 24 25 26 ...
```

So the output is an R list; no surprise there, as we knew beforehand 
that **split** produces an R list.  Also not surprisingly, the elements
of the list are named "Catcher" etc.  So for example, the third
outfielder is in row 12 of the data frame.

> 📘 Pro Tip
>
> The idea here, using **split** on **1:nrow(mlb)**, was a bit of a trick.
> Actually, it is a common ploy for experienced R coders, but you might
> ask, "How could a novice come up with this idea?"  
>
> The answer, as noted several times already here, is that programming
> is a creative process.  This was a creative solution.
>
> Creativity may not come quickly!  Of course, there are many forums on
> the Web at which you can ask questions, e.g. Stack Overflow, but
> *resist the temptation to immediately go that route*.  Don't give up!
> The more you think about a problem, the more skilled you will get,
> even if you sometimes come up empty-handed.  

Now, remember, a nice thing about R lists is that we can reference their
elements in various ways.  The first element above, for instance, is any
of **rownums$Catcher**, **rownums[['Catcher']]** and **rownums[[1]]**,
This versatility is great, as for example we can use the latter two
forms to write loops.

And a loop is exactly what we need here.  (One can also do this with
*functional programming*, which we will cover in a later lesson.) We
want to call **lm** four times, once for each position.  We could do
this, say, with a loop beginning with

``` r
for (i in 1:4)
```

to iterate through the four position types, but it will be clearer if we
use the names:

``` r
for (pos in c('Catcher','Infielder','Outfielder','Pitcher'))
```

Recall 'for' loops are of the form

``` r
for (variable in vector)...
```

Instead of having a numeric vector, e.g. the 1:4 above, we now have a
character vector, which each element of the vector being a character
string, i.e. 'Catcher', 'Infielder' etc., but the principles are the same.

We could have **lm** and **print** calls in the body of the loop.
But let's be a little fancier, building up a data frame with the output.
We'll start with an empty frame, and keep adding rows to it.

Our code is

``` r
posNames <- c('Catcher','Infielder','Outfielder','Pitcher')
m <- data.frame()
for (pos in posNames) {
   posRows <- rownums[[pos]]
   lmo <- lm(Weight ~ Age, data = mlb[posRows,])
   newrow <- lmo$coefficients
   m <- rbind(m,newrow)
}
```

Here is the output:

``` r
> m
  X180.828029016113 X0.794925225995348
1          180.8280          0.7949252
2          170.2466          0.8589593
3          176.2884          0.7883343
4          185.5994          0.6543904
```

Some key things to note here.  

*  The overall strategy is to start with an empty data frame, then keep
   adding rows to it, one row of regression coefficients per player position.

*  In order to add rows to **m**, we used R's **rbind** ("row bind")
   function.  The expression **rbind(m,newrow)** forms a new data frame,
   by tacking **newrow** onto **m** and returning the result.  Here we
   reassign the result back to **m**, also a common operation.  (Note
   carefully: The **rbind** operation did not change **m**; it merely
   created a new data frame.  To update **m**, we needed to assign that
   new data frame to **m**.) By the way, there is also a **cbind**
   function for columns.
   
*  In the call to **lm**, we used **mlb[rownums[[pos]],]** instead of
   **mlb** as previously, since here we wanted to fit a regression line
   on each position subgroup.  So, we restricted attention to only those
   rows of **mlb** for which the position was equal to the current value
   of **pos**.

So, what happens is:  **m** is initially an empty data frame.  Then the
loop, for its first iteration, sets **pos** to 'Catcher'.  Then a
regression line will be fit to the rows of **mlb** that are for
catchers.  That fit is returned to us from **lm**, and we extract the
coefficients, assigning them to **lmo**.  (Once again, the name is
arbitrary; I chose this one to symbolize "lm output.")  We extract the
coefficients and tack them on at the end of **m**.

> 📘 Pro Tip
>
> This is a very common *design
> pattern* in R (and most other languages), to build up a data frame (or
> similar structure) row by row in a loop.

Nice output, with the two columns aligned.  But those column names are
awful, and the row labels should be nicer than 1,2,3,4.  We can fix
these things:

``` r
> row.names(m) <- posNames
> names(m) <- c('intercept','slope')
> m
           intercept     slope
Catcher     180.8280 0.7949252
Infielder   170.2466 0.8589593
Outfielder  176.2884 0.7883343
Pitcher     185.5994 0.6543904
```

What happened here?  We earlier saw the built-in **row.names** function,
so that setting row names was easy.  But what about the column names?
Recall that a data frame is actually an R list, consisting of several
vectors of the same length, which form the columns.  So, **names(m)** is
the names of the columns.

So with a little finessing here, we got some nicely-formatted output.
Moreover, we now have our results in a data frame for further use.  For
instance, we may wish to plot the four lines on the same graph, and we
would use rows of the data frame as input.

A little more finessing is possible.  Look at the line

``` r
posNames <- c('Catcher','Infielder','Outfielder','Pitcher')
```

We're using a computer!  We shouldn't have to type out these names by
hand, as I did in this line.  In fact, we already have them in one of
our R objects, **rownums**; recall our earlier check:

``` r
> str(rownums)
List of 4
 $ Catcher   : int [1:76] 1 2 3 35 36 66 67 68 101 102 ...
 $ Infielder : int [1:210] 4 5 6 7 8 9 37 38 39 40 ...
 $ Outfielder: int [1:194] 10 11 12 13 14 15 16 43 44 45 ...
 $ Pitcher   : int [1:535] 17 18 19 20 21 22 23 24 25 26 ...
```

The elements of the R list **rownums** are the names of the positions!
So, the better way to set **posNames** is

``` r
posNames <- names(rownums)
```

> 📘 Pro Tip
>
> Again, the reader may be thinking,
> "How in the world would I have been able to realize this?"  Again, the
> answer is that as you acquire more experience in coding, you will be
> more and more able to come up with creative insights like this.  Patience!

Finally, what about those numerical results?  There is substantial
variation in those estimated slopes, but again, they are only estimates.
The question of whether there is substantial variation at the population
level is one of statistical inference, to be discussed in a later
lesson.

## <a name="cran"> </a> Lesson 25:  R Packages, CRAN, Etc.

One of the great things about R is that are tens of thousands of
packages that were developed by users and then contributed to
the [CRAN repository](https://cran.r-project.org).  As of December 2020,
there were nearly 17,000 packages there.  If you need to do some special
operation in R, say spatial data analysis, it may well be in there. 
You might take the [CRAN Task Views](https://cran.r-project.org/web/views/) 
as your starting point, or simply use Google, e.g. plugging in the search 
term "CRAN spatial data." 
Other good sources of public R packages are
[Bioconductor](https://www.bioconductor.org/) and useRs' personal GitHub
pages.  

Below, we'll introduce one of the most popular user-contributed
packages, **ggplot2**.  But first, how does one install and load
packages?

First, one needs a place to put the packages.  UseRs often designate a
special folder/directory for their packages (both those they download
and ones they write themselves).  I use 'R' in my home directory for
that purpose, but if you don't specify a folder, your package installer
will choose one for you.  It won't matter as long as you are consistent.
I'll assume you don't specify a package folder.

To install, say, **ggplot2**, you can type at the R prompt,

``` r
> install.packages('ggplot2')
```

Or in RStudio, choose Tools | Install Packages...

When you want to use one of your installed packages, you need to tell R
to load it, e.g. by typing at the R prompt,

``` r
> library(ggplot2)
```

In RStudio, click the Packages button and select the one you want; there
may be a delay while R makes a list of all your packages.

Later, you'll write your own R packages.  We won't cover that here, but
there are many good tutorials for this on the Web.

## <a name="advanced"> </a> Lesson 26:  A Pause, Before Going on to Advanced Topics

At this point, you have a pretty good grounding in R.  You are capable
of doing lots of things in R.  It may be all you need, but even if not,
you know enough to ask a question online if you get stuck on something.

The remaining topics are more advanced, and lessons will be somewhat
longer and more detailed that the previous ones.  But you are still
strongly encouraged to go through them, as they will not only cover new
topics but also give you deeper insight into the earlier material.

## <a name="gg2first"> </a> Lesson 27:  The ggplot2 Graphics Package

Now, on to **ggplot2**.

The **ggplot2** package was written by Hadley Wickham, who later became
Chief Scientist at RStudio.  It's highly complex, with well over 400
functions, and rather abstract, but quite powerful.  We will touch on it
at various points in this tutorial, while staying with base-R graphics
when it is easier to go that route.

Now to build up to using **ggplot2**, let's do a bit more with base-R
graphics first, continuing with our weight/age investigation of the
ballplayers.  To begin, let's do a scatter plot of weight against age,
color-coded by position.  We could type

``` r
> plot(mlb$Age,mlb$Weight,col=mlb$PosCategory)
```

but to save some typing, let's use R's **with** function (we'll change
the point size while we are at it):

``` r
> with(mlb,plot(Age,Weight,col=PosCategory,cex=0.6))
```

By writing **with**, we tell R to take Age, Weight and PosCategory in
the context of **mlb**.

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WtAgePosBase.png)

Here is how we can do it in **ggplot2**:

First, I make an empty plot, based on the data frame **mlb**:

``` r
> p <- ggplot(mlb)
```

Nothing will appear on the screen.  The package displays only when you
"print" the plot:

``` r
> p
```

This will just display an empty plot.  (Try it.)  By the way, recall
that any expression you type, even 1 + 1, will be evaluated and printed
to the screen.  Here the plot (albeit) empty is printed to the screen.

Now let's do something useful:

``` r
> p + geom_point(aes(x = Age, y = Weight, col = PosCategory),cex=0.6)
```

![alt text](https://raw.githubusercontent.com/matloff/fasteR/master/inst/images/WtAgePosGG.png)

What happened here?  Quite a bit, actually, so let's take this slowly.

* We took our existing (blank) plot, **p**, and by writing the'+' sign,
directed **ggplot2** to add to the plot **p**.  

* Now, WHAT do we want added?  We are saying, "**ggplot2**, please add
  to the plot **p** whatever **geom_point** returns."  

* Note that **geom_point** is a **ggplot2** function.  Its task is to
  produce scatter plots.

* Here are the details on the arguments to **geom_point**: 

    * We want to plot weight against height.  We do not need to specify what
      data frame these two variables are from, as we already stated that
the plot **p** is for the data frame **mlb**.  

    * We are also specifying that the color coding will be according to
      the player position, again from **mlb**.

* When R evaluates that entire expression, **p + geom_point(aes(x = Age,
  y = Weight, col = PosCategory),cex=0.6)**, the result will be another
**ggplot2** graph object. Since we typed that expression at the '>'
prompt, it was then printed to the screen as seen above.

* There is one mystery left, though:  What does the function **aes**
  ('aesthetic") do?  And why is the expression **cex=0.6** NOT an
argument to **aes**?  Unfortunately, there are no easy answers to
these questions, and in a rare exception to our rule of explaining all,
we will just have to leave this as something that must be done.

One nice thing is that we automatically got a legend printed to the
right of the graph, so we know which color corresponds to which
position.  We can do this in base-R graphics too, but need to set an
argument for it in **plot**.

## <a name="appfam"> </a> Lesson 28:  Should You Use Functional Programming?

Earlier in this tutorial, we've found R's **tapply** function to be
quite handy.  There are several others in this family, notably
**apply**, **lapply** and **sapply**.  In addition, there are other
related functions, such as **do.call** and **Reduce**.  And there are
a number of counterparts in the Tidyverse **purrr** package.
All of these go under the aegis of *functional programming* (FP).

To many, FP is intended as a higher-level replacement for loops, and
some members of the R community view that as desirable, even a must.  I
personally take a more moderate point of view, but before discussing the
controversy, let's see how FP works as a loop-replacement.

As a simple example, say we have a nonnegative integer vector **x**, and
want code that counts doubles each element that is greater than 9.
Of course, this is something we should not use a loop with in the first
place.  We should take advantage of R's vectorization capabilities:

``` r
x <- ifelse(x > 9,2*x,x)

```

But let's ignore vectorization, for the sake of illustrating the issues,
and write up a loop version:

``` r
for (i in 1:5) if (x[i] > 9) x[i] <- 2 * x[i]
```

Now, how would we replace this loop by a call to R's **sapply** function?
The latter has the call form

``` r
sapply(X,FUN)
```

where **X** is an R factor and **FUN** is a function.  We will assume
here that **FUN** returns a number, not a vector or other R object.  The
action of the function is to apply **FUN** on each element of **X**,
producing a new vector.  (It of course can be reassigned to the old
one.)

The key is defining **FUN**:

``` r
doubleIt <- function(z) if(z > 9) return(2*z) else return(z)
sapply(x,doubleIt)
```

Let's check:

``` r
> x <- c(5,12,13,8,88)
> x <- sapply(x,doubleIt)
> x
[1]   5  24  26   8 176
```

Or, we can use what is called an *anonymous* function:

``` r
> x <- c(5,12,13,8,88)
> x <- sapply(x,function(z) if(z > 9) return(2*z) else return(z))
> x
[1]   5  24  26   8 176
```

Instead of defining the function separately, we define it right there in
the second argument of **sapply**.  
 
Now let's consider something more elaborate.  Recall our earlier
baseball player example, in which we wanted to fit separate regression
lines to each of the four player position categories.  We used a loop,
which for convenience I'll duplicate here:

``` r
rownums <- split(1:nrow(mlb),mlb$PosCategory)
posNames <- c('Catcher','Infielder','Outfielder','Pitcher')
m <- data.frame()
for (pos in posNames) {
  lmo <- lm(Weight ~ Age, data = mlb[rownums[[pos]],])
  newrow <- lmo$coefficients
  m <- rbind(m,newrow)
}
```

How might we do this in FP?  We've seen the **tapply** function a couple
of times already.  Now let's turn to **lapply** ("list apply").  The
call form is

``` r
lapply(VectorOrList,FUN)
```

This first argument must be a vector or list, and the second argument
must be the name of a one-argument function.  This calls
**FUN** on each element of **VetorcOrList**, placing the
return values in a new list.

How might we use that here?  Well, **lapply**, as the name implies, is
aimed at working on lists.  Do we have any?  Why yes, **rownums** is a
list!

And indeed, we do want to take some action on each element of that list:
We want to fit a linear regression model to the rows in that element.
It is natural, then, to take for **FUN** the following function:

``` r
zlm <- function(rws) lm(Weight ~ Age, data=mlb[rws,])$coefficients
```

Here **rws** is a set of row numbers, e.g. those for the pitchers.  This
function calls **lm** on those rows, i.e. on the data **mlb[rws,]**,
then extracts the regression coefficients.

The code then is

``` r
> zlm <- function(rws) lm(Weight ~ Age, data=mlb[rws,])$coefficients
> w <- lapply(rownums,zlm)
```

The call to **lapply** then says, run **zlm** on each set of rows we see
in **rownums**, placing the coefficient vectors in an output list.
Specifically: Recall that the first element of **rownums** was
**rownums[['catcher']]**.  So, first **lapply** will make the call

``` r
zlm(rownums[['Catcher']])
```

which will fit the desired regression model on the catcher data.  Then
**lapply** will do

``` r
zlm(rownums[['Infielder']])
```

and so on.  The outputs of the four **lm** calls will be returned in an
R list, which we have assigned to **w** above.  Let's check the first
one:

``` r
> w[[1]]
(Intercept)         Age 
180.8280290   0.7949252 
``` 
jibing with **m[1,]** in our data-frame/loop appraoch above.

Well, then, what did we accomplish -- if anything -- by using **lapply**
here rather than our earlier approach using a loop?  Certainly the
**lapply** version did make for more compact code, just 2 lines.  But we
had to think a harder to come up with the idea.  Also, printing it
out is less compact:

``` r
> w
$Catcher
(Intercept)         Age 
180.8280290   0.7949252 

$Infielder
(Intercept)         Age 
170.2465739   0.8589593 

$Outfielder
(Intercept)         Age 
176.2884016   0.7883343 

$Pitcher
(Intercept)         Age 
185.5993689   0.6543904 
```

(Actually, we can use **sapply** here instead of **lapply**, with a
nicer printing.)

So, should beginning R coders use FP?  Actually, even I, with decades of
coding experience, take a moderate approach.  The criterion for
loop-based (LB) code vs.  FP should be to ask these questions:

* Would FP code be easier to write than LB in this case?

* Would FP code be easier to debug than LB in this case?

* Would FP code be easier to read -- either by others, or by myself 6
  months from now -- than LB in this case?

For the code in this tutorial in which we've used **tapply**, I believe
the answers to the above questions are definitely Yes.  But for the
**lapply** example above, I would say the answer is No -- *especially
for beginning coders*, but even for myself.  

Beginners are in the process of learning functions.  FP by definition is
based on writing functions, thus making FP a more abstract and difficult
process.  And I certainly disagree with the doctrinnaire view of some
that one should never write loops.

My recommendation is to take things on a case-by-case basis.

Now, let's turn to another central function in the **apply** family.
Not surprisingly, it's named **apply**!  It is usually used on
**matrix** objects (like data frames, but with the contents being all of
the same type, e.g. all numerical), on either rows or columnṡ, but can
be used on data frames too.

The call form is

``` r
apply(d,rc,g)
```

Here R will apply the function **g** to each row (**rc** = 1) or column
(**rc** = 2) of the data **d**.  If the function **g** returns a number,
then **apply** will return a vector.

Let's find the max values for the variables in the **pima** data:

``` r
> apply(pima,2,max)
 pregnant   glucose diastolic   triceps   insulin       bmi  diabetes
age 
    17.00    199.00    122.00     99.00    846.00     67.10      2.42
81.00 
     test 
     1.00 
```

Note that to use the  **apply** family, you can either use a built-in R
function, e.g. **max** here, or one you write yourself, such as **zlm**
above.

The R **apply** family includes other functions as well,  They are quite
useful, but don't use them solely for the sake of avoiding writing a loop.
More compact code may not be easier.

## <a name="txt"> </a> Lesson 29:  Simple Text Processing, I

These days, text processing is big in the Data Science field, e.g. in
Natural Language Processing applications.  In this lesson, we'll do a
simple yet practical example, in order to illustrate some key functions
in base-R.  (R has many packages for advanced text work, such as **tm**.)

Our example will cover reading in a file of text, and compiling a word
count, i.e. calculating the number of times each word appears.  This
kind of task is at the core of many text classification algorithms.

The file is
[here](https://raw.githubusercontent.com/matloff/fasteR/master/data/aboutR.txt).
It's basically the About section of the [R Project home
page](https://www.r-project.org/).  Here are the first few lines:

```

What is R?

Introduction to R

   R is a language and environment for statistical computing and graphics.
```

Now, how can we read the file?  For instance, **read.table** won't work,
as it expects the same number of nonblank fields on each line.  As you
can see above, our file has a variable number of such fields per line.

Instead, we read the lines of the file via a function named, not
surprisingly, **readLines**:

``` r
> abt <- readLines('https://raw.githubusercontent.com/matloff/fasteR/master/data/aboutR.txt')
```

So, what exactly is in **abt** now?  Let's turn to our usual inspection
tool, **str**.

``` r
> str(abt)
 chr [1:70] "" "What is R?" "" "Introduction to R" "" ...
```

So, **abt** is a vector of 70 elements, of type character.  Each element
of this vector is one line from the file:

```
> head(abt)
[1] ""                                                                          
[2] "What is R?"                                                                
[3] ""                                                                          
[4] "Introduction to R"                                                         
[5] ""                                                                          
[6] "   R is a language and environment for statistical computing and graphics."
```

The first line in the file was empty, so **abt[1]** is "", and so on.

Recall, our goal here is to tabulate the various words in the file.  We
won't be tabulating each individual line, so let's just make one long
line out of **abt**.

The main R function for concatening strings is **paste**.  For
instance, 

``` r
> paste('abc','987')
[1] "abc 987"
```

It can also be applied on an element-by-element basis in a vector, but
as noted, we want to create one long vector.  The **collapse** argument
does that for us:

``` r
abt1 <- paste(abt,collapse=' ') 

```

This says, "Take all the 70 strings in **abt**, and collapse them into one
big string, with a single space separating each of the original
strings."  So, it joined the elements of **abt** into one long string,
**abt1**, with successive elements of **abt** being separated by a
blank (in addition to whatever blanks were in the original strings).

``` r
> str(abt1)
 chr " What is R?  Introduction to R     R is a language and environment for statistical computing and graphics.    I"| __truncated__
```

So, **abt1** is now a single character string.  We can inspect parts of
it with the **substr** function,, e.g.

``` r
> substr(abt1,288,336)
[1] "nd colleagues. R can be considered as a    differ"
```

tells us the 288th through 336th characters in **abt1**.  How many
characters are in **abt1** in all?

``` r
> nchar(abt1)
[1] 3461
```

We now need to break **abt1** down into individual words.  We can do so using
**strsplit**:

``` r
> y <- strsplit(abt1,' ')
> str(y)
List of 1
```

That second argument, ' ', means we want the blank character to be our
splitting delimiter.  In some other setting, we may wish to use, say, a
comma as the splitting delimiter, or whatever.

Now let's look at **y**.  Keeping in mind that that object is an R list, 
we can use double brackets to inspect the first element of **y** (which
is the *only* element of **y**, as we saw above that **y** is a "list of
1").

``` r
> str(y[[1]])
 chr [1:722] "" "What" "is" "R?" "" "Introduction" "to" "R" "" "" "" "" "R" ..
```

So, **y[[1]]** is a character vector of length 722.  There is one
element for each word in the original text, though some of the "words"
are actually empty.  We see here that the first word in the text,
**y[[1]][1]**, was empty, the second word, **y[[1]][2]**, was 'What',
the third was 'is' and so on.

> 📘 **ALWAYS KEEP IN MIND**
>  
> When one gets to this level of R (or for that matter, *any* language)
, it is crucial to pay close attention
> to the class and size of all R objects. 
> 
> Here we have:
>
> * **abt** is a character vector of length 70 (70 lines in the text)
> * **abt1** is a character vector of length 1 (entire text in 1 long string)
> * **y** is an R list of length 1
> * **y[[1]]** is a character vector of length 722 (722 words in text)
> * **y[[1]][1]**, **y[[1]][2]** etc. are strings (1st word, 2nd word...)
>
> Subtle differences between object types can make big
> differences in actions.  
>
> *Dealing with this is not rocket science, just something that
> requires patience.*  You the reader should take some time at this point to
> ensure that you understand the above accounting for the various
> variables.

Now, why does the R list **y** have length only 1?  The answer is that
only string was fed into **strsplit**.  Recall what we did:

``` r
> y <- strsplit(abt1,' ')

```

If **abt1** had consisted of, say, 5 strings rather than just 1, **y**
would have been an R list of 5 elements.


At some places in the original input, we had several consecutive blanks.
When there is more than one consecutive blank, the **strsplit** function
treats the excess blanks as "words."  (This comes as quite a surprise to
Python programmers.)

So, how to get rid of the blank "words"?

``` r
> y1 <- y[[1]]  # easier to read, less cluttered
> allWords <- y1[y1 != '']  # != means "not equal to"
> allWords
> allWords
  [1] "What"                      "is"
  [3] "R?"                        "Introduction"
  [5] "to"                        "R"
...
```

The expression 

``` r
y1[y1 != '']
```

may look a little mysterious, but actually it works in the same way as
we've seen before in extracting subsets of vectors, data frames and so
on:

1. As noted, **!=** means not equal, so **!= ''** means "not an empty word."
   (Warning: This will cause some double negatives below.  Again, just
   be patient (the supreme trait of any programmer).

2. Remember, each element of **y1** is a "word," 722 of them.  We saw
   above that the first word is '', i.e. an empty string, the 
   second is "What" and so on.  The expression **y1 != ''** produces 
   722 TRUEs and FALSEs, the first one being FALSE (no, the first word
   was not nonempty), the second one being TRUE (yes, the second word was 
   nonempty), etc.

3. As we saw before, a vector (**y1** here) evaluated
   at indices taking on TRUE and FALSE values will retain the 
   vector elements corresponding to the TRUEs.  In other words, the
   expression **y1[y1 != '']** consists of the nonempty words.

So, **allWords** is just what we need---the original file contents broken down
into individual words, with no empty words.

A couple of other points:

* '!' means "not" in R, e.g.

``` r
> 3 < 8
[1] TRUE
> !(3 < 8)
[1] FALSE
```

* Material following '#' is a `comment`, a note the programmer inserts
to explain the code, for clarity and future maintainability, to
aid him/herself and/or others who read the code.  (In many cases,
comments are here to benefit you, the reader.)

We'll continue with this example in the next lesson, but first, time for
a **Your Turn** session.

> ❄️  Your Turn
>
> Write code to determine which line in 
> **abt** is longest, in terms of the number of characters.

## <a name="txt1"> </a> Lesson 30:  Simple Text Processing, II

Now, let's complete our goal of producing a word count for the original
text, i.e. which words appeared in the text and how many times did each
one appear?

As usual, it is a must to inspect the result, say the first 25 elements:

``` r
> head(allWords,25)
 [1] "What"         "is"           "R?"          
 [4] "Introduction" "to"           "R"           
 [7] "R"            "is"           "a"           
[10] "language"     "and"          "environment" 
[13] "for"          "statistical"  "computing"   
[16] "and"          "graphics."    "It"          
[19] "is"           "a"            "GNU"         
[22] "project"      "which"        "is"          
[25] "similar"     
```

Good, all the words seem to be there, and the "" are NOT there, just as
desired.  But how to get the word counts?  Why, it's our old friend,
**tapply**!

``` r
> q <- tapply(allWords,allWords,length)
> head(q,25)
            ;            …) “environment”      (easily)     (formerly 
            1             1             1             1             1 
   (including       (linear             *             ©             a 
            1             1             5             1            13 
        about     accretion     activity.           add    additional 
            3             1             1             1             1 
     Advanced   algorithmic        allows            an      analysis 
            1             1             1             5             2 
    analysis,           and           are        around       arrays, 
            2            27             4             1             1 
```

We got rid of the blank words, but the report here is still a little
rough, for example treating ';' as a "word."  But overall, it's doing
what we want, showing for instance that the word "analysis" occurs 2
times in the original text.

Now, how did this call to **tapply** work here?  Actually, this is
really the same pattern we saw with **tapply** before, with the
**length** function as our third argument.  It may look a little odd
that the first two arguments are identical, but it makes sense:

1.  The first argument says we want to split up the **allWords** vector into 
    piles. 

2.  The second argument says we want the *definition* of the piles to
    also be based on **allWords**.  In other words, we want a separate
    pile for each distinct word.

3.  Each entity that we are informally calling a "pile" above is an R
    vector:

``` r
    > str(allWords)
   chr [1:515] "What" "is" "R?" "Introduction" "to" "R" "R" "is" "a" ...
```

Applying the **length** function to each vector gives us the count
in each pile, exactly what we needed.


> 📘 Pro Tip
>
> In coding, certain patterns do arise often, such as the
> **tapply(x,x,length)** trick we saw here.  In fact,
> there are even coding books with "design patterns" in their titles.
> Take note when you see the same pattern a lot, as it may come in handy.

We're not fully done yet.  For instance, we have a punctuation problem,
where periods, commas and so on are considered parts of words, such as
the period in **allWords[17]** seen above, 'graphics.'  We also probably
should change capital letters to lower case, so that 'What' and 'what'
are not counted as two different words.

For major usage, we should consider using one of the advanced R packages
in text processing.  For instance, the **tm** package has a
**removePunctuation** function.  But let's see how we can do this with
the basics.

We'll use R's **gsub** function.  Its call form, as we'll use it, is

``` r
gsub(string_to_change,replacement,input_vector,fixed=TRUE)
```

E.g.

``` r
> a <- c('abc','de.')
> gsub('.','',a,fixed=TRUE)  # replace '.' by empty string
[1] "abc" "de" 
```

(The **fixed** argument is complex, and pops up in all the R string
manipulation packages.  This again is something you should use for now,
and look into when you become more skilled at R.)

So, to remove all periods in **allWords**, we can do:

``` r
> awNoPers <- gsub('.','',allWords,fixed=TRUE) 
> awNoPers[17]  # check that it worked
[1] "graphics"
```

We could continue to fine-tune the output in this manner.

## <a name="linreg2"> </a> Lesson 31:  Linear Regression Analysis, II

Continuing our look at linear regression analysis using R, let's look at
the famous [bike sharing
data](ttps://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset).
(See the latter site for the documentation; e.g. temperature has been
scaled, rather than measured in degrees.)
It's in a **.zip** file, so it will need a little extra preprocessing:

``` r
# fetch from Web, and store the downloaded data to the file 'bike.sip'
> download.file('https://archive.ics.uci.edu/ml/machine-learning-databases/00275/Bike-Sharing-Dataset.zip','bike.zip')
> unzip('bike.zip')  # out come the files 'day.csv' and 'hour.csv'
> day <- read.csv('day.csv',header=TRUE)
> head(day)  # always take a look around!
  instant     dteday season yr mnth holiday weekday workingday weathersit
1       1 2011-01-01      1  0    1       0       6          0          2
2       2 2011-01-02      1  0    1       0       0          0          2
3       3 2011-01-03      1  0    1       0       1          1          1
4       4 2011-01-04      1  0    1       0       2          1          1
5       5 2011-01-05      1  0    1       0       3          1          1
6       6 2011-01-06      1  0    1       0       4          1          1
      temp    atemp      hum windspeed casual registered  cnt
1 0.344167 0.363625 0.805833 0.1604460    331        654  985
2 0.363478 0.353739 0.696087 0.2485390    131        670  801
3 0.196364 0.189405 0.437273 0.2483090    120       1229 1349
4 0.200000 0.212122 0.590435 0.1602960    108       1454 1562
5 0.226957 0.229270 0.436957 0.1869000     82       1518 1600
6 0.204348 0.233209 0.518261 0.0895652     88       1518 1606
```

By the way, the weather variables have been rescaled to the interval
[0,1].  A value of 0.28, for instance, means 28% of the way from the
minimum to the maximum value of this variable.

One new concept here is the presence of *indicator* variables, more
informally known as *dummy variables*.  These are variables taking only
the values 0 and 1, with a 1 "indicating" that some trait is present.
For instance, the **holiday** variable is either 1 or 0, depending on
whether that day was a holiday (which might affect the demand for bikes
that day).

Those who manage this bike sharing service may wish to predict future
demand for bikes, say the next day, to aid in their planning.  As an
example, let's try to predict the number of casual riders from some
weather variables and the dummy variable **workingday**.

``` r
> day1 <- day[,c(8,10,12:14)]
> head(day1)
  workingday     temp      hum windspeed casual
1          0 0.344167 0.805833 0.1604460    331
2          0 0.363478 0.696087 0.2485390    131
3          1 0.196364 0.437273 0.2483090    120
4          1 0.200000 0.590435 0.1602960    108
5          1 0.226957 0.436957 0.1869000     82
6          1 0.204348 0.518261 0.0895652     88
> lmout <- lm(casual ~ .,data=day1)
> lmout
...
Coefficients:
(Intercept)   workingday         temp          hum    windspeed  
     1063.6       -806.6       2149.5       -812.7      -1145.3  
 
```

The expression "casual ~ ." means, "regress **casual** against all the
other variables in this dataset.

These numbers make sense.  The negative coefficient for **workingday**
says that, all else equal, there tend to be fewer casual riders on a
work day. 

By the way, we probably should expect fewer riders on very
cold or very hot days, so we may wish to add a quadratic term to the
model, say by doing

``` r
day1$temp2 <- temp^2  # the caret symbol means exponentiation, 
                      # i.e. 2nd power here
```

This would add the indicated column to **day1**.  But we will not pursue
this for now.

One of the very important features of R is *generic functions*.  These
are functions that take on different roles for objects of different
classes.  One such example is the **plot** function we saw earlier.

Try typing "plot(lmout)" at the R prompt.  You will be shown several
plots desribing the fitted regression model.  What happened was that the
function **plot** is just a placeholder.  When we type "plot(lmout)" R
says, "Hmm, what kind of object is **lmout**?  Oh, it's of class
**'lm'**.  So I'm going to transfer (*dispatch*) this call to one
involving a special plot function for that class, **plot.lm**."  This is
in contrast to our previous calls to **plot**, which were invoked on
vectors; those calls were dispatched to **plot.default**.

Another generic function is **summary**:

``` r
> summary(Nile)
   Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
  456.0   798.5   893.5   919.4  1032.5  1370.0 
> summary(lmout)
...
Coefficients:
            Estimate Std. Error t value Pr(>|t|)    
(Intercept)  1063.55     101.37  10.492  < 2e-16 ***
workingday   -806.63      33.41 -24.143  < 2e-16 ***
temp         2149.52      86.32  24.901  < 2e-16 ***
hum          -812.74     112.98  -7.194 1.57e-12 ***
windspeed   -1145.31     208.55  -5.492 5.51e-08 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
...
```

In the first case, the call to **summary**, invoked on a vector, was
dispatched to **summary.default**, while in the second the transfer was
to **summary.lm**.  In both cases, whoever it was in the R development
team who wrote these functions decided what summary information should
be printed out automatically.

Again, the purpose of this tutorial is to present R, not statistics.
The interested reader should consult a statistics book regarding
*p-values* and *confidence intervals.*  The former are show in the last
column of the above summary.  An approximate 95% confidence interval
for, say, the population coefficient of humidity is -812.74 plus or
minus 1.96 times the *standard error*, 112.98.  Note carefully that
p-values have long been considered to be poor methodology; see 
the [ASA statement](https://amstat.tandfonline.com/doi/full/10.1080/00031305.2016.1154108).

Another important generic function is **predict**.  Say we want to
predict **casual** for a work day in which **temp**, **hum** and
**windspeed** are 0.26, 0.55, 0.18, respectively.

``` r
> newCase <- data.frame(workingday=1, temp=0.26, hum=0.55, windspeed=0.18)
> predict(lmout,newCase)
       1 
162.6296 
```

The **predict** function, which here is **predict.lm**, assumes that the
new cases to be predicted are supplied as a data frame, with the same
column names as with the original data.

## <a name="dates"> </a> Lesson 32:  Work with the R Date Class

In the bike sharing data, dates were included, in **day$dteday**.  As
noted, some of those were holidays, indicated in the **holiday** column.
Let's see how many holidays there were:

``` r
> hds <- day$dteday[day$holiday == 1]
> hds
 [1] 2011-01-17 2011-02-21 2011-04-15 2011-05-30 2011-07-04 2011-09-05
 [7] 2011-10-10 2011-11-11 2011-11-24 2011-12-26 2012-01-02 2012-01-16
[13] 2012-02-20 2012-04-16 2012-05-28 2012-07-04 2012-09-03 2012-10-08
[19] 2012-11-12 2012-11-22 2012-12-25
```

Once again, let's review how the above code works.  The expression "[day$holiday == 1]" yields a bunch of TRUEs and FALSEs.  Using them as indices in the vecotr **day$dteday** gives us exactly the dates that are holidays. 

We see above that there were 21 holidays during the time period of the
data.  But we can do more.  First, what kind of object is **hds** above?

``` r
> class(hds)
[1] "factor"
```

Fine, but R has a special class for date data, not surprisingly called
**'Date'**.  Let's convert to that class:

``` r
> hd <- as.Date(hds)
> class(hd)
[1] "Date"
> hd
 [1] "2011-01-17" "2011-02-21" "2011-04-15" "2011-05-30" "2011-07-04"
 [6] "2011-09-05" "2011-10-10" "2011-11-11" "2011-11-24" "2011-12-26"
[11] "2012-01-02" "2012-01-16" "2012-02-20" "2012-04-16" "2012-05-28"
[16] "2012-07-04" "2012-09-03" "2012-10-08" "2012-11-12" "2012-11-22"
[21] "2012-12-25"
```

Though it prints out just as before, there are extra properties now, and
even bettery, in POSIX form:

``` r
> hp <- as.POSIXlt(hd)
> hp
 [1] "2011-01-17 UTC" "2011-02-21 UTC" "2011-04-15 UTC" "2011-05-30 UTC"
 [5] "2011-07-04 UTC" "2011-09-05 UTC" "2011-10-10 UTC" "2011-11-11 UTC"
 [9] "2011-11-24 UTC" "2011-12-26 UTC" "2012-01-02 UTC" "2012-01-16 UTC"
[13] "2012-02-20 UTC" "2012-04-16 UTC" "2012-05-28 UTC" "2012-07-04 UTC"
[17] "2012-09-03 UTC" "2012-10-08 UTC" "2012-11-12 UTC" "2012-11-22 UTC"
[21] "2012-12-25 UTC"
> hp[16]$wday  # what day of the week was July 4, 2012?
[1] 3
# ah, Wednesday (code 3)
```

(The UTC parts are the times of day, which we had not supplied.)

There are many operations that can be done on R dates.  The above is
just a little sample.

## <a name="style"> </a> Lesson 33:  Tips on R Coding Style and Strategy

Programming is a creative activity, and thus different programmers will
have different coding styles.  Some people feel so strongly that they
will publish there own particular style guides, such as 
[this one](https://google.github.io/styleguide/Rguide.xml) 
by the R community at Google.  Mine is
[here`](https://github.com/matloff/R-Style-Guide).

Needless to say, style is a matter of personal taste.  But:

**Style IS important for any code you intend to use again, for two reasons:**

1. You will quickly forget how your code works.

2.  If you share your code with others, you need to make its workings
    clear to them.

**Equally important is strategy, the way you approach a coding project.**

There is no magic formula on how to write code.  As noted earlier, I
cannot *teach* yow how to code.  I can only show you how the
ingredients work -- loops, variables, functions, if/else etc. -- and you
must creatively put them together into code that achieves goals.  It's
like solving a big puzzle, and like many big puzzles, you may need to
ponder the problem for quite a while, gaining insights here and there
until it's finally done.  Yet, as with coding style, there are strategies
that we all agree on.

So in spite of great individual variation, there are common aspects that
everyone agrees with, which we'll discuss in this lesson.

**Comment your code:**

In any programming course for Computer Science students, this
is absolutely central.  If a student turns in a programming assignment
with few or no comments, it will get a failing grade.  If comments are
needed for clarity and readability for CS students, who are presumably
strong programmers, then R users who are not expert programmers need
comments even more.

A [style
guide](https://www.cs.utah.edu/~germain/PPS/Topics/commenting.html)
at a top university computer science department puts it well:

> Commenting involves placing Human Readable Descriptions inside of
> computer programs detailing what the Code is doing. Proper use of
> commenting can make code maintenance much easier, as well as helping
> make finding bugs faster. Further, commenting is very important when
> writing functions that other people will use. Remember, well
> documented code is as important as correctly working code.

(Also see specific tips on commenting, later in that document.)

*Don't be under the illusion that your code is self-documenting; it
  isn't!  A typical comment might look like this:*

``` r
w <- f(w)
# at this point, the data frame w will consist of the original rows for
# people over age 65 and who are homeowners
```

*At the top of each source file, insert comments giving the reader an
overview of the contents.*

This will typically an overview of the roles of each major function, how
the functions interact with each other, what the main data structures
are, and so on.

I strongly recommend that you write these comments at the top of a file
BEFORE you start coding (and of course modifying it as you do write
code).  This will really help you focus during the coding process.

**Indent your code:**

``` r
if (x < y) {
   x <- y^2
   z <- x + y
}
```

is much easier to read than

``` r
if (x < y) {
x <- y^2
z <- x + y
}
```

**Write your code in top-down fashion:**

If you have a function **f** that is more than, say, a dozen lines long,
break its code into calls to smaller functions, say **g** and **h**.
Then **f** will consist of those calls, plus some "glue" lines to deal
with the return values and so on.  Of course, it's a matter of taste as
to break things up that way, but the point is that it makes your code
both easier to *read* (by others, or by yourself later), and even more
important, easier to *write*.  Breaking up the code like this makes it
read like an outline.

**Don't skimp on attending to the "corner cases":**

Computer Science people talk about "corner cases," meaning special
situations in which code may fail in spite of being generally sound.

For instance, consider this code:

``` r
> i <- 5
> 1:i
[1] 1 2 3 4 5
```

But what about the special case in which **i = 0**?

``` r
> i <- 0
> 1:i
[1] 1 0
```

This may not be what you wanted.  You probably should insert a check,
say

``` r
if (i >= 1) i:5
```

and maybe also code to handle the erroneous case.  This will depend on
the situation, but the main point is to be aware of possible corner
cases.

**Use a debugging tool:**

More on this in a later lesson!

## <a name="logit"> </a> Lesson 34: The Logistic Model

In our earlier examples of regression analysis, we were predicting a
continuous variable such as human weight.  But what if we wish to
predict a *dichotomous* varible, i.e. one recording which of two
outcomes occurs?

Consider the Pima dataset from earlier examples.  Say we are predicting
whether someone has -- or will later develop -- diabetes.  This is coded
in the **test** column of the dataset, 1 for having the disease, 0 for
not.

As a simple example, say we try to predict **test** from the variables
**bim** and **age**.  A linear model would be

mean test = &beta;<sub>0</sub> + &beta;<sub>1</sub> bmi + &beta;<sub>2</sub> age

Remember, **test** takes on the values 1 and 0.  What happens when we
take the average of a bunch of 1s and 0s?  The answer is that we get the
proportion of 1s.  For instance, the mean of the numbers 1,0,1,1 is 3/4,
which is exactly the proportion of 1s in that data.

In statististical terms, what the above equation is doing is expressing
the probability of a 1 -- i.e. the probability of having diabetes --
in terms of Body Mass Index and age.

Not a bad model, but one troubling point is that the right-hand side
could evaluate to a number less than 0 or greater than 1, which would be
impossible for a probability.  In order to deal with that problem, we
might use a *logistic* model, as follows.

Define the logistic function to be 

l(t) = 1 / (1 + e<sup>-t</sup>)

We then modify the above equation to

probability of diabetes = l(&beta;<sub>0</sub> + &beta;<sub>1</sub> bmi + &beta;<sub>2</sub> age)

As before, the statistical details are beyond the scope of this
R tutorial, but here is how you estimate the coefficients
&beta;<sub>i</sub> using R:

``` r
> glout <- glm(test ~ bmi + age, data=pima, family=binomial)
> summary(glout)
...
Coefficients:
            Estimate Std. Error z value Pr(>|z|)    
(Intercept) -5.40378    0.51530 -10.487  < 2e-16 ***
bmi          0.09825    0.01248   7.874 3.45e-15 ***
age          0.04561    0.00694   6.571 4.98e-11 ***
...
```

Let's explore those estimated &beta;<sub>i</sub> a bit.  Consider 
women with about average BMI, say 32, and compare 30-year-olds to those
of age 40.  

``` r
> l <- function(t) 1 / (1 + exp(-t))
> l(-5.40378 + 32*0.09825 + 30*0.04561)
[1] 0.2908045
> l(-5.40378 + 32*0.09825 + 40*0.04561)
[1] 0.3928424
```

So, the risk of diabetes increases substantial over that 10-year period,
but this population and BMI level.

## <a name="fd"> </a> Lesson 35:  Files and Folders/Directories

Note:  On Unix-family systems such as Linux, the Windows term *folder*
is said to be a *directory*.  You will frequently see this in Mac
discussions as well.  (The Mac OS is a Unix-family system.)  We will
typically use the term *directory* here, as that is what R uses.

In assembling a dataset for my **regtools** package, I needed to collect
the records of several of my course offerings.  I started in a directory
that had one subdirectory for each offering.  In turn, there was a file
named **Results**.  As an intermediate step, wanted to find all such
files, placing the text for each one in an R list **gFiles**.  Only some
specific columns of each file will be retained.  (The discussion here is
a slightly adapted version.)

The chief R functions I used were:

* **list.dirs:**  Returns a character vector with the names of all the
  directories (i.e. subdirectories) within the current directory.

* **dir:**  Returns a character vector with the names of all files
  within the current directory.

* **%in%:**  Determines whether a specified object is an element in a
  specified vector. 

* **setwd:**  Changes to the specified directory.

Here is the code:

``` r
getData <- function() {

   currDir <- getwd()  # leave a trail of bread crumbs

   dirs <- list.dirs(recursive=FALSE)
   numCourseOfferings <- 0
   # create empty R list, into which we'll store our course records
   resultsFiles <- list()
   for (d in dirs) {
      setwd(d)  # descend into d directory
      # check if there is a Results file there
      fls <- dir()
      if (!('Results' %in% fls)) {  # not there, skip this dir
         setwd(currDir)
         next
      }
      # ah, there is such a file; increment our count
      numCourseOfferings <- numCourseOfferings + 1
      # open it
      resultsLines <- readLines('Results')
      # delete the comment lines; look at 1st character in each line
      resultsLines <- delComments(resultsLines)
      resultsFiles[[numCourseOfferings]] <- extractCols(resultsLines)
      setwd(currDir)
   }
   resultsFiles  # return all the grades records
}
```

Before we go into the details, note the following:

* The code is written in a top-down manner.  Much of the work of
**getData** is offloaded to other functions (code not shown),
**delComments** and **extractCols**.

* There are lots of comments!

Now, consider the line

``` r
   dirs <- list.dirs(recursive=FALSE)
```

As mentioned, **list.dirs** will determine all the subdirectories
within the current directory.  But what about subdirectories of
subdirectories, and subdirectories of subdirectories of subdirectories,
and so on?  Setting **recursive** to FALSE means we want only
first-level subdirectories.

So, the line

``` r
   for (d in dirs) {
```

will then have us process each (first-level) directory, one by one.

When we enter one of those subdirectories, the line

``` r
      fls <- dir()
```

will determine all the files there, storing the result as a character
vector **fls**.

Then, as the comment notes, the lines

``` r
      if (!('Results' %in% fls)) {  # not there, skip this dir
         setwd(currDir)
         next
      }
```

will, in the event that there is no **Results** file in this
subdirectory, skip this subdirectory.  The R keyword **next** says, "Go
to the next iteration of this loop," which here means to process the
next subdirectory.  Note that to prepare for that, we need to move back
to the original directory:

``` r
         setwd(currDir)
```

On the other hand, if this subdirectory *does* contain a file named
**Results**, the remaining code increments our count of such files,
reads in the found file, and assigns its contents as a new element of
our **resultsFiles** list.

## <a name="whl"> </a> Lesson 36:  R 'while' Loops

We've seen R **for** loops in previous lessons, but there's another kind
of loop, **while**.  It keeps iterating until some specified condition
is met.  We don't know how many iterations will be needed, unlike the
**for** case, with a fixed number of iterations.

As our example, consider r's built-in dataset **AirPassengers**, which
consists of number of air travelers in thousands, in monthly data from
January 1949.  As usual, let's glance at it first:

``` r
> airpass <- AirPassengers  # less typing below
> str(airpass)
 Time-Series [1:144] from 1949 to 1961: 112 118 132 129 121 135 148 148 136 119 ...
```

Suppose we wish to know when the cumulative number of passengers first
exceeded 10 million.  A crude way would be to use R's **cumsum**
("cumulative sums") function:

``` r
> cumsum(airpass)
  [1]   112   230   362   491   612   747   895  1043  1179  1298  1402  1520
 [13]  1635  1761  1902  2037  2162  2311  2481  2651  2809  2942  3056  3196
 [25]  3341  3491  3669  3832  4004  4182  4381  4580  4764  4926  5072  5238
 [37]  5409  5589  5782  5963  6146  6364  6594  6836  7045  7236  7408  7602
 [49]  7798  7994  8230  8465  8694  8937  9201  9473  9710  9921 10101 10302
 [61] 10506 10694 10929 11156 11390 11654 11956 12249 12508 12737 12940 13169
 [73] 13411 13644 13911 14180 14450 14765 15129 15476 15788 16062 16299 16577
 [85] 16861 17138 17455 17768 18086 18460 18873 19278 19633 19939 20210 20516
 [97] 20831 21132 21488 21836 22191 22613 23078 23545 23949 24296 24601 24937
[109] 25277 25595 25957 26305 26668 27103 27594 28099 28503 28862 29172 29509
[121] 29869 30211 30617 31013 31433 31905 32453 33012 33475 33882 34244 34649
[133] 35066 35457 35876 36337 36809 37344 37966 38572 39080 39541 39931 40363
```

We see that that occurred in the 60th month.  But though this approach
would be convenient, it also would be wasteful:  We are calculating *all*
the cumulative sums, even though we don't need them all.  In a really
long vector, this could be slow.  Here is a less wasteful way:

``` r
tot <- 0
i <- 1
while (i <= length(airpass) && tot < 10000) {  ## && means 'and'
    i <- i + 1
    tot <- tot + airpass[i]
}
i  # prints 60
```

So, the **while** loop keeps iterating until we get the desired
cumulative total.

Key points here:

* The **<=** operator means "less than or equal to."  There is also
  **>=** for "greater than or equal to."

* The **&&** operator stands for "and".  It is slightly different from 
  the **&** operator, which involves vector operands.

* The condition within the 'while' says that (a) we are not yet at the
  end of the **airpass** vector, AND (b) our total is still less than 10000.

* Note the need for the condition **i <= length(airpass)**.  It's
  possible that **tot** will never exceed 10000 (not true here, but we
wouldn't know that *a priori*), so we need that condition so that the
loop doesn't iterate forever!

There's more, though.  The **cumsum** function is vectorized, so using
it, though seemingly wasteful, may actually be faster than the loop

## <a name="forMore"> </a> To Learn More 

These are books and other resources that I myself consult a lot (yes, I
do consult my own books; can't keep it all in my head :-) ), plus others
I recommend.

**Nonprogramming Coverage of R**

* Andrie de Vries and Joris Meys, *R For Dummies* (second edition), For
  Dummies

* Jaren Lander,  *R for Everyone: Advanced Analytics and Graphics*
  (second ed.), Addison-Wesley

**R Programming and Language**

* John Chambers, *Software for Data Analysis: Programming with R*, Springer

* Dirk Eddelbuettel, *Seamless R and C++ Integration with Rcpp*,
  Springer

* Colin Gillespie and Robin Lovelace, *Efficient R Programming: A
  Practical Guide to Smarter Programming*

* Norm Matloff, *The Art of R Programming*, NSP

* Norm Matloff, *Parallel Computation for Data Science*, CRC

* Hadley Wickham, *Advanced R* (second edition), CRC

**Data Science with R**

* Nina Zumel and John Mount, *Practical Data Science with R*, Manning
  (2nd ed.)

* Hadley Wickham and Garrett Grolemund, *R for Data Science: Import,
Tidy, Transform, Visualize, and Model Data*, O'Reilly

**Graphics in R**

* Winston Chang, *R Graphics Cookbook: Practical Recipes for Visualizing Data*, O'Reilly

* Paul Murrell, *R Graphics* (third edition), CRC

* Deepayan Sarkar, *Lattice: Multivariate Data Visualization with R*,
Springer

* Hadley Wickham, *ggplot2: Elegant Graphics for Data Analysis*, Springer

**Regression Analysis and Machine Learning, Using R**

* Francis Chollet and JJ Allaire, *Deep Learning in R*, Manning

* Julian Faraway, *Linear Models with R*, CRC

* Julian Faraway, *Extending the Linear Model with R*, CRC

* John Fox and Sanford Weisberg, *An R Companion to Applied Regression*,
SAGE

* Frank Harrell, *Regression Modeling Strategies: With Applications to
Linear Models, Logistic and Ordinal Regression, and Survival Analysis*,
Springer 

*  Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani,
*Introduction to Statistical Learning: with Applications in R*, 
Springer, 2nd ed. 

* Max Kuhn, *Applied Predictive Modeling*, Springer

* Max Kuhn and Kjell Johnson, Feature Engineering and Selection: *A
Practical Approach for Predictive Models*, CRC

* Norm Matloff, *Statistical Regression and Classification: from Linear
Models to Machine Learning*, CRC

* Norm Matloff, *The Art of Machine Learning: Algorithms+Data+R*, NSP,
  coming January 2024

**Other**

* Rob Hyndman and George Athanasopoulos, *Forecasting: Principles and Practice*,
OTexts 

* Ted Kwartler, *Text Mining in Practice with R*

* Norm Matloff, *Probability and Statistics for Data Science: Math + R +
Data*, CRC

* Julia Silge and David Robinson, *Text Mining with R: A Tidy Approach*,
O'Reilly

* Yihui Xie *et al*, *R Markdown: The Definitive Guide*, CRC 

**Web**

I also would recommend various Web tutorials:

* Szilard Palka, 
[CEU Business Analytics program: Use Case Seminar 2 with Szilard Pafka (2019- 05-08)](https://t.co/kbhw44Tbbn) 

* Hadley Wickham, 
[the Tidyverse](https://www.tidyverse.org) 

## <a name="thanks"> Thanks </a>

author is grateful to Kyle Butts for some format improvements in July
2022.

This tutorial has also benefited from feedback from (in alphabetical order)
Clay Ford, Reese Goding, Ira Sharenow, and Aaron Wichman, as well as
numerous anonymous suggestions.

## <a name="ide"> Installing and Using IDEs </a>

An *interactive development environment* (IDE) is a software tool that
enables editing, saving and running your code, as well as related
actions such as installing packages.

The real "power users" tend to use either Emacs Speaks Statistics (ESS),
a plugin for the Emacs editor, or Nvim-r,, a plugin for the vim editor.
However, since this tutorial is aimed at those with little or no prior
coding background, we will not cover them.  Instead, we introduce 
RStudio.  Here are some pros and cons:

* RStudio is very highly popular, especially in the US and Australia/New
  Zealand.  Indeed, for many users, RStudio *is* R.  

* Lots of help available on the Web, and in R User Groups that have been
  established in many major cities.  Has numerous features, keyboard
shortcuts etc.  

* That however also has a downside, since as noted earlier, the
  compexity of RStudio can be "overwhelming."

In light of that last point, we recommend that you NOT try to learn
RStudio to any degree of complexity at the outset.  Just learn how to
create, load, run, and save files of R code, the simple stuff, which
should be easy.  Leave the advanced features for later.

### Installation

There are many tutorials on the Web for installing RStudio.   
[This one](https://techvidvan.com/tutorials/install-r/) is pretty good, 
for all major platforms.

### Startup

If your screen has an RStudio icon, click it.  Otherwise type 'rstudio'
into a terminal window.

### Basic actions:

Again, there is a lot more one can do than the following, but we'll
stick to the absolute basics.

Note the pane in the lower-left portion of the RStudio screen.  By
default, that is the Console pane, containing the usual R '>' prompt.
You can use it just as we have throughout this tutorial.  Note too that
this is where your R output will appear.

Everything here involves files, where we store our R code (*scripts*).

**creating a new code file:**  File | New File | R Script will create an
empty window pane, ready to be filled with code.  Start typing!

**saving a code file:** File | Save will save the contents of the pane.
If it's a new file, you'll be asked to give the file a name.  Make sure
to note what folder the file will be in, so you know where to read it
from later.

**running code:** To run the code in your current window, choose Code |
Run Region | Run All.

**exiting RStudio:**

File | Quit Session...


## LICENSING

The document is covered by a 
[Creative Commons](http://creativecommons.org/licenses/by-nd/3.0/us/) license,
Creative Commons Attribution-No Derivative Works 3.0 United States 
![alt text](http://i.creativecommons.org/l/by-nd/3.0/us/88x31.png).  I have
written the document to be *used*, so readers, teachers and so on are
very welcome and encouraged to copy it verbatim.  Copyright is retained
by N. Matloff in all non-U.S. jurisdictions, but permission to use these
materials in teaching is still granted, provided the authorship and
licensing information here is displayed.  I would appreciate being
notified if you use this book for teaching, just so that I know the
materials are being put to use, but this is not required.  information
displayed.  No warranties are given or implied for this material.

