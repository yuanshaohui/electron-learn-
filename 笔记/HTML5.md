## 目录
[toc]
## 简单实例
```html
<!doctype html>
<html>

<head>
    <meta charset="utf-8" />
    <title>标题</title>
</head>

<body>
    <!--这是一段标记内容-->
    <h1>这是页面内容</h1>
    <h1>这是<font color="red" size="7">红色</font></h1>
    <p>锄禾日当午，<br />汗滴禾下土，<br />谁知盘中餐，<br />粒粒皆辛苦。<!--br是换行的自结束标签--></p>
    <p>a&lt;b&gt;c<br />空&nbsp;格<br />&copy;版权所有特殊符号<!--运用实体，显示不能被打出的符号--></p>
</body>

</html>
```
## 图片标签
| 图片格式  | 特点                             | 应用                   |
| --------- | -------------------------------- | ---------------------- |
| jpeg(jpg) | 色彩颜色丰富，可压缩，不支持透明 | 用来保存颜色丰富的图片 |
| gif       | 颜色少，动态图，简单透明         | 颜色单一的动态图       |
| png       | 支持的颜色多，支持复杂透明       | 显示复杂透明的图片     |
```html
<!doctype html>
<html>
<!doctype html>
<html>

<head>
    <meta charset="tuf-8">
    <title>图片标签</title>
</head>

<body>
    <!-- 
        使用img标签从外部引入图片
        src:引用文件地址(相对地址)，"/../1.0.jpg"表示返回几级上层目录
        alt:对图片进行描述
        width:修改文件的宽度
        height:修改文件的高度

    -->
    <img src="1.0.jpg" alt="这是一辆跑车" width="600px" />
</body>

</html>
```
## meta标签
```html
<!doctype html>
<html>

<head>
    <meta charset="utf-8" />
    <meta name="keywords" content="html5,python,javascript" />
    <!-- 关键词 -->
    <meta name="description" content="这是对网页的描述">
    <!-- 网页描述的一句话 -->
    <meta http-equiv="refresh" content="5;url=http://www.baidu.com" />
    <!-- 用来跳转 -->
    <title>关于meta标签的使用</title>
</head>

<body>
    <h1>内容</h1>
</body>

</html>
```
## html的语法规范
1. html中不区分大小写
2. 注释不接受嵌套
3. html标签必须结构完整(浏览器最大限度的补全)、
4. 标签可以嵌套，但是不能交叉嵌套
5. 属性必须有值，且必加引号 
## 内联框架
```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8" />
    <title>内联框架</title>
</head>

<body>
    <p>内联框架</p>
    <!-- 
        src:
        width:
        height:
        name:
     -->
    <iframe src="图片标签.html" frameborder="0" name="内联框架的名字"></iframe>
</body>

</html>
```
## 超链接
- href：超链接的地址(若为#，可回到顶部)
    - target:打开方式
        - _self  默认值
        - _blank 在新的窗口中打开
        - 内联框架的名字 可在内联框架中打开
 ```html
 <!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8" />
    <title>超链接</title>
</head>

<body>
    <!--
        href：超链接的地址
        target:打开方式
            _self  默认值
            _blank 在新的窗口中打开
            内联框架的名字 可在内联框架中打开
    -->
    <a href="图片标签.html">这是本地的超链接地址</a>
    <a href="http:www.baidu.com">这是百度的超链接地址</a>
    <a href="1.0.jpg" target="图片">在内联框架中打开本地超链接</a>
    <iframe src="图片标签.html" name="图片" frameborder="0"></iframe>
</body>

</html>
 ```
## 块儿标签和内联元素
- div独占一行，无任何额外属性
- span内联元素，行内元素
    - a
    - img
    - iframe
    - span
- p元素不可以包含任何元素
- div可以包含spand元素，反之不行
- a元素可以包含除他本身的任何元素