





- `git add .` 

会把当前目录及子孙目录里的变动都加到暂存区；





- `git add --all` 

会将项目里所有文件的变动都加到暂存区，也就是说该命令不论在项目的哪级目录执行，都有同样的效果。





- `git update-ref -d HEAD`

```
fatal: ambiguous argument 'HEAD~1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

```

会删除 HEAD 引用，这意味着 Git 将不再知道当前所在的分支，你会处于一个"分离头指针"的状态，这时 HEAD 将指向一个具体的提交而不是一个分支