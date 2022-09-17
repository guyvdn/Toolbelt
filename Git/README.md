# .gitconfig

path = %USERPROFILE%/.gitconfig

```ini
[user]
	name = Your Name Here
	email = Your Email Here
[alias]
	s = status
	aa = add --all
	h = log --graph --all --pretty=format:'%C(auto)%d %s %C(yellow)%ad %C(cyan)<%an> %C(green)%h' --date='format-local:%Y-%m-%d %H:%M:%S'
	fm = fetch origin master:master
	fn = fetch origin main:main
	mm = merge master
	branches = branch
	unstage = reset HEAD --
	pushit = push --no-verify
	pushup = push -u origin HEAD
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

## Other cool stuff

https://www.npmjs.com/package/git-removed-branches