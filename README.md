# ceshi
测试
LWF 首次提交

1.首先配置
  git config --global user.name 'lwf';
  git config --global user.email '309759321@qq.com'

2.配置ssh 允许访问
  生成ssh 
    ssh-keygen -t rsa -C '306975921@qq.com'
  接着按3个回车
  最后在.ssh目录下得到了两个文件 id_rsa(私有秘钥) id_rsa 公有秘钥

3.配置github上添加ssh key deploy keys

4. git clone ssh地址

版本提交
5. git add 添加到暂存区
   git commit -m '描述'  添加到版本库
   git status 查看状态


6. 回退到之前版本
   git reset --hard HEAD^ 回退上个版本
   git reset --hard commitID 版本号
   git log 查看日志  --pretty-oneline简化
   git reflog重返未来

   




