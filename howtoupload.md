# 这个文档给你一个简要的介绍，如何在linux环境下下载git上的项目以及上传你的项目
## 下载
1. 你可以直接登录到github上，打开某个项目，点击clone or download。
2. 直接输入 git clone https://github.com/shareWithU/guojiaotong下载项目。
## 上传
1. cd 到上传项目的根目录下，然后初始化本地仓库，使用命令git init
2. 添加当前工作目录的文件，使用命令git add .(add后面有个“.”，和add之间有个空格，“.”表示当前目录)
3. 查看当前目录下是否有未被git管理的文件，以及被修改但是未提交的文件。使用命令git status（若有很多红色文件，重复步骤2,直到都是绿色）
4. 设置你要提交到的地址以及密码，使用命令 git config --global user.email "xxxx"     
git config --global user.name "xxxx"
5. 提交文件，使用命令git commit -m "这里写修改的备注"
6. 关联远程仓库，origin后跟的是远程仓库的别名    
git remote add origin https://github.com/shareWithU/guojiaotong.git
7. git push -u origin master