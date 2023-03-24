# team4-test
try to pull request

试着在dev或其他分支修改内容，并pull request



### 注意

1. 当你fork主仓库后，origin指你fork出来的仓库，upstream指主仓库

2. 不要使用upstream来更新你的本地分支，用origin更新。

    因为pull request时是根据 origin 向 upstream 提交的，基于upstream的修改从落后的origin提交，可能乱套

    使origin与upstream保持同步的方法：在github上你fork的仓库页面，在绿色的"<> code"按钮下面，点"Sync fork" - "Update branch"

3. 主仓库有master、dev、feature三个分支，当你用git clone时，仅clone了master分支

    要clone其他两个分支：

- 错误做法

    在第一次git clone后，使用``` git branch dev``` 创建dev分支，跟据本地master分支的内容创建dev（因为使用``` git branch dev``` 命令时你正处于master分支）

    会导致master特有的文件出现在dev分支

- 正确做法：（教程里也是这么做的）

    在第一次git clone后，使用``` git branch dev origin/dev``` 根据远程分支origin/dev创建dev分支

    保证本地dev分支是完全远程dev分支的复制

4. 同理3，想更新哪个分支就从远程复制哪个分支，复制到本地的名字随便，记住要往哪个分支推就行。例如，你从远程复制dev分支后，就不要pull request到feature分支。
5. 以上理解就可以，在这个仓库我对master、dev、feature分支做了明显区分，实际中dev、feature就是从main分支衍生出的，具体情况具体讨论吧。