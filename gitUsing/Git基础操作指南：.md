# git的安装：
[Git (git-scm.com)](https://git-scm.com/)

# git的使用基本操作：
1. 在github创建远程仓库
	1. 注册一个github账号[GitHub](https://github.com/)
	2. 创建一个远程仓库![[Pasted image 20241108192707.png]]
		*对，就是那个new，然后输入仓库的名字就好了*
	3. 复制一下url，后面会用![[Pasted image 20241108192823.png]]
		*就是中间那一串地址* 
1. git init
	1. 找到你要建立本地仓库的位置，比如D:/Myproj/
	2. 打开文件夹，对着空白处右键，有个在终端中打开
	3. 然后输入git init
	4. git config -global user.email ”你的邮箱“
	5. git config -global user.name "你的id"
2. git add filename
	1. filename 是指你要添加的文件名字，带后缀！
	2. 如果是某一文件夹下的所有文件，    .\文件夹名字\*.*
	3. ps:可以用git status查看当前保存了哪些文件的快照
3. git commit -m (msg)
	1. msg是代表这次提交到本地库的备注
	2. commit的作用是把你之前add进去的文件塞到本地仓库
	3. 注意，commit之后add的暂存区会清空![[Pasted image 20241108222040.png]]
4. git push (url) (branch)
	1. 这个操作就是把本地的commit的文件全部塞进你的远程仓库里
	2. 这个url就是前面让你复制的url！记得要带分支名字，比如master
	3. ![[Pasted image 20241108222220.png]]
6. git pull url:
	1. 用来拉取你要下载的文件夹，顾名思义，但是需要先init才能拉取！
	2. 注意！这个url是你要下载的那些文件的url，不是你建立的仓库的url！
	3. 具体怎么获得url，打开别人发给你的仓库地址，然后打开，按照原来找url的方法找到这个仓库的url，然后就能拉取了！
	4. 所谓的拉取就是下载下来（）
7. git branch的操作
	1. 这个操作有点复杂，请详见[Git 分支管理 | 菜鸟教程 (runoob.com)](https://www.runoob.com/git/git-branch.html)