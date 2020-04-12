## css 选择器(某些场景使用)

### 兄弟选择器 (权重叠加)

1. 除了父子关系, 还可以根据兄弟关系查找元素

2. 对后边的一个兄弟元素有效

   ```css
   div + p {
       background-color: skyblue;
   }
   ```

3. 对后边的所有兄弟元素有效

   ```css
   div ~ p {
       background-color: skyblue;
   }
   ```

4. 查找前边的一个兄弟元素

5. 查找前边的所有兄弟元素



### 属性选择器 (权重叠加)

1. 对有指定属性的标签有效

   ```css
   div[id] {
       background-color: yellowgreen;
   }
   ...
   <div id="div1">这是一个div1标签</div>
   ```

2. 对有指定的属性和属性值的标签有效

   ```css
   div[name=div3] {
       background-color: purple;
   }
   ...
   <div name="div3">这是一个div3标签</div>
   ```

3. 对有多属性和多属性值的标签有效

   ```css
   div[id][name=div4] {
       background-color: purple;
   }
   ...
   <div id="div3" name="div3">这是一个div3标签</div>
   <div id="div4" name="div4">这是一个div4标签</div>
   ```



### 伪类选择器和伪元素

使用场景: 有时候, 需要选择本身没有标签, 但是仍然易于识别的网页部位, 比如段落首行, 鼠标悬停, 鼠标进入等等

1. #### 伪类

   | 语法         | 描述                             | css版本 | 是否常用 |
   | ------------ | -------------------------------- | ------- | -------- |
   | :active      | 选择正在被激活的元素             | 1       |          |
   | :hover       | 选择被鼠标悬浮下的元素           | 1       | 是       |
   | :link        | 选择未被访问的元素               | 1       |          |
   | :visited     | 选择已被访问的元素               | 1       |          |
   | :first-child | 选择满足是其父元素的第一个子元素 | 2       |          |
   | :lang        | 选择带有指定 lang 属性的元素     | 2       |          |
   | :focus       | 选择拥有键盘输入焦点的元素       | 2       | 是       |
   | :enabel      | 选择每个已启动的元素             | 3       |          |
   | :disable     | 选择每个已禁止的元素             | 3       |          |
   | :checked     | 选择每个被选中的元素             | 3       |          |
   | :target      | 选择当前的锚点元素               | 3       |          |

   : hover 的使用 (复合选择器 + 伪类选择器)

   ```css
   p.test:hover {
       background-color: yellowgreen;
   }
   ...
   <p class="test">我是段落内容</p>
   ```

   :focus 的使用

   ```css
   input:focus {
       height: 50px;
       width: 300px;
   }
   ...
   <label>请输入内容:<input type="text"></label>
   ```

   

2. #### 伪元素

   | 语法           | 描述                           | css版本 | 是否常用 |
   | -------------- | ------------------------------ | ------- | -------- |
   | ::first-letter | 选择指定元素的第一个单词       | 1       | 是       |
   | ::first-line   | 选择指定元素的第一行           | 1       | 是       |
   | ::after        | 在指定元素的内容后面插入内容   | 2       | 是       |
   | ::before       | 在指定元素的内容前面插入内容   | 2       | 是       |
   | ::selection    | 选择指定元素中被用户选中的内容 | 3       |          |

   ::first-letter 和 ::firstline 的使用

   ```css
   /*改变第一个字符的样式*/
   p::first-letter {
       font-size: 50px;
   }
   /*改变第一行字符的样式*/
   p::first-line {
       background-color: skyblue;
   }
   ```



### 否定伪类

1. 可以选择不是指定标签的一些标签

2. 语法:

   ```css
   标签:not(选择器){}
   ```

3. 使用, 设置 p 标签中 class 属性值不等于 box 的背景颜色

   ```css
   p:not(.box){
       background-color: yellow;
   }
   ```

   







































 



