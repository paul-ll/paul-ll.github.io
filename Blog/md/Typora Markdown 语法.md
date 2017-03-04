[TOC]



## Typora Markdown 语法

### 前言

Typora是一个功能强大的Markdown编辑器，使用GFM风格（即大名鼎鼎的github flavored markdown），Typora目前支持Mac OS和Windows，Linux版本尚未发布。Typora可以插入数学表达式，插入表情，表格，支持标准的Markdown语法，可以使用标注....，功能强悍！！！还可以导出PDF文件和HTLM文件。实时预览！！！非常牛逼！

![这里写图片描述](http://img.blog.csdn.net/20170125095650478?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 数学表达式

要启用这个功能，首先到 `Preference` -> `Editor` 中启用。然后使用 `$` 符号包裹 Tex 命令，例如： `$lim_{x \to \infty} \ exp(-x)=0$` 将产生如下的数学表达式：

![这里写图片描述](http://img.blog.csdn.net/20170125095841413?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 下标

下标使用 `~` 包裹，例如：`H~2~O`  将产生水的分子式。

### 上标

上标使用 `^` 包裹，例如：`y^2^=4` 将产生表达式

![这里写图片描述](http://img.blog.csdn.net/20170125100105796?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 插入表情

使用 `:happy:` 输入高兴的表情，使用 `:sad:` 输入悲伤的表情，使用 `:cry:` 输入哭的表情等。以此类推！

![这里写图片描述](http://img.blog.csdn.net/20170125100211070?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 下划线

用HTML的语法 `<u>Underline</u>` 将产生下划线 <u>Underline</u>.

### 删除线

GFM添加了删除文本的语法，这是标准的Markdown语法木有的。使用 `~~` 包裹的文本将会具有删除的样式，例如 
```
 ~~删除文本~~  
```
将产生  
> ~~删除文本~~ 

的样式。

### 代码

+ 使用  ` 包裹的内容将会以代码样式显示，例如
```
使用 `hello`

```
将会产生 `hello` 的样式。

+ 输入 `~~~` 或者 ``` 然后回车，可以输入代码块，并且可以选择代码的语言。例如：

```
public Class HelloWorld{
  System.out.println("Hello World!");
}
```

### 强调

使用两个 `*` 号或者两个 `_` 包裹的内容将会被强调。例如

```
 **使用两个*号强调内容**
  __使用两个下划线强调内容__
```

将会产生如下样式

 **使用两个*号强调内容**
  __使用两个下划线强调内容__

Typroa 推荐使用两个*号。

### 斜体

在标准的Markdown语法中，*和_包裹的内容会是斜体显示，但是GFM下划线一般用来分隔人名和代码变量名，因此我们推荐是用星号来包裹斜体内容。如果要显示星号，则使用转义：

```
  \*
```

### 插入图片

我们可以通过拖拉的方式，将本地文件夹中的图片或者网络上的图片插入。

![这里写图片描述](http://img.blog.csdn.net/20170125102435095?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 插入URL连接

使用尖括号包裹的url将产生一个连接，例如：`<www.baidu.com>` 将产生连接:  [www.baidu.com](www.baidu.com) .

如果是标准的url，则会自动产生连接。

### 目录列表Table of Contents（TOC）

输入 `[toc]` 然后回车，将会产生一个目录，这个目录抽取了文章的所有标题，自动更新内容。

### 水平分割线

使用 `***` 或者 `---`，然后回车，来产生水平分割线。

***

### 标注

我们可以对某一个词语进行标注。例如

```
某些人用过了才知道[^注释]
[^注释]:Somebody that I used to know.
```
将产生：

![这里写图片描述](http://img.blog.csdn.net/20170125102940413?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

把鼠标放在 `注释` 上，将会有提示内容。

### 表格
```
|姓名|性别|毕业学校|工资|
|:---|:---:|:---:|---:|
|杨洋|男|重庆交通大学|3200|
|峰哥|男|贵州大学|5000|
|坑货|女|北京大学|2000|

```
将产生:

![这里写图片描述](http://img.blog.csdn.net/20170125103221823?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 数学表达式块

输入两个美元符号，然后回车，就可以输入数学表达式块了。例如：

```
 $$\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\\end{vmatrix}$$
```

将会产生:

![这里写图片描述](http://img.blog.csdn.net/20170125103344367?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 任务列表

使用如下的代码创建任务列表，在 `[]` 中输入 `x` 表示完成，也可以通过点击选择完成或者没完成。

```
- [ ] 吃饭
- [ ] 逛街
- [ ] 看电影
- [X] 吃零食
```

将产生如下样式：

![这里写图片描述](http://img.blog.csdn.net/20170125103601562?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvdHpzXzEwNDEyMTgxMjk=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)


### 列表

输入 `+`,  `-`,  `*`, 创建无序的列表，使用任意数字开头，创建有序列表，例如：

```
**无序的列表**

* hehe
* haha
* xixi
```

**无序的列表**

* hehe
* haha
* xixi

```
**有序的列表**

1. 苹果
2. 香蕉
3. 我都喜欢
```

**有序的列表**

1. 苹果
2. 香蕉
3. 我都喜欢

### 块引用

使用 `>` 来插入块引用。例如：

```
>这是一个块引用！
```

将产生如下样式：

>这是一个块引用！


### 标题

使用#表示一级标题，##表示二级标题，以此类推，有6个标题。

