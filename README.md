**陈玉强的个人博客**  
=========  
  
**一、java学习笔记**  
-------  
**10月18日总结** 
1.java是一门面向对象的编程语言  
2.java 中区分大小写   

**二、git学习笔记**  
-------
**10月18日总结**  
**1、git 命令**  
git init：初始化  
git status：查看当前状态  
git diff：查看不同
git add 文件名 ：将文件放入暂存区  
git commit -m"描述信息":提交更改，实际上就是把暂存区的所有内容提交到当前分支  
git log:查看提交日志  
git reflog：查看每一次命令（后悔药）
git log --pretty=oneline：简单查看提交日志  
git reset -hard HEAD^:回退到上一版  
cat 文件名：查看文件内容  
git rest --hard 版本号前几位：回退到该版本  
qwd:查看当前路径  
cd 文件地址：进入输入的地址  
**2、git的三个工作区**  
&ensp;&ensp;三个区即工作区（repository）、暂存区（stage）、分支（master)。  
&ensp;&ensp;工作区存放的是文件夹内可以看到的文件；暂存区存放的事从工作区提交过来的文件（即执行git add）和修改的文件；分支是git自动创建的master，以及master的一个指针HEND,HEND永远指向master，即当前文件。  
&ensp;&ensp;通过git add可以将工作区的文件提交到暂存区，git commit可将暂存区文件一次性提交到分支。  

![](https://www.liaoxuefeng.com/files/attachments/919020074026336/0)  
        
![](https://www.liaoxuefeng.com/files/attachments/919020100829536/0)  
**3、学习过程及感悟**  
&ensp;&ensp;今天在执行·git add 文件名·的时候，总是显示不能检索到文件，后来才发现原来自己在保存readme.txt的时候没有加txt的后缀，而是在输入文件名的下一栏中选择了.txt格式，显然两种操作是不同的。从解决完这个问题后，我就一路开挂，真正体验到git的魔力，爽到爆！！尤其是在学习完之后在markdownpad上写笔记，再将笔记添加到这个网站上，这中间的过程真的是太爽了！  
