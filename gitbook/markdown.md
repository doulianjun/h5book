# 使用markdown语法进行写作
## markdown简介
现代文章的编写需要有丰富的图文混合排版格式，以及便捷的交互阅读体验。我们可以用word文本编辑工具来编写，也可以用html语言来编写。但这两者都有一些缺点。word软件的排版功能很复杂，80%的word排版功能是用不上的，这使得我们的写作注意力总是被分散。html语言已经成了一种越来越专业的软件开发语言，也是变得越来越复杂，已经脱离了最初单纯的文章编写需求，越来越趋近于满足功能逻辑复杂的软件开发需要。

Markdown是一种新的文章编写语言，它专门为文章编写而生，非常直观好读、简洁易写。它的排版功能只是html的一个子集，而又脱离了html语法标记的繁琐感，通过一批精选的大众熟悉的标点符号来来表达文章的排版需求，从而使我们的创作注意力集中文章内容的本身上，免除繁琐文章排版的拖累。

下面我们来领略一下markdown的魅力。

## 块级元素
### 段落和换行
 一个自然段是由多行句子构成的，自然段之间由一个或多个空行分割。在这里“空行”的意思是“看起来像空行”，也就是说，如果行中有tab制表符、空格等，该行也会被当作空行。一个空行标识一个单一段落，相当于html中的`<p>`。
 
 句子中的回车换行如同html类似，一般情况下都将被markdown忽略。如果要强制换行，可以在句子后面加上两个空格再换行即可。连续两个空格加换行，相当于html中的`<br>` 


### 标题
markdown用 \# 来标识一个标题。用 \# 的数量来标识1~6级标题。如下所示：  

代码：

    # 一级标题  
    ## 二级标题  
    ### 三级标题  
    #### 四级标题  
    ##### 五级标题  
    ###### 六级标题  

效果：

# 一级标题  
## 二级标题  
### 三级标题  
#### 四级标题  
##### 五级标题  
###### 六级标题  
注：# 和标题文字之间建议保留一个字符的空格，这是Markdown 写法惯例。

### 列表
在 Markdown 中，只需要在文字前面加上 \- 就可以标识一个列表项，例如：  

    ### 这是无序列表
    - 列表项1  
    - 列表项2  
    - 列表项3  

效果：

### 这是无序列表
- 列表项1  
- 列表项2  
- 列表项3  

上面是无序列表，有序列表只需要将\- 更换为 1. 即可.  

    ### 这是有序列表
    1. 列表项1  
    1. 列表项2  
    1. 列表项3  

效果：
### 这是有序列表
1. 列表项1  
1. 列表项2  
1. 列表项3  

注：-、1.和文本之间要保留一个字符的空格。

### 块引用
只需要使用 > 开头即可
> 白日依山尽  
> 黄河入海流  
> 欲穷千里目  
> 更上一层楼  


### 表格

用竖线“|”表示一个表格单元格。使用 “| ------------- |:-------------:| -----:|”区分表格头部区和表格主体区。

代码：

    | Tables        | Are           | Cool  |
    | ------------- |:-------------:| -----:|
    | col 3 is      | right-aligned | $1600 |
    | col 2 is      | centered      |   $12 |
    | zebra stripes | are neat      |    $1 |

效果：

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

### 代码块
代码块用于表达源代码，只需要在行首添加4个空格或者1个tab制表符即可。这个作用相当于html的`<pre>`标签。

代码：

        <style type="text/css">
             /**
             * Example of an initial loading indicator.
             * It is recommended to keep this as minimal as possible to provide instant feedback
             * while other resources are still being loaded for the first time
             */
            html, body {
                height: 100%;
                background-color: hsl(0, 0%, 93%);
                background: url(resources/images/sjsgsl.logo.sm.png) no-repeat;
                background-position: center center;
            }
    
            #appLoadingIndicator {
                position: absolute;
                width: 0%;
                height: 0px;
            }
    
            #DetailPage .x-scroll-scroller{
                position: relative;
            }
        </style>

