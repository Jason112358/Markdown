# 表格
表格的格式为用|分隔各单元格内容，用---分隔表头与内容。例如：  
| 学号 | 姓名 | 成绩 |
| --- | --- | --- |
|211|Hector|100|
|212|Jason|59|
|225|Star|99|
## 对齐方式  
这里很形象地用:和-的组合来表示，将:视作表格的框架，将-视作表格内容即可方便记忆。例如：
|学号 | 姓名 | 成绩 |
|:---|:---:|---:|
|这一列靠左对齐|这一列居中对齐|这一列靠右对齐|
|211|Hector|100|
|212|Jason|59|
|225|Star|99|
还是很直观嗷

# 小结
Markdown的基础语法还是非常简单的，如果有HTML的基础应该会更加简单，在高级技巧中除了一些小细节的使用，也引入了大量的HTML的语法和标签，下面介绍Markdown的高级技巧。

# 高级技巧
## 支持哪些HTML元素呢？
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。  
目前支持的 HTML 元素有：<kbd>\<kbd> \<b> \<i> \<em> \<sup> \<sub> \<br></kbd>等 ，例如：
> 使用<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd>打开任务管理器。

**这里在VSCode的两种Preview模式下有不同的显示格式，Markdown Preview Enhanced显示格式更多，VSCode自带Preview显示格式较少**  

## 转义
Markdown转义与大部分语言转义相同都使用\来实现，例如：↑五行以前的标签的表示。

## 公式
Markdown中公式的插入需要使用$$符号来前后包裹LaTeX或Tex公式。例如：  

$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$

* 注意$$要与之前的语句隔一行，避免之前\$\$符号的影响。
* 在这里Markdown Previewer Enhanced又比VSCode自带的Previewer牝一点，支持公式的显示。多写几个例子：

$$a+b$$
$$x_1$$
$$x_1^3$$
$$x_{(22)}^{33}$$
$$x_{sth}^{sth}$$

这是简单的公式引入，还有更加复杂的公式需要在学习LaTeX等相关知识后综合应用。

***
Markdown基础学习就到这里，参考链接：[RUNOOB Markdown教程](https://www.runoob.com/markdown/md-tutorial.html)