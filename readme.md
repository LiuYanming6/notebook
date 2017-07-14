
1. 设置本地github环境
将公钥放到github上
ssh-keygen
cat ~/.ssh/id_rsa.pub

测试是否成功
ssh -T git@github.com

git config --global user.name 'onovps'  # 需要吗

2. 下载项目并修改上传
git clone http://github.com/mingruyue/l2cm_libuci.git
git add Makefile-src
git commit -m "add local src Makefile"
git push

3. 创建新的项目仓库
…or create a new repository on the command line

echo "# notebook" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/mingruyue/notebook.git
git push -u origin master
…or push an existing repository from the command line

git remote add origin https://github.com/mingruyue/notebook.git
git push -u origin master
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