效果：

    <style type="text/css">
         /**
         * Example of an initial loading indicator.
         * It is recommended to keep this as minimal as possible to provide instant feedback
         * while other resources are still being loaded for the first time
         */
        html, body {
            height: 100%;
            background-color: hsl(0, 0%, 93%);
            background: url(resources/images/sjsgsl.logo.sm.png) no-repeat;
            background-position: center center;
        }
    
        #appLoadingIndicator {
            position: absolute;
            width: 0%;
            height: 0px;
        }
    
        #DetailPage .x-scroll-scroller{
            position: relative;
        }
    </style>

### 水平线

使用三个短横线“---”单独一行来表达一个水平线。

代码：

    ---
效果：

---
    
## 行内元素
 
### 超链接
使用 `[]` 表达链接文本，紧跟着 `()` 表达链接的网址。如下代码所示：  

    请访问专业的HTML5培训机构[北京乐美无限公司](http://www.nemo-tec.com/)  

效果：

请访问专业的HTML5培训机构 [北京乐美无限公司](http://www.nemo-tec.com/)  

使用 `[]` 表达链接文本，紧跟着 `()` 表达链接的网址。如下代码所示：  

    请访问专业的HTML5培训机构[北京乐美无限公司](http://www.nemo-tec.com/)  

效果：

请访问专业的HTML5培训机构 [北京乐美无限公司](http://www.nemo-tec.com/)  

使用 `[]` 表达链接文本，紧跟着 `()` 表达链接的网址。如下代码所示：  

    请访问专业的HTML5培训机构[北京乐美无限公司](http://www.nemo-tec.com/)  

效果：

请访问专业的HTML5培训机构 [北京乐美无限公司](http://www.nemo-tec.com/)  

### 强调(文字加粗和斜体效果)
一个星号`*`表示强调，对应于html语言的`<em>`标记，两个星号`**`表示强烈强调，对应于html语言的`<strong>`标记。用星号在前后包裹需要标注的文字范围。

代码：

    相信天上掉*馅饼*的人，大多会落入**陷阱**。

效果：

相信天上掉*馅饼*的人，大多会落入**陷阱**。


### 图片
语法格式为：

    ![Alt text](/path/to/img.jpg "Optional title")
以感叹号开头，后面加上中括号`[]`表示的图片配图文字，再跟上用小括号`()`表示的图片来源网址。

代码：

    乐美无限公司成立于2011年![phones](images/logo.zhuanjia.png)，专注于以HTML5为主要方向的移动互联网软件技术项目孵化和培训业务。html5技术支持跨手机平台的应用软件开发，只需要使用cordovar封装即可生成各个平台上的app。
    
效果：
    
乐美无限公司成立于2011年![phones](images/logo.zhuanjia.png)，专注于以HTML5为主要方向的移动互联网软件技术项目孵化和培训业务。html5技术支持跨手机平台的应用软件开发，只需要使用cordovar封装即可生成各个平台上的app。


也可以使用图片索引来嵌入图片：

    
    ![Alt text][id]
    
    索引声明：
    [id]: url/to/image  "Optional title attribute"

代码：

    使用图片：![logo][id008]
    [id008]: images/logo.zhuanjia.png "乐美无限LOGO 移动互联网职业教育专家"

效果：

使用图片：![logo][id008]

[id008]: images/logo.zhuanjia.png "乐美无限LOGO 移动互联网职业教育专家"


注： 目前图片不支持设置宽高。

### 行内代码片段

如果要在行内标记一小段行内程序代码，可以用反引号把它包起来(\`) , 这个作用相当于html中的`<code>` 标签

代码：

    HTML行内标签包括：`<span>`、`<cite>`、`<del>`等。

效果：

HTML行内标签包括：`<span>`、`<cite>`、`<del>`等。


## 其他

### 自动插入锚链接

代码：

    <http://www.nemo-tec.com/>

效果：

<http://www.nemo-tec.com/>





### 特殊符号需要使用反斜杠转义

    \   反斜线
    `   反引号
    *   星号
    _   底线
    {}  花括号
    []  方括号
    ()  括弧
    #   井字号
    +   加号
    -   减号
    .   英文句点
    !   惊叹号


** 注1：本文只介绍了最简单常用的markdown写法，还有其他写法，感兴趣的同学可以自行了解。**

** 注2：我本人习惯在markdown语法符号与相邻文字之间多写一个空格，这样看起来比较好看。 **

** 注3：使用图片文件时，尽量使用`png`文件格式，`bmp`文件格式尺寸太大。 **
