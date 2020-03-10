## 目录
[toc]
## 基本style样式
- 样式位置
    - 内联样式
    - 内部样式
    - 外部文件（利用link标签来引入）
```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>css</title>
    <style type="text/css">
        p {
            color: red;
            font-size: 40px;
        }
    </style>
</head>

<body>
    <!-- <p style="color:red;font-size: 40px;">style的内联标签显示样式</p> -->
    <p>通过整体来更改样式</p>
    <p>通过整体来更改样式</p>
</body>

</html>
```
link样式
```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>css</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
    <!-- <p style="color:red;font-size: 40px;">style的内联标签显示样式</p> -->
    <p>通过整体来更改样式</p>
    <p>通过整体来更改样式</p>
</body>

</html>
```
## 基本语法
- 选择器
- 声明块儿
- 选择器
    - id选择器
    - class选择器
    - 选择器分组（并集选择器）-----钥匙的共同特征
        - *{}表示选择所有元素
    - 复合选择器（交集选择器）-----融合成特制的钥匙
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>css选择器</title>
    <style>
        #p1 {
            color: sienna;
            font-size: 40px;
        }

        .p2 {
            font-size: 20px;
        }

        .hello {
            font-size: 30px;
        }

        .p2,
        .p3 {
            color: slateblue;
        }
    </style>
</head>

<body>
    <p id="p1">古诗标题</p>
    <p class="p2 hello">正文正文正文正文</p>
    <p class="p2">正文正文正文正文</p>
    <p class="p2">正文正文正文正文</p>
    <p class="p2">正文正文正文正文</p>
    <p class="p3">并集选择器测试</p>
    <p class="p3">并集选择器测试</p>
    <p class="p3">并集选择器测试</p>
</body>

</html>
```