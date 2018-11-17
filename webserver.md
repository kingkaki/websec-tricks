## $_SERVER['HTTP_HOST']伪造

当传入两个host头部时

```
Host: localhost
Host: evalcode
```

- Apache

```
string(19) "localhost, evalcode"
```

- nginx  以第二个Host为基准

```
string(8) "evalcode"
```

## $_SERVER['PHP_SELF']

$_SERVER[‘PHP_SELF’] 可伪造