#从0开始做一个包含服务端的IM跨平台APP（一） --- React开发环境/相关第三方配置


![Alt text](https://upload-images.jianshu.io/upload_images/2166258-afbae36f76dde4c0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "APP相关技术架构如上图所示" )

整体技术架构如图所示
* * *

###安装脚手架并启动
   <pre> <code> 
   npm install -g create-react-app
   </code></pre>
 
 <p>利用脚手架新建一个app testIM</p>
   
 <pre><code>
 create-react-app testim
 </code></pre>
 *app名字不能包含大写字母
  
 <p>安装完成启动app</p>
    <pre>
     cd /Users/taogumbp/Desktop/资料/testim  
     npm start 
    </pre>
    
![Alt text](https://upload-images.jianshu.io/upload_images/2166258-b2959dde45b102d3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "启动成功")
启动成功
* * *

![Alt text](https://upload-images.jianshu.io/upload_images/2166258-f36364f074e1162a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "相关配置")

脚手架文件相关配置如下图所示
* * *
###如何使用create-react-app
* npm install redux --save 安装第三方库redux
* npm run eject 弹出配置文件，自定义webpack
* 拓展package.json里script字段，npm run命令

在创建 React 项目之后，使用 npm run eject 命令报错：This git repository has untracked files or uncommitted changes

原因<br>
因为在初始化项目之后，该项目并没有本地 git 仓库，而此项目目录下又有 .gitignore 文件，所以此时会向上级寻找未提交的项目。

解决方法<br>
1.初始化仓库 git init<br>
2.添加并提交 git add .   git commit -m '初始化项目'<br>
3.重新执行 npm run eject


到这一步，我们的app框架就初步搭建起来了！！
