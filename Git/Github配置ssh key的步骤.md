#### 生成ssh key

在客户端生成SSH key（密钥对：公钥和私钥）

```
ssh-keygen -t rsa -C "alexander_lxy@outlook.com" -b 2048
```

```
-b：指定密钥长度；
-e：读取openssh的私钥或者公钥文件；
-C：添加注释；
-f：指定用来保存密钥的文件名；
-i：读取未加密的ssh-v2兼容的私钥/公钥文件，然后在标准输出设备上显示openssh兼容的私钥/公钥；
-l：显示公钥文件的指纹数据；
-N：提供一个新密语；
-P：提供（旧）密语；
-q：静默模式；
-t：指定要创建的密钥类型，支持RSA和DSA两种认证密钥
```





#### 获取ssh key公钥内容



```
 cat ~/.ssh/id_rsa.pub
```



#### github配置

在服务端的配置文件中加入你的公钥



#### git config

```
git config --global user.email "alexander_lxy@outlook.com"
 git config --global user.name "alexander"
```



```text
git config http.sslVerify "false"
```



