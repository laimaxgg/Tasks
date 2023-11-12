# 1.Markdown的标题语法
在单词或短语的前面添加**井号（#）+空格**可创建一个标题，标题的等级由井号（#）的数量决定。
例如：添加一个井号（#）表示创建一个一级标题，添加两个井号（#）表示创建一个二级标题。Markdown最多可创建六级标题:
|语法|效果|
|---|---|
|``# 一级标题 ``|# 一级标题 |
|``## 二级标题``|## 二级标题|
|``### 三级标题``|### 三级标题|
|...|...|
|``###### 六级标题``|###### 六级标题|

另外：Markdown还可以在文本下方添加任意数量的=号来将文本识别为一级标题，或添加任意数量的-号来将文本识别为二级标题。
# 2.Markdown的换行语法
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行。另外，Markdown还支持使用HTML的`<br>`标签换行。
# 3.Markdown的段落语法
在一行或多行文本末尾按回车键即可创建空白行并输入段落，但Markdown不支持使用空格（space）和制表符（tab）缩进段落，使用它们可能会造成某些格式错误。
# 4.Markdown的强调语法
## 粗体（blod）
请在单词或短语的前后各添加两个星号（*）或下划线（_）即可将单词或短语标记为粗体。Markdown 应用程序在如何处理单词或短语中间的下划线上并不一致。为兼容考虑，在单词或短语中间部分加粗的话，请使用星号。
|语法|效果|
|---|---|
|``I just love **bold text**. ``|I just love **bold text**.|
|``I just love __bold text__.``|## I just love __bold text__.|
|``Love**is**bold**``|Love**is**bold|
|``我喜欢使用**粗体**``|我喜欢使用**粗体**|
## 斜体（Italic）
在单词或短语前后添加一个星号（*）或下划线（_）即可用斜体显示文本。如要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不能带空格。
|语法|效果|
|---|---|
|``Italicized text is the *cat's meow*. ``|Italicized text is the *cat's meow*.|
|``Italicized text is the _cat's meow_.``|## Italicized text is the _cat's meow_.|
|``A*cat*meow``|A*cat*meow.|
|``一只猫*喵*了一声``|一只猫*喵*了一声|
## 粗体（Bold）和斜体（Italic）
如要同时用粗体和斜体突出显示文本，需在单词或短语的前后各添加三个星号或下划线。如要加粗并用斜体显示单词或短语的中间部分，需在要突出显示的部分前后各添加三个星号，中间不能带空格。
|语法|效果|
|---|---|
|``This text is ***really important***. ``|This text is ***really important***.|
|``This text is ___really important___.``|## This text is ___really important___.|
|``This text is __*really important*__.``|This text is __*really important*__.|
|``This text is **_really important_**.``|This text is **_really important_**.|
|``This is really***very***important text.``|This is really***very***important text.|
|``这个文段***非常重要***``|这个文段***非常重要***|
# 5.Markdown 引用语法
## 创建块引用
在段落前添加一个 > 符号即可创建一个块引用。
>``> Dorothy followed her through many of the beautiful rooms in her castle.``

> Dorothy followed her through many of the beautiful rooms in her castle.
## 多个段落的块引用
块引用可以包含多个段落。在段落之间的空白行添加一
个 > 符号即可将多个段落一起块引用。
>``> Dorothy followed her through many of the beautiful rooms in her castle.``
>``>``
>``> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.``

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
## 嵌套块引用
块引用可以嵌套。在要嵌套的段落前添加一个 >> 符号。
>``> Dorothy followed her through many of the beautiful rooms in her castle.``
``>``
``>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.``

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
## 带有其它元素的块引用
块引用可以包含其他 Markdown 格式的元素。
例如：粗体、斜体可在块引用中使用。
>``> #### The quarterly results look great!``
>``>``
>``> - Revenue was off the chart.``
>``> - Profits were higher than ever.``
>``>``
>``>  *Everything* is going according to **plan**.``

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
# 6.Markdown的列表语法
## 有序列表
在每个列表项前添加数字并紧跟一个英文句点即可创建有序列表。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

## 无序列表
在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+)即可创建无序列表 。缩进一个或多个列表项可创建嵌套列表。
## 在列表中嵌套其他元素
要在保留列表连续性的同时在列表中添加另一种元素，需将该元素缩进四个空格或一个制表符。
## 7.Markdown的代码语法
要将单词或短语表示为代码，请将其包裹在反引号 (`) 中。
|语法|效果|
|---|---|
|``At the command prompt, type `nano`. ``|At the command prompt, type `nano`.|

如果要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(``)中。
|语法|效果|
|---|---|
|` ``Use `code` in your Markdown file.`` ``|``Use `code` in your Markdown file.``|
## 8.Markdown的分隔线语法
要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。另外为了兼容性，需在分隔线的前后均添加空白行。
## 9.Markdown的链接语法
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

>这是一个链接 [Markdown语法](https://markdown.com.cn)
>``这是一个链接 [Markdown语法](https://markdown.com.cn)。``