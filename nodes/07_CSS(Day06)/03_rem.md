## rem

### 概念

1. rem 可以在用户浏览网页时, 根据屏幕的尺寸, 来向用户展示更合适用户的布局, 文字, 图片, 按钮的像素大小
2. rem (font size of the root element) 是指相对于根元素的字体大小的单位
3. 一旦根节点 html 定义的 font-size 变化, 那么整个网页中运用到 rem 的也会随之变化



### 使用

1. 浏览器的默认字体都是 16 px, 所有未经调整的浏览器都符合 1rem = 16px, 那么 12px = 0.75rem, 10px = 0.625rem
2. 目前 PC 端开始普遍使用 rem, 移动端基本完全使用



在开发时, 一般设置根节点 html 的 font-size: 10px, 便于计算

```css
html {
    font-size: 10px;
}
```

当我们想设置盒子的 宽度 为 200px 时, 改写成 rem 的方式就是: 

font-size: 20rem



在适配于不同设备时, 只需要调整根节点 html 中的 font-size 基数即可