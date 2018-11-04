- 1
	- 配置
		- git config --global user.name "Your Name"     // 配置用户名
		- git config --global user.email "Your Email"   // 配置邮箱
	- 下载
		- git clone git@github.com:hxdaxu/GitDemo.git

	- 添加至缓存区
		- git add <file name>           // 将修改内容添加至暂存区
		- git add --all                 // 添加所有改变的已跟踪文件和未跟踪文件
		- git add .

	- 工作区、暂缓区、HEAD差别
		- git diff                      // 工作区和暂存区差异比较
		- git diff --cached             // 暂存区和 HEAD 的差异
		- git diff HEAD                 // 工作区和 HEAD 的差异
	- 查看状态
		- git status

	- 提交
		- git commit -m "message" 

	- 重置、回退
		- git reset --soft HEAD^        // 重置上次提交，保留修改的内容
		- git reset --hard HEAD^        // 彻底重置上次提交，不保留修改
		- git reset --hard <commit id>  // 彻底重置至某次提交，不保留修改
		- git checkout [file] 检出文件，丢出改动

	- 查看历史
		- git log                       // 查看提交历史
		- git log --oneline             // 提交历史简短显示
		- git log -5                    // 查看最近5条提交历史

	- 分支
		- git checkout <branch_name>    // 切换分支
		- git checkout -b <branch_name> // 创建并切换到该分支
		- git branch                    // 查看本地分支列表
		- git branch <branch_name>      // 创建新分支，基于当前HEAD
		- git branch -D <branch_name>   // 删除分支
	- 进度栈
		- git stash                     // 保存进度
		- git stash pop                 // 恢复最近一次保存的进度
		- git stash save "message"      // 保存进度，并添加一个描述
		- git stash list                // 查看保存的进度列表

	- cherry pick
		- git cherry-pick <commit ID>   // 拣选一次提交应用于当前HEAD