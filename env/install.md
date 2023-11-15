## 问题1: Could not resolve host: raw.githubusercontent.com
第一步：通过网站https://www.ipaddress.com/查找raw.githubusercontent.com的ip地址

第二步：ping id地址看能不能通

第三步：sudo vi /etc/hosts 然后搜索到ip地址映射添加到最后一行，比如：199.232.68.133 raw.githubusercontent.com 保存退出，重新安装即可

第四步：安装nvm: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

```js
vim ~/.bashrc 
// 安装zsh的
vim ~/.zshrc 
```

```js
// 添加
########### nvm #############
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
########### nvm #############
```
```js
source ~/.bashrc 
// 安装zsh的
source ~/.zshrc 
```

第五步：安装homebrew: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"



## 问题2：Mac 生成 SSH 密钥
第一步：cd ~/.ssh  

第二步：ssh-keygen -t rsa -C “你的邮箱”

第三步：ssh-add ~/.ssh/id_rsa

第四步： cat ~/.ssh/id_rsa.pub 

第五步：拷贝内容至github
