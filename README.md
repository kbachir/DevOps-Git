# Git Commands

### Local Changes
- `git init`: create a new local repository
- `git status`: view changes in wkdir
- `git add`: add a file to the next commit. `.` for all current changes, `<file-name>` for specific files.
- `git commit -m`: commits all changes in tracked files. `-m` to add a message.
- `git push`: to push to associated GitHub repo

### Branches
- `git branch -av`: list all existing branches
- `git checkout <branch>`: switch HEAD branch
- `git branch <new-branch>`: create a new branch based on your current HEAD
- `git branch -d <branch>`: delete a local branch

### Remotes
- `git remote -v`: list all currently configured remotes
- `git remote show <remote>`: show info about a remote
- `git remote add <shortname> <url>`: add a new remote repo
- `git fetch <remote>`: like git pull but doesn't integrate into HEAD
- `git pull <remote> <branch>`: downloads repo and merges changes into HEAD
- `git push <remote> <branch>`: publish local changes to remote repo
- `git merge <branch>`: merge a branch into current HEAD

### Resets
- `git reset --hard HEAD`: discard all local changes in your wkdir
- `git checkout HEAD <file>`: discard local changes in a specific file
- `git revert <commit>`: revert a commit by producing a new commit with contrary changes
- `git reset --hard <commit>`: reset your HEAD pointer to a previous commit **and discard all changes since**
- `git reset <commit>`: reset your HEAD pointer to prev commit **and preserve all changes as unstaged** 
- `git reset --keep <commit>`: reset your HEAD pointer to prev commit **and preserve uncommitted local changes**

### Initialising a new repo

- `git init -b main`
- `git add .`
- `git commit -m "initial commit"`
- `git remote add origin  <REMOTE_URL>`
- `git remote -v`
- `git push origin main`

### CLoning an existing repo

- `git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`
