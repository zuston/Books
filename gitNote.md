### Git-------note

> git的三个分区（工作区->缓存区->分支区）
> 
> 1. git init
> 2. git add a.php（将工作区的文件添加到缓存区去跟踪）
> 3. git commit -m “add the a.php”（将缓冲区的文件提交到分支）
> 
> ------
> 
> 上述为一些git提交基础

------

- 远程库克隆（先有远程库，然后在本地clone远程库）
  
  git clone [url]
  
- 本地仓库连接远程关联github仓库（本地已经先有仓库，将远程关联）
  
  1. git remote add origin [url]（关联远程仓库）
  2. git pull origin master（将远程仓库内容pull到本地的origin）
  3. git push -u origin master（将本地的仓库origin推送到master分支
  
- git分支创建
  
  1. git branch（查看分支）
  2. git branch dev（创建dev分支）
  3. git checkout dev（将分支转换到dev）
  4. git checkout -b dev（是2，3两步的结合，创建dev分支和转换到dev）
  5. git merge master（将master分支合并到当前分支）
  6. git branch -d master（删除master分支）
  
- git删除文件
  
  1. git rm demo.php
  
- git状态查看
  
  1. git status
  
- git版本回退
  
  1. git log（查看git提交记录）
  2. git log —pretty==oneline
  3. git reset —hard HEAD^
  4. git reset —hard 343434

[^​created by Zuston]: this is the git note