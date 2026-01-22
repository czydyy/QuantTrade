# QuantTrade
## 开发环境说明

### 使用 vscode 远程开发

+ 安装插件 Remote SSH
+ 连接到主机
+ 可以选择配置文件配置，配置文件中内容如下：

```
Host aliyun-web
    HostName 8.140.239.234
    User root
    IdentityFile C:\Users\chenzeyu\.ssh\id_rsa
Host local-vm
    HostName 192.168.138.130
    User root
    IdentityFile C:\Users\chenzeyu\.ssh\id_rsa
```


配置IdentityFile 可以免密登录，没有id_rsa这个文件，可以用如下命令生成：

```
ssh-keygen -t rsa -b 4096
```

复制**C://user/zychen/.ssh/id_rsa.pub** 中的内容到阿里云云服务器上 **/root/.ssh/authorized_keys**  文件中

### 使用git做代码同步

## 代码规范 和 命名规则
代码规范和命名规则，都参考《google cpp style guide》