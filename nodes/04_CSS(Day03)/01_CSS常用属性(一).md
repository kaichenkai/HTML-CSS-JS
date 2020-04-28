## CSS 常用属性(一)

### css 的分类

1. css 有N多属性, 根据继承性, 主要可以分为 2 大类



### 可继承属性

1. 父标签的属性值会传递给子标签

   一般是文字控制属性, 例如: color, text-align, font-size 等



### 不可继承属性

1. 父标签的属性值不能传递给子标签

   一般是区块控制属性 



### 第一阶段需要掌握

1. visibility  

   控制标签内容

   | 值      | 描述                 |
   | ------- | -------------------- |
   | visible | 默认值, 元素时可见的 |
   | hidden  | 元素时不可见的       |

   与 display 属性相似, display: none 时, 会隐藏内容 + 空间

   

2. cursor

   规定要显示的光标的类型(形状)

   | 值          | 描述                             |
   | ----------- | -------------------------------- |
   | pointer     | 光标呈现为指示链接的指针(一只手) |
   | move        | 光标指示某对象可被移动           |
   | crosshair   | 光标呈现为十字架(绘图)           |
   | not-allowed | 禁止访问的(一个圆圈, 一条斜杠)   |

   

3. color

   

4. font

   设置文字

   | 值          | 描述                                                         |
   | ----------- | ------------------------------------------------------------ |
   | font-family | font-family:Arial, Helvetica, sans-serif                     |
   | font-size   | 设置字体大小                                                 |
   | font-weight | lighter: 细一点, normal: 常规, bold: 粗一点, bolder: 更粗一点 |
   | font-style  | 设置斜体等风格                                               |

   

5. text-decoration

   文本装饰

   | 值           | 描述                    |
   | ------------ | ----------------------- |
   | none         | **去掉 a 标签的下划线** |
   | underline    | 定义文本下的一条线      |
   | overline     | 定义文本上的一条线      |
   | line-through | 穿透文本, 删除线        |

   

6. text-indent

   设置首行缩进, 该样式需要指定一个长度, 并且只对第一行有效

   

7. text-align

   文本对齐

   左对齐, 右对齐, 居中对齐, 两边对齐

   

8. text-transform

   用于将元素中的字母转换大小写

   大写：text-transform:uppercase

   小写：text-tansform:lowercase

   首字母大写：text-transform:capitalize

   正常：text-transform:none

   

9. list-style

   设置所有列表的属性

   | 值       | 描述             |
   | -------- | ---------------- |
   | circle   | 使标题变成圆形   |
   | square   | 使标题变成正方形 |
   | ........ | **去掉标题**     |

   

10. overflow

    控制内容溢出的情况

    | 值      | 描述                          |
    | ------- | ----------------------------- |
    | visible | 默认值                        |
    | scroll  | 添加水平, 垂直滚动条          |
    | auto    | 根据内容增加滚动条 (推荐使用) |
    | hidden  | 隐藏超出盒子的内容            |

    

11. line-heigh

    设置行高, 行高越大, 则行间距越大

    行间距: (等于行高 - 字体高度) / 2    ==>  line-height 减去 font-size

    

12. box-sizing

    允许以特定的方式定义某个区域的最大宽度和高度

    | 值          | 描述                                                    |
    | ----------- | ------------------------------------------------------- |
    | content-box | 默认值, 设置盒子的外边距,边框, 内边距时, 盒子大小会扩大 |
    | border-box  | 盒子大小不变, 设置外边距等属性时, 盒子内容会缩小        |











