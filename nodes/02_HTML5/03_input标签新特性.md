## input 新用法

### fieldset

<!--将表单内容的一部分打包, 生成一组相关表单的字段-->
<!--<legend></legend>标签为 fieldset 元素定义标题-->

```html
<fieldset>
    <legend>用户登录</legend>
    <label>用户名: <input type="text"></label><br/>
    <label>密码: <input type="password"></label>
</fieldset>
```



### 新增的 type 属性

1. color

   ```html
   <label>选择颜色<input type="color"></label>
   ```

2. email

   校验用户输入内容是否符合邮箱格式

   ```html
   <label>请输入邮箱 <input type="email"></label>
   ```

3. number

   校验用户输入内容是否为数字

   ```html
   <label>请输入数字 <input type="number"></label>
   ```

4. url

   校验是否为 url

   ```html
   <label>请输入url <input type="url"></label>
   ```

5. search

   ```html
   <label>请输入搜索内容 <input type="search"></label>
   ```

6. range

   ```html
   <label>范围 <input type="range"></label>
   ```

7. date

   ```html
   <label>选择日期 <input type="date"></label>
   ```

   日期标签

8. datetime
   日期时间标签

   ```html
   <label>选择日期时间 <input type="datetime-local"></label>
   ```

9. time

   时间标签

   ```html
   <label>选择时间 <input type="time"></label>
   ```

10. month

    月标签

    ```html
    <label>选择月份 <input type="month"></label>
    ```

11. week

    周标签

    ```html
    <label>选择周 <input type="week"></label>
    ```

    











