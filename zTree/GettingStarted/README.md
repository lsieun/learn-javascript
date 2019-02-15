# zTree

## Quick Start

引入zTree的js和css：

```html
<link rel="stylesheet" href="/css/zTreeStyle/zTreeStyle.css"/>
<script type="text/javascript" src="/js/jquery.ztree.all.js"></script>
```

页面使用

```html
<ul id="treeDemo" class="ztree"></ul>

<script type="text/javascript">
    var setting = {};

    var zNodes = [];

    $(document).ready(function(){
        $.fn.zTree.init($("#treeDemo"), setting, zNodes);
    });
</script>
```
