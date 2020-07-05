# git命令学习

## start a working area (see also: git help tutorial)

- Clone a repository into a new directory
    > git clone repository_url
    > git clone repository_url directory
- Create an empty Git repository or reinitialize an existing one
    > git init (new_repository)
- Create your id
    > git config user.name your_name
    > git config user.email your_email
    > git config --global user.name your_name
    > git config --global user.email your_eamil

## work on the current change (see also: git help everyday)

- Add file contents to the index
    > git add file_name
- Move or rename a file, a directory, or a symlink
    > git mv file_name new_file_name
- Reset current HEAD to the specified state
    > git reset HEAD
- Remove files from the working tree and from the index
    > git rm file_name
    > 将文件只从暂存区移除 git rm --cached file_name

## examine the history and state (see also: git help revisions)

- Use binary search to find the commit that introduced a bug
    > bisect
- Print lines matching a pattern
    > grep
- Show commit logs
    > git log
    > git log --oneline
- Show various types of objects
    > show
- Show the working tree status
    > git status

## grow, mark and tweak your common history

- List, create, or delete branches
    > 创建分支 git branch branch_name
    > 列出分支 git branch
    > 删除分支 git branch -d branch_name
- Switch branches or restore working tree files
    > git checkout branch_name
- Record changes to the repository
    > git commit -m "message"
- Show changes between commits, commit and working tree, etc
    > 尚未缓存的改动 git diff
    > 查看已缓存的改动 git diff --cached
    > 查看所有改动 git diff HEAR
    > 显示简要的改动信息 git diff --stat
- Join two or more development histories together
    > git merge
- Reapply commits on top of another base tip
    > rebase
- Create, list, delete or verify a tag object signed with GPG
    > 查看所有标签 git tag
    > 创建一个标签 git tag -a v1.0

## Remote library

- Link a remote library
    > git remote add origin(short_name) remote_library_url
- List, delete a remote library
    > git remote
    > git remote -v
    > git remote rm origin(remote_library_name)

## collaborate (see also: git help workflows)

- Download objects and refs from another repository
    > git fetch
- Fetch from and integrate with another repository or a local branch
    > git pull origin
- Update remote refs along with associated objects
    > git push origin master
