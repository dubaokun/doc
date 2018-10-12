# git的区间
    - 工作区
    - 暂存区

# 撤销修改
> 修改分为两种情况，以下详细介绍这两种情况；
## 在工作区修改但没有add到暂存区
> git checkout -- <file>

## 在工作区修改了也add到暂存区    
    - git reset HEAD <file> 先撤销暂存区的修改
    - git checkout -- <file> 再撤销工作区的修改


# 撤销删除
## 如果之前add到暂存区，可以直接
    - git checkout -- <file>

## 不过如果是昨天删的，那就只能
    - git reset --hard <id>>
    

# git查看某个文件的修改历史
    - git log --pretty=oneline 文件名
    - git show 356f6def9d3fb7f3b9032ff5aa4b9110d4cca87e
    - git blame file
