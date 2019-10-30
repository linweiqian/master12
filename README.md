# 关于git无法将文件push到gitHub储存库中的问题
## 如果出现以下报错：
## 错误提示一:
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/linweiqian/master.git/'
## 错误提示二:
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.
## 错误提示三:
Please make sure you have the correct access rights
and the repository exists.
## 错误提示四:
fatal: unable to access 'https://github.com/linweiqian/master.git/': Failed to connect to 127.0.0.1 port 1080: Connection refused
## 错误提示五:
On branch master,nothing to commit, working tree clean
## 错误提示六:
fatal: remote origin already exists.
## 如果出现以上错误则在gitbash中输入以下命令
git config --global credential.helper store
## 然后输入
git remote add origin 你的存储库地址，git push -u origin master
## 如果第一次提交则会弹出一个登陆窗口，输入你的github账号和密码，如果不是第一次提交则直接登陆