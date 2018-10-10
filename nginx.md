## $_SERVER['HTTP_HOST']伪造

当我们传入两个Host头的时候，Nginx将以第一个为准，而PHP-FPM将以第二个为准。

也就是说，如果我传入：

```
Host: 2018.mhz.pw
Host: xxx'"@example.com
```

从而产生歧义