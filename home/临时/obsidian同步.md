# onedrive
- 软件需要：syncfolder（安卓）
# git
- 软件需要：
	- pc：git、github for desktop
	- 安卓：Mgit
## 电脑操作流程：
- 第一次上传：
	1. git520修改hosts，给github提速
	2. 注册github账户
	3. 在网页上新建仓库，并复制ssh地址
	4. 打开本地obsidian文件夹，首次 git bash
		1. git init
		2. git config --global user.name xxxx
		3. git config --global user.email xxxx@
		4. ssh,并添加到github settings中
		5. remote add origin git@github:xxxx
		6. 在仓库根目录下创建.gitignore，写入：appearance.json
		7. add .
		8. commit -m 消息
		9. git push origin master
- 以后每次修改：
	1. 每次在电脑上修改前：git pull origin master
		- 出现冲突：在github for desktop中查看，若无关紧要则“diagard the change"，若是需要保留的更改则先add commit ,再pull
		- 请务必遵照修改先pull，修改后push的准则，这样将不可能有任何 冲突
	2. 修改后：git push origin maste
	- 可以在github for desktop中查看历史修改
## 手机操作流程
- 第一次将仓库下载到手机：
	1. Mgit中创建ssh key，并添加到github settings中
	2. 从网页上复制仓库ssh地址，克隆到本地
- 以后每次修改：
	- 修改前先点“拉取”
	- 修改后点“提交”，“推送”即可