# linux opreation

- 在当前目录下查找指定名称的字符串

``` find /path/ -name "filename" ```

- 当前目录搜索文件内容含有某字符的文件

``` find /path f | xargs grep "file content"  ```

- 查找指定类型文件含有某字符串

``` find /path f -name "*.sh" | xargs grep -i "file content" ```

- mysql 修改指定账户密码
``` sql
    # login as root user
    use mysql;
    UPDATE user set authentication_string = Password("new password") WHERE user="root";
    flush privileges;

```

- 链接操作
```sh
    ln -s /path/to/root /path/to/destination
```

- 新建用户操作
```sh
    useradd username
    passwd username
    # adduser 更加方便
```

- 添加用户到sudo组
```sh
    usermod -a -G sudo username
```


- 让新建用户共享linux补齐效果
```sh
    usermod -s /bin/bash username
```

- 查看端口占用
```sh
    lsof -i:port
```




