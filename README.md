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

7.撤销修改   工作区和暂存区的修改撤销

  工作区的修改（没有添加到暂存区 可以手动删除）
  可以使用命令：git checkout -- readme.md
    -- 一定要加上  表示你要返回修改 不然成了切换分支了


  要是工作区的修改已经提交到了暂存区  （并没有提交到到版本库）
  那就先
    1. git reset HEAD 文件名称   撤销暂存区的文件
    2. git checkout -- 文件名称 撤销修改工作区的文件

8.删除文件
  git rm




远程库的文件

1. 把本地文件要推送到远程库里

   先建立
   git remote add origin git@github.com:michaelliao/learngit.git
   
   添加后，远程库的名字就是origin，这是Git默认的叫法，也可以改成别的，但是origin这个名字一看就知道是远程库。

    下一步，就可以把本地库的所有内容推送到远程库上：

    	$ git push -u origin master



