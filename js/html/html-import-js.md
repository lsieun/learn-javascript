# HTML页面引入javascript文件

失败的方式： 这样会导致文件显示不正确。

```html
<script type="text/javascript" src="jquery-3.3.1.js"/>
```

正确的方式：

```html
<script type="text/javascript" src="jquery-3.3.1.js"></script>

<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>

<script type="text/javascript">
   $(function(){
      alert("My First Jquery Test");
   });
</script>
```
