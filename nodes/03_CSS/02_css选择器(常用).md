## css 选择器 (常用)

### 什么是选择器?

1. 选择指定的标签设置样式



### 通用选择器 (权重:0)

1. 对所有标签都有效

   ```css
   * {
       color: blue;
   }
   ```



### 标签选择器 (权重:1)

1. 对指定的标签有效

   ```css
   div {
       color: purple;
   }
   ```

   

### 类选择器 (权重:10)

1. 对同一类名(class)有效, 同一个标签可能有多个类

   ```css
   .className {
       color: pink;
   }
   ```



### id 选择器 (权重:100)

1. 对标有特定 id 属性的标签有效

   ```css
   #idName {
       color: yellow;
   }
   ```



### 群组选择器 (权重: 不叠加)

1. 它也可以与标签选择器结合使用

2. 可以同时使用多个选择器, 多个选择器将被同时应用指定的样式

   ```css
   div, p, .className1, .className2 {
       background-color: skyblue;
   }
   ```



### 复合选择器 (权重: 叠加)

1. 可以同时使用多个选择器, 这样可以同时满足多个选择器的元素

2. div.box1 会选中页面中 div 标签内具有 class="box1" 的元素

   ```css
   div.box1 {  /*没有空格*/ 
       background-color: skyblue;
   }
   ```



### 后代选择器 (权重: 叠加)

1. 主要应用在**标签嵌套**的结构中，它可与标签选择器结合使用，减少命名，同时也可以通过层级，限制样式的作用范围

2. 对 div 标签内的 class="className1" 的**所有子标签**有效

   ```css
   div .className1 { /*有空格*/
       background-color: skyblue;
   }
   ```

 

### 直接后代选择器 (权重: 叠加)

1. 对 div 标签内的 class="className1" 的**直接子标签**有效

   ```css
   div > .className1 { /*有空格*/
       background-color: skyblue;
   }
   ```

   



