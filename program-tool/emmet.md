Skip to content
This repository
Search
Pull requests
Issues
Marketplace
Explore
 @tangyouhua
Sign out
33
242 141 tangyouhua/program-resource
 Code  Issues 1  Pull requests 0  Projects 0  Wiki  Insights  Settings
program-resource/program-tool/ 
Name your file…
 or cancel
 
# Emmet

<!-- toc -->
* [HTML](#HTML)
   * [孩子节点](#孩子节点)
   * [节点个数](#节点个数)
   * [上一级节点](#上一级节点)
   * [分组符号](#分组符号)
   * [ID与class](#ID与class)
   * [自定义属性](#自定义属性)
   * [列表数字](#列表数字)
   * [文本](#文本)
   * [隐式写法](#隐式写法)
   * [随机字符串](#随机字符串)
* [CSS](#CSS)
   * [浏览器特定属性](#浏览器特定属性)
   * [元素外包围代码](#元素外包围代码)
   * [为每个元素加上内容](#为每个元素加上内容)
   * [移除列表序号](#移除列表序号)
   * [引用被包围的文字](#引用被包围的文字)
   * [上一个下一个编辑位置](#上一个下一个编辑位置)
   * [上一个下一个元素](#上一个下一个元素)
   * [删除tag](#删除tag)
<!-- toc end -->

## HTML
### 孩子节点
符号 `>`

```
div>ul>li
```

### 节点个数
可以带乘号 `*`，指定节点个数

```
div>ul>li*3
```

### 邻居节点
可以带邻居节点符号 `+`

```
div+p+bq
```

### 上一级节点
上一级节点符号 `^`

```
div+div>p>span+em^bq
```

### 分组符号
 分组符号 `()`

```
div>(header>ul>li*2>a)+footer>p
(div>dl>(dt+dd)*3)+footer>p
```

### ID与class
```
div#header+div.page+div#footer.class1.class2.class3
```

### 自定义属性
自定义属性 `[]`

```
td[title="Hello world!" colspan=3]
```

### 列表数字
列表数字符号 `$`

```
ul>li.item$*5
```

多个 `$` 可以对数字进行对齐

```
ul>li.item$$$*5
```

`$@-` 表示逆序

```
ul>li.item$@-*5
```

`@N` 表示其实数字

```
ul>li.item$@3*5
```

### 文本
文本 `{text}`

```
a{Click me}
```

### 隐式写法
不写前缀，会根据上下文添加

```
.wrap>.content	div.wrap>div.content
```

### 随机字符串
```
lorem lipsum 
lorem*10 生成10个单词的随机字符
```

**注意：**空格是停止符  

## CSS
### 浏览器特定属性
生成浏览器特定属性

```
-bdrs
```

###  元素外包围代码
在元素外包围代码

```
CTRL W
```

### 为每个元素加上内容
加上 `*` 可以为每个元素加上内容

```
ul>li.nav-item$*>a
```

### 移除列表序号
`|t ` 操作符可以移除列表的序号

```
ul>li.nav>li.nav-item$*|t
```

### 引用被包围的文字
可以用 `$#` 引用被包围的文字

```
ul>li[title=$#]*>{$#}+img[alt=$#]
```

### 上一个下一个编辑位置
```
CTRL+ALT+LEFT/RIGHT 
```

### 上一个下一个元素
```
SHIFT+SUPER+,
SHIFT+SUPER+.
```

### 删除tag
```
CMD+']  
```
@tangyouhua
Commit new file

emmet.md

Add an optional extended description…
  Commit directly to the master branch.
  Create a new branch for this commit and start a pull request. Learn more about pull requests.
 
© 2018 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
API
Training
Shop
Blog
About
Press h to open a hovercard with more details.
