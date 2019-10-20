**陈玉强的个人博客**  
=========  

**一、java学习笔记**  
-------  
**10月20日笔记**  
今天学习了java的重写(override),要点如下:  
&ensp;&ensp;1.重写是一种建立在继承关系上对父类方法的改写。  
&ensp;&ensp;2.重写代码应放在需要重写的子类中,以方法的形式,并且方法描述与父类完全一致,而重写内容放在方法内。  
&ensp;&ensp;3.重写中若有返回值,则子类返回值必须小于或等于父类返回值。  
另外在我写代码的过程中我犯了一个错误：误将其他类写在main函数中，程序总是报错。应当写在main方法外、主类（就是包含main函数的那个类，不知道具体叫什么）中。  
测试代码如下(注释掉的部分分就是重写):  
```
package yuqiang.com;

public class textInstance {
	public static void main(String[] args) {
		
		SStudent gStudent=new SStudent();
		gStudent.run();

		
	}
	
	
	

}
class vehicle{
		public void run() {
			System.out.println("跑!");
		}
		
		public void  stop() {
			System.out.println("停!");
		}
		
	}
	
	class SStudent extends vehicle{
		public SStudent() {
			
		}
		/*public void run() {
			System.out.println("学生坐车!");
		}*/
		
	}  
```

   

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
&ensp;&ensp;&ensp;&ensp;今天在执行·git add 文件名·的时候，总是显示不能检索到文件，后来才发现原来自己在保存readme.txt的时候没有加txt的后缀，而是在输入文件名的下一栏中选择了.txt格式，显然两种操作是不同的。从解决完这个问题后，我就一路开挂，真正体验到git的魔力，爽到爆！！尤其是在学习完之后在markdownpad上写笔记，再将笔记添加到这个网站上，这中间的过程真的是太爽了！  
&ensp;&ensp;&ensp;&ensp;今天在查看网页的时候，发现“一、java学习笔记”不能正常显示为标题，后来发现，**在上一个大标题下空出一行，且空出那一行不能有空格**，才将问题解决。
