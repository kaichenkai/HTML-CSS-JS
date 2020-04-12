## css 样式

### 概念

1. css 指层叠样式表



### 作用

1. 它是来美化网页用的
2. HTML 代码是用来构建网页整体布局, CSS 则是用来美化网页, 两者缺一不可
3. 建房子需要用钢筋水泥 (HTML标签, 属性等) 把房子整体架构建好, 涂料之类的 (CSS 属性) 就是装饰房子的



### css 的定义方法

```css
/* 选择器{属性:值; 属性:值; 属性:值;} */

div { 
    width:100px; 
    height:100px; 
    background:gold; 
}
```



### css 的引入方式（3种）

1. 内联式

   通过标签的 style 属性，在标签上直接写样式

   ```html
   <div style="width:100px; height:100px; background: blue;">div tag</div>
   ```

2. 嵌入式

   通过 style 标签，在网页上创建嵌入的样式表

   ```html
   <style type="text/css">
           div {width:100px; height:100px; background: blue;}
           ......
   </style>
   ```

3. 外链式（推荐使用）

   通过 link 标签，链接外部样式文件到页面中

   ```html
   <link rel="stylesheet" type="text/css" href="css/main.css">
   ```

4. #### 优先级别

   当以多种方式编写 css 代码时, 到底哪种样式会被使用 ?

   ##### 内联式级别最高

   嵌入式 和 外链式, 需要看顺序, 一般外链式会写到嵌入式的前边, 即

   嵌入式  >  外链式







