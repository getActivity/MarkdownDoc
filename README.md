# Markdown 语法文档

* 项目地址：[Github](https://github.com/getActivity/MarkdownDoc)

* 在看过很多人用 markdown 写的博客和 Github 文档后，从中我也看出了一些问题，大多人对 markdown 语法玩得不够溜，我自己曾经在这块踩过了不少的坑，于是乎我将自己在 markdown 知识和经验进行提炼和汇总，供大家学习和使用，整个文档划分为以下两部分：

    * [开车指南](#开车指南)

        * [标题的用法](#标题的用法)

        * [列表的用法](#列表的用法)

        * [引用的用法](#引用的用法)

        * [代码块的用法](#代码块的用法)

        * [斜体的用法](#斜体的用法)

        * [粗体的用法](#粗体的用法)

        * [删除线的用法](#删除线的用法)

        * [文字高亮的用法](#文字高亮的用法)

        * [图片的用法](#图片的用法)

        * [链接的用法](#链接的用法)

        * [标题锚点的用法](#标题锚点的用法)

        * [表格的用法](#标题锚点的用法)

        * [复选框的用法](#复选框的用法)

        * [分割线的用法](#分割线的用法)

        * [换行符的用法](#换行符的用法)

    * [飙车指南](#飙车指南)
      
        * [反义语法](#反义语法)

        * [修改图片的显示大小](#修改图片的显示大小)

        * [修改文字的显示重心](#修改文字的显示重心)

        * [使用的展开收缩功能](#使用的展开收缩功能)

* 开车指南介绍了常规的语法用法，精通 markdown 语法同学可以略过，飙车指南则介绍了 markdown 语法之外的一些用法，因为 markdown 本身支持的语法格式太少，往往没有办法满足我们的需求，所以需要用到 html 语法来帮我们扩展一些非常规的用法，例如修改图片显示的大小，修改文本重心、展开收缩功能等等。

* 另外大家可能好奇我为什么不用网上已有的方案，在这个开源项目之前，我其实看过很多人写的 markdown 语法介绍，但是都没能符合我的要求，普遍存在以下问题：

    1. 写得不够通俗易懂

    2. 语法介绍得不够全面

    3. 只讲语法不讲槽点坑点

    4. 语法介绍得太简单，很多重要的细节没有讲到位

    5. 只讲了 md 语法，没有讲 md 之外一些特殊用法

* 而我想做的，正是将上面这些的问题全部解决掉，做一份让每一个程序员都能看懂、学会、学精的 markdown 文档。

## 开车指南

### 标题的用法

* 使用 #（井号）表示标题，# 越多表示标题就越小，最多支持使用六个 #

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

* 接下来让我们看看具体的效果

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

### 列表的用法

使用 * 表示列表，列表下面还有列表，列表层级无限制，子列表的前面必须要有四个空格或者一个制表符，并且上一个语法必须也是列表，这样才能表示它是这个列表的子列表，另外除了 * 符号，- 符号也可以作为列表使用，但是更推荐大家使用 * 符号。

```
* 一级列表

    * 二级列表

        * 三级列表
```

接下来让我们看看具体的效果

* 一级列表

    * 二级列表

        * 三级列表

列表还分为有序列表和无序列表，上面介绍的是无序列表的用法，下面介绍有序列表的用法

```
1. 有序列表

    1. 有序子列表

    2. 有序子列表

2. 有序列表

    1. 有序子列表

    2. 有序子列表
```

用法和无序列表差不多，只不过将前面的 * 换成了具体的数字

1. 有序列表

    1. 有序子列表

    2. 有序子列表

2. 有序列表

    1. 有序子列表

    2. 有序子列表

### 引用的用法

* 使用 > 表示引用，一个 > 代表一次引用，一行可以使用多个 >，并且没有数量限制

```
> 一级引用
> > 二级引用
> > > 三级引用
```

> 一级引用
> > 二级引用
> >
> > > 三级引用

### 代码块的用法

* 使用两个 \`\`\` 将内容包裹起来，就会出现代码块的效果，具体的格式如下：

\`\`\`  
System.out.println("Markdown");  
\`\`\`

* 具体的效果如下：

```
System.out.println("Markdown");
```

* 如果需要代码高亮功能，则需要第一个 \`\`\` 符号后面加上对应的编程语言，具体的格式如下：

\`\`\`java  
System.out.println("Markdown");  
\`\`\`

* 具体的效果如下：

```java
System.out.println("Markdown");
```

### 斜体的用法

* 使用两个 * 或者 _ 包裹住某个文字，就会出现斜体的效果，具体的格式如下：

```
*我是斜体*

_我是斜体_
```

* 具体的效果如下：

*我是斜体*

_我是斜体_

### 粗体的用法

* 使用两个 ** 或者 __ 包裹住某个文字，就会出现粗体的效果，具体的格式如下：

```
**我是粗体**

__我是粗体__
```

* 具体的效果如下：

**我是粗体**

__我是粗体__

### 删除线的用法

* 使用两个 ~~ （波浪号）包裹住某个文字，就会出现删除线的效果，具体的格式如下：

```
~~删除线~~
```

* 具体的效果如下：

~~删除线~~

* 需要注意的是：这个语法某些 markdown 编辑器是不支持的

### 文字高亮的用法

* 使用两个 ` 包裹住某个文字，就会出现高亮的效果，具体的格式如下：

```
`重点文字`
```

* 具体的效果如下：

`重点文字`

### 图片的用法

* 使用 `![图片介绍](图片地址)` 的格式来表示图片，具体的格式如下：

```
![百度图片](https://www.baidu.com/img/bd_logo.png)
```

* 具体的效果如下：

![百度图片](https://www.baidu.com/img/bd_logo.png)

* 图片链接不仅支持网络的，还支持本地的，具体的格式如下：

```
![图片介绍](file/local_image.jpg)
```

* 具体的效果如下：

![图片介绍](file/local_image.jpg)

### 链接的用法

* 使用 `[链接描述](链接地址)` 的格式来表示链接，具体的格式如下：

```
[打开百度一下](https://www.baidu.com)
```

* 具体的效果如下：

[打开百度一下](https://www.baidu.com)

* 链接不仅支持网络的，还支持本地的，具体的格式如下：

```
[打开本地链接](file/local_markdown.md)
```

* 具体的效果如下：

[打开本地链接](file/local_markdown.md)

* 另外链接还可以搭配图片来做，具体的格式如下：

```
[![我是图片+链接](https://www.baidu.com/img/bd_logo.png)](https://www.baidu.com)
```

* 具体的效果如下：

[![我是图片+链接](https://www.baidu.com/img/bd_logo.png)](https://www.baidu.com)

### 表格的用法

* 表格的用法稍微有点复杂，但是还是有规律可循，具体的格式如下：

```
|      表头1    |     表头2    |     表头3   | 
|  :--------   |  :--------:  |  --------: |
|  我是表格内容  |  我是表格内容  | 我是表格内容 |
|  我是表格内容  |  我是表格内容  | 我是表格内容 |
```

* 具体的效果如下：

|      表头1    |     表头2    |     表头3   |
|  :--------   |  :--------:  |  --------: |
|  我是表格内容  |  我是表格内容  | 我是表格内容 |
|  我是表格内容  |  我是表格内容  | 我是表格内容 |

* 第一行表示表格的表头，第二行表示表格的重心，后面的行数表示表格的内容

* 这里特别讲一下表格的重心设置，一共有三种样式可供选择

    * `:---` 表示这一列左对齐

    * `---:` 表示这一列右对齐

    * `:---:` 表示这一列居中

* 简单点讲，就是根据冒号的写法来决定表格列的内容重心

### 标题锚点的用法

* 锚点的格式跟链接差不多，唯一不同的是括号里面放的不是普通链接，而是当前页面的标题引用，具体的格式如下：

```
[点击这里回到一级标题](#一级标题)
```

* 具体的效果如下：

[点击这里回到一级标题](#一级标题)

* 另外有一点需要注意，锚点中的链接，需要进行一些处理，否则会导致无法识别

    * 如果锚点中的链接中存在大写的英文，则需要手动转换成小写的英文才能被识别

    * 如果锚点中的链接中存在 ` ` （空格），则需要手动替换成 `-` （减号），如果有多个空格，则用多个减号代替

    * 如果锚点中的链接中存在某些特殊符号，如：`,`（逗号）`.`（点号）、`/` （斜杆）`\` （反斜杆）等，则需要进行删除才能进行识别

### 复选框的用法

* 使用 `* [x]` 或者 `- [x]`  代表已经选中的复选框，使用 `* []` 或者 `* []` 代表未选中的复选框，具体的格式如下：

```
* [x] 已办事例 A

* [ ] 待办事例 A

- [x] 已办事例 B

- [ ] 待办事例 B
```

* 具体的效果如下：

* [x] 已办事例 A

* [ ] 待办事例 A

- [x] 已办事例 B

- [ ] 待办事例 B

### 分割线的用法

* ***、---、___可以显示横线效果，推荐大家使用 ---，具体的格式如下：

```
***
---
___
```

* 具体的效果如下：

***
---
___

### 换行符的用法

* 在 markdown 中直接换行是没有效果的，先让我们做一下测试：

```text
我是第一行
我是第二行
```

* 具体效果如下：

我是第一行
我是第二行

* 正确换行有三种方式，在第一行后面再多加个换行符

```text
我是第一行

我是第二行
```

* 具体效果如下：

我是第一行

我是第二行

* 另外一个是在第一行后面多加两个空格

```text
我是第一行  
我是第二行
```

* 具体效果如下：

我是第一行  
我是第二行

* 还有一种方式，是使用 html 标签来换行

```text
我是第一行<br/>我是第二行
```

* 具体效果如下：

我是第一行<br/>我是第二行

## 飙车指南

### 反义语法

* 有些特殊字符因为涉及到 markdown 语法，所以被 markdown 自动识别了，如果我不想被识别成 markdown 该怎么做？其实也很简单，只需要在特殊字符前面加上一个 \ 即可，具体的格式如下：

```
\#\#\#\# 我是谁
```

* 具体效果如下：

\#\#\#\# 我是谁

### 修改图片的显示大小

* 有两种方式修改，一种是指定图片的宽高，另外一种是指定图片的缩放比例，具体的格式如下：

```xml
<img src="https://www.baidu.com/img/bd_logo.png" width="300px" height="200px" alt="图片名称" />

<img src="https://www.baidu.com/img/bd_logo.png" width="50%" height="50%" alt="图片名称" />
```

* 具体的效果如下：

<img src="https://www.baidu.com/img/bd_logo.png" width="300px" height="200px" alt="图片名称" />

<img src="https://www.baidu.com/img/bd_logo.png" width="20%" height="20%" alt="图片名称" />

### 修改文字的显示重心

* 需要用 html 标签来实现，具体的格式如下：

```
<p align="left">文字左对齐</p>

<p align="center">文字居中</p>

<p align="right">文字右对齐</p>
```

* 具体的效果如下：

<p align="left">文字左对齐</p>

<p align="center">文字居中</p>

<p align="right">文字右对齐</p>

### 使用的展开收缩功能

* 需要用 html 标签来实现，具体的格式如下：

```
<details>
<summary>更新日志（收缩状态）</summary>

* 惊不惊喜？

* 意不意外？

* 开不开心？

* 懵不懵逼？

</details>


<details open>
<summary>更新日志（展开状态）</summary>

* 惊不惊喜？

* 意不意外？

* 开不开心？

* 懵不懵逼？

</details>
```

* 具体的效果如下：

<details>
<summary>更新日志（收缩状态）</summary>

* 惊不惊喜？

* 意不意外？

* 开不开心？

* 懵不懵逼？

</details>


<details open>
<summary>更新日志（展开状态）</summary>

* 惊不惊喜？

* 意不意外？

* 开不开心？

* 懵不懵逼？

</details>

#### 作者的其他开源项目

* 安卓技术中台：[AndroidProject](https://github.com/getActivity/AndroidProject) ![](https://img.shields.io/github/stars/getActivity/AndroidProject.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidProject.svg)

* 安卓技术中台 Kt 版：[AndroidProject-Kotlin](https://github.com/getActivity/AndroidProject-Kotlin) ![](https://img.shields.io/github/stars/getActivity/AndroidProject-Kotlin.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidProject-Kotlin.svg)

* 权限框架：[XXPermissions](https://github.com/getActivity/XXPermissions) ![](https://img.shields.io/github/stars/getActivity/XXPermissions.svg) ![](https://img.shields.io/github/forks/getActivity/XXPermissions.svg)

* 吐司框架：[ToastUtils](https://github.com/getActivity/ToastUtils) ![](https://img.shields.io/github/stars/getActivity/ToastUtils.svg) ![](https://img.shields.io/github/forks/getActivity/ToastUtils.svg)

* 网络框架：[EasyHttp](https://github.com/getActivity/EasyHttp) ![](https://img.shields.io/github/stars/getActivity/EasyHttp.svg) ![](https://img.shields.io/github/forks/getActivity/EasyHttp.svg)

* 标题栏框架：[TitleBar](https://github.com/getActivity/TitleBar) ![](https://img.shields.io/github/stars/getActivity/TitleBar.svg) ![](https://img.shields.io/github/forks/getActivity/TitleBar.svg)

* 悬浮窗框架：[XToast](https://github.com/getActivity/XToast) ![](https://img.shields.io/github/stars/getActivity/XToast.svg) ![](https://img.shields.io/github/forks/getActivity/XToast.svg)

* Shape 框架：[ShapeView](https://github.com/getActivity/ShapeView) ![](https://img.shields.io/github/stars/getActivity/ShapeView.svg) ![](https://img.shields.io/github/forks/getActivity/ShapeView.svg)

* 语种切换框架：[MultiLanguages](https://github.com/getActivity/MultiLanguages) ![](https://img.shields.io/github/stars/getActivity/MultiLanguages.svg) ![](https://img.shields.io/github/forks/getActivity/MultiLanguages.svg)

* Gson 解析容错：[GsonFactory](https://github.com/getActivity/GsonFactory) ![](https://img.shields.io/github/stars/getActivity/GsonFactory.svg) ![](https://img.shields.io/github/forks/getActivity/GsonFactory.svg)

* 日志查看框架：[Logcat](https://github.com/getActivity/Logcat) ![](https://img.shields.io/github/stars/getActivity/Logcat.svg) ![](https://img.shields.io/github/forks/getActivity/Logcat.svg)

* Android 版本适配：[AndroidVersionAdapter](https://github.com/getActivity/AndroidVersionAdapter) ![](https://img.shields.io/github/stars/getActivity/AndroidVersionAdapter.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidVersionAdapter.svg)

* Android 代码规范：[AndroidCodeStandard](https://github.com/getActivity/AndroidCodeStandard) ![](https://img.shields.io/github/stars/getActivity/AndroidCodeStandard.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidCodeStandard.svg)

* Android 资源大汇总：[AndroidIndex](https://github.com/getActivity/AndroidIndex) ![](https://img.shields.io/github/stars/getActivity/AndroidIndex.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidIndex.svg)

* Android 开源排行榜：[AndroidGithubBoss](https://github.com/getActivity/AndroidGithubBoss) ![](https://img.shields.io/github/stars/getActivity/AndroidGithubBoss.svg) ![](https://img.shields.io/github/forks/getActivity/AndroidGithubBoss.svg)

* Studio 精品插件：[StudioPlugins](https://github.com/getActivity/StudioPlugins) ![](https://img.shields.io/github/stars/getActivity/StudioPlugins.svg) ![](https://img.shields.io/github/forks/getActivity/StudioPlugins.svg)

* 表情包大集合：[EmojiPackage](https://github.com/getActivity/EmojiPackage) ![](https://img.shields.io/github/stars/getActivity/EmojiPackage.svg) ![](https://img.shields.io/github/forks/getActivity/EmojiPackage.svg)

* 省市区 Json 数据：[ProvinceJson](https://github.com/getActivity/ProvinceJson) ![](https://img.shields.io/github/stars/getActivity/ProvinceJson.svg) ![](https://img.shields.io/github/forks/getActivity/ProvinceJson.svg)

#### 微信公众号：Android轮子哥

![](https://raw.githubusercontent.com/getActivity/Donate/master/picture/official_ccount.png)

#### Android 技术 Q 群：10047167

#### 如果您觉得我的开源库帮你节省了大量的开发时间，请扫描下方的二维码随意打赏，要是能打赏个 10.24 :monkey_face:就太:thumbsup:了。您的支持将鼓励我继续创作:octocat:

![](https://raw.githubusercontent.com/getActivity/Donate/master/picture/pay_ali.png) ![](https://raw.githubusercontent.com/getActivity/Donate/master/picture/pay_wechat.png)

#### [点击查看捐赠列表](https://github.com/getActivity/Donate)

## License

```text
Copyright 2023 Huang JinQun

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```