# checkbox



```xml
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <meta http-equiv="Content-Type" content="text/html;charset=utf-8">
    <title>jQuery测试</title>
    <style type="text/css">
        .cls{
            background-color: fuchsia;
        }
    </style>
    <script type="text/javascript" src="js/jquery-1.12.3.js"></script>
    <script type="text/javascript">
        $(function () {
            $('#btnAll').click(function(){
                $(':checkbox').prop("checked",true);
            });
            $('#btnNone').click(function(){
                $(':checkbox').prop("checked",false);
            });
            $('#btnReverse').click(function(){
                $(':checkbox').each(function (k,v) {
                    $(v).prop("checked",!$(v).is(":checked"));
                });
            });
        });
    </script>
</head>
<body>
    <input type="button" id="btnAll" value="全选"/>
    <input type="button" id="btnNone" value="不选"/>
    <input type="button" id="btnReverse" value="反选"/>
    <input id="ch_swimming" type="checkbox"/><label for="ch_swimming">游泳</label>
    <input id="ch_basketball" type="checkbox"/><label for="ch_swimming">篮球</label>
    <input id="ch_football" type="checkbox"/><label for="ch_swimming">足球</label>
</body>
</html>
```

