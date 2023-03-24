# team4-test
try to pull request

试着在dev或其他分支修改内容，并pull request



### 注意

这里主仓库有master、dev、feature三个分支，当你用git clone时，仅clone了master分支

想要clone其他两个分支，**不要在本地直接创建!!!**

- 错误做法

    在第一次git clone后，使用``` git branch dev``` 创建dev分支

    这种创建是复制了一份master分支的内容给dev，即使在创建后用```git pull```，会把

- 正确做法：

    在第一次git clone后，使用``` git branch dev origin/dev``` 根据远程分支origin/dev创建dev分支
