
## git配置用户名和邮箱：

```bash
git config --global user.name "<Your name> "
git config --global user.email "<Your email>"

#检查配置
git config --global  --list
```

## git配置ssh

```bash
ssh-keygen -t rsa -C "<Your email>"
```

然后进入`~`目录找到`.ssh`目录里的`id_rsa.pub`文件，复制全部内容到“GitHub settings”的添加ssh key。

检查是否配置成功

```bash
ssh -T git@github.com
```

