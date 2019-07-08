$ git config --global alias.st status
$ git config --global alias.co checkout
$ git config --global alias.ci commit
$ git config --global alias.br branch


以后提交就可以简写成:
$ git ci -m "bala bala bala..."

在撤销修改一节中，我们知道，命令git reset HEAD file可以把暂存区的修改撤销掉（unstage），重新放回工作区。既然是一个unstage操作，就可以配置一个unstage别名:
$ git config --global alias.unstage 'reset HEAD'

配置一个git last，让其显示最后一次提交信息：

$ git config --global alias.last 'log -1'
