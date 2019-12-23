# Visual Studio Code
## 一、**快捷键说明**
### *项目相关*
>* 新建项：Ctrl+Shift+A
>* 新建项目：Ctrl+Shift+N
>* 打开项目：Ctrl+Shift+O
>* 保存项目：Ctrl+S
>* 生成项目:Ctrl+Shift+B
>* 添加新类：Shift+Alt+C
>* 添加新项目到项目：Shift+Alt+A
>* 显示Solution Explorer（解决方案资源管理器）：Ctrl+Alt+L

### *调试相关*
>* 设置断点：F9
>* 调试(启动)：F5
>* 停止调试：Shift+F5
>*  调试(逐语句)：F11
>* 调试(逐过程)：F10
>* 取消所有断点：Ctrl+Shift+F9
>* 调试(开始执行不调试)：Ctrl+F5
>* 调试(重新启动)：Ctrl+Shift+F5
>* 停止快捷匹配： Ctrl+Alt+Q
>* 附加到进程：Ctrl+Alt+P

### *编辑相关*
>* 在当前行插入空行：Ctrl+Enter
>* 在当前行下方插入空行：Ctrl+Shift+Enter
>* 使用IntelliSense（智能感知）自动完成：Ctrl+空格键
>* 选择代码的自定义部分：Alt+Shift+箭头键(←,↑,↓,→)
>* 匹配大括号、括号：Ctrl+}
>* 在匹配的括号、括号内选择文本：Ctrl+Shift+}
>* 保存所有文件和项目:Ctrl+Shift+S
>* 注释选定行：Ctrl+C
>* 取消选定行的注释：Ctrl+K
>* 正确对齐所有代码：Ctrl+D
>* 从头到尾选择整行：Shift+End 
>* 从尾到头选择整行：Shift+Home
>* 删除光标右侧的所有字：Ctrl+Delete
>* 删除光标左侧的所有字：Ctrl+Backspace
>* 剪切选定行：Ctrl+X
>* 删除选定行：Ctrl+L
>* 转小写：Ctrl+U
>* 转大写：Ctrl+Shift+U
>* 选中从光标起到行首间的代码：Shift+Home
>* 选中从光标起到行尾间的代码：Shift+End

### *搜索相关*
>* 查找所有引用：Shift+F12
>* 显示查找对话框：Ctrl+F 
>* 显示替换对话框：Ctrl+H
>* 跳转到行号或行：Ctrl+G 
>* 查找所选条目在整个解决方案中的引用：Ctrl+Shift+F
>* 在文件中查找：Ctrl+Shift+F 
>* 查找下一个：F3
>* 查找上一个：Shift+F3

## 二、**插件安装卸载**
### *安装插件*
>* Ctrl/Cmd+P (或 Ctrl/Cmd + E) 输入 ext install \[插件关键字/名称\]
>* Ctrl/Cmd+Shift+P (或 F1) 输入 Extensions, 选中 Install Extension然后输入插件名称/关键字.

### *卸载插件*
>* 快捷键 win + R 打开运行 %appdata% 回车，删除当前目录下的 Code 和 Visual Studio Code
>* win + R  输入 %userprofile% 回车，删除当前目录下 删除 .vscode 文件夹

## 三、**使用 Git**
1.  git命令行工具安装
 这里直接上官网下载对应版本即可–>[Git官网链接](https://git-scm.com/ "Git官网")
2. git使用前配置
   1. 在桌面或者任意目录下右键打开git bash（或者直接打开CMD命令行）
   2. 敲入命令
     * git config --global user.name xxxxx
     * git config --global user.email xxx@x
   3.在打开的编辑器中编辑图示字段
     git config --global --edit
3. git基本命令
   >* <pre> git init</pre> 
        >在当前文件夹创建一个git仓库，最直观的就是当前目录下多出了.git文件夹(windows下需要显示隐藏文件夹才能看到，linux下需要ls -a).
   >* <pre> git add </pre> 
       >从当前文件夹添加文件到暂存区域，以便于git追踪.
   >* <pre> git commit -m "do what"</pre> 
       >从暂存区域提交代码到代码仓库，提交说明为 “do what”
   >* <pre>git diff</pre>
        >用来比较仓库，暂存区，工作目录的不同（用法很多）
   >* <pre> git reset</pre> 
       用来回退到上个提交的版本，做了两件事：
        >   1. 修改了HEAD指向（仓库当前版本回退到上个）
        >   2. 将仓库上个版本的文件覆盖到暂存区域，用以丢弃上次的提交，（工作目录，文件夹中的文件还没变）
   >* <pre> git diff</pre> 
        >用来比较仓库，暂存区，工作目录的不同（用法很多）
   >* <pre> git log</pre> 
        >查看版本提交记录
   >* <pre> git status</pre> 
        >查看git仓库当前状态，如有没有 工作区文件未添加到暂存区(Untracked),工作区文件修改未提交到暂存区(Unstaged),暂存区的文件未提交到仓库(Changes to be committed)等等，有问题解决问题。当仓库与工作区，暂存区文件一致时，提示应该是”nothing to commit, working tree clean“
   >* <pre> git checkout</pre> 
        >同git reset一样拥有超多功能，切换分支，回复文件到工作目录，等等
   >* <pre> git branch</pre> 
         创建分支 git branch xxx
   >* <pre> git merge</pre> 
        >合并分支

**说明：这里所有的命令在命令行中都可以 添加 –help弹出官方帮助文档 ，例如 git add --help查看git add的使用说明。**