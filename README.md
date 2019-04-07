## socket.io 实现的广播系统

## 页面应用

页面头部

```html
<head>
  <script src="/real/socket.io.js"></script>
</head>
```

页面底部：

```html
<script>
  socket = io({ path: "/real" });
  socket.on("systenMsg", arg => {
    console.log(arg);
  });
</script>
```
