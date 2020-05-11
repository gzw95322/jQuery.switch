# jQuery.switch
Jquery 开关（esmodule版）

> **注意：**基于es6实现，目前只在webpack打包后才能正常使用。

## 调用

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
    <script src="https://cdn.bootcss.com/jquery/1.8.3/jquery.min.js"></script>
  </head>
  <body>
    <div id="switchTpl"></div>
    <script>
      $(function () {
       $("#switchTpl").switchBtn({
            data: [0, 1], // 元数据
            value: 0, // 默认值
            label: "",
            inputName: "switchTpl",
            callBack: function(val) {
                console.log(val);
            }
        });
      });
    </script>
  </body>
</html>

```



## 参数

| 参数      | 类型     | 默认值   | 注释             |
| --------- | -------- | -------- | ---------------- |
| data      | Array    | []       | 元数据           |
| value     | Array    | []       | 已选项           |
| inputName | String   | "switch" | input 名称       |
| className | String   | ""       | 附加样式         |
| callBack  | Function |          | 回调，返回已选值 |
