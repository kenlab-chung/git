# git
## Gitlab Community Edition 镜像使用帮助
地址：https://mirror.tuna.tsinghua.edu.cn/help/gitlab-ce/
注意: gitlab-ce 镜像仅支持 x86-64 架构

### Debian/Ubuntu 用户
首先信任 GitLab 的 GPG 公钥:

curl https://packages.gitlab.com/gpg.key 2> /dev/null | sudo apt-key add - &>/dev/null
再选择你的 Debian/Ubuntu 版本，文本框中内容写进 /etc/apt/sources.list.d/gitlab-ce.list

你的Debian/Ubuntu版本: 
debian 8:
deb http://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/debian jessie main 
debian 9:
deb http://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/debian stretch main
debian 10:
deb http://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/debian buster main
debian 14:
deb https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/ubuntu trusty main
debian 16:
deb https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/ubuntu xenial main
debian 18:
deb https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/ubuntu bionic main
安装 gitlab-ce:

sudo apt-get update
sudo apt-get install gitlab-ce

### RHEL/CentOS 用户
新建 /etc/yum.repos.d/gitlab-ce.repo，内容为

[gitlab-ce]
name=Gitlab CE Repository
baseurl=https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/yum/el$releasever/
gpgcheck=0
enabled=1
再执行

sudo yum makecache
sudo yum install gitlab-ce
