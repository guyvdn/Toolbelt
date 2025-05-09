# .gitconfig

path = %USERPROFILE%/.gitconfig

```ini
[user]
	name = Your Name Here
	email = Your Email Here
[alias]
	aa = add --all
	aliases = config --get-regexp alias
	branches = branch
	cm = commit -m
	configure = config --global --edit
	fm = fetch origin master:master
	fn = fetch origin main:main
	h = log --graph --all --pretty=format:'%C(auto)%d %s %C(yellow)%ad %C(cyan)<%an> %C(green)%h' --date='format-local:%Y-%m-%d %H:%M:%S'
	login = git config credential.helper store
	mm = merge master
	mn = merge main
	pushit = push --no-verify
	pushup = push -u origin HEAD
	pushitup = push -u origin HEAD --no-verify
	s = status
	uncommit = reset --soft HEAD^
	unstage = reset HEAD --
[merge]
	tool = kdiff3
[mergetool "kdiff3"]
	path = C:\\Program Files\\KDiff3/kdiff3.exe
	trustExitCode = false
[diff]
	guitool = kdiff3
[difftool "kdiff3"]
	path = C:\\Program Files\\KDiff3/kdiff3.exe
	trustExitCode = false
[core]
	editor = 'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession
[mergetool]
	keepBackup = false
```

## Worktree

- git worktree add -b emergency-fix ../temp master <!-- .element: class="fragment" -->
- fix things <!-- .element: class="fragment" -->
- git worktree remove ../temp <!-- .element: class="fragment" -->


## Other cool stuff

https://www.npmjs.com/package/git-removed-branches
