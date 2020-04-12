## HTML 标签类型相互转换

### 内联标签 --> 块标签

1. 设置 css 中 display: block  -- 显示为块标签

   ```css
   span {
       background-color: green;
       display: block;
       width: 200px;
       height: 50px;
       padding: 20px;
   }
   ```



### 块标签 --> 内联标签

1. 设置 css 中 display: inline  -- 显示为内联标签

   ```css
   div {
       background-color: gold;
       display: inline;
   }
   ```



### 内联标签 --> 内联-块级标签

1. dipslay:inline-block -- 显示为内联块元素，表现为同行显示并可修改宽高内外边距等属性



### 块标签 --> 内联-块级标签

1. dipslay:inline-block -- 显示为内联块元素，表现为同行显示并可修改宽高内外边距等属性

