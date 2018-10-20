# react-native
## 一、搭建环境
###  1、使用Homebrew
- mac OS X操作系统，同时可以开发iOS和Android应用
- 使用Homebrew通用包管理工具
- 更新brew和相关依赖包
```
brew update
brew upgrade
```
### 2、用brew安装环境依赖包
- React Native包管理器同时使用了node和watchman
- flow是Facebook公司的一个类型检查库
```
brew install node
brew install watchman
brew install flow
```
### 3、安装React Native
- 用npm来安装React Native
```
npm install -g react-native-cli
```
### 4、安装iOS依赖
- 需要获取一个iOS开发者账号（免费的）
- 需要下载并安装Xcode

### 5、安装Android依赖

第一步 : 下载 mac 版的 JDK
下载地址: http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
// 同意协议并点击下载
 

第二步 : 下载完成后, 按提示完成安装.
打开Finder,可以在下图所示的路径中找到安装好的jdk:
其中Contents下的Home文件夹，是该JDK的根目录
 ![JDK的根目录](https://github.com/JackYang3567/react-native/blob/master/img-storage/jdk_dir.png)


 

其中：

bin目录下存放JDK用于开发的一些终端命令工具。常见的工具如：
“javac”的作用是将java源文件编译为class文件(即自解码文件)；
“java”命令的作用是运行class文件。
 
db目录下是java开发的一个开源的关系型数据库；
 
include目录下是一些C语言的头文件；
 
jre目录下JDK所依赖的java运行时；
 
lib目录下存放JDK开发工具所依赖的一些库文件；
 
man目录下存放JDK开发工具的说明文档。
 

第三步 : 安装好JDK后需要配置JDK的环境变量，

 

1.在英文输入法的状态下，按键盘“Ctrl + 空格”组合键，调出Spotlight搜索，在这里可以快速启动终端，输入ter,然后回车，即可打开终端：



 



 

2.如果你是第一次配置环境变量，可以使用“touch .bash_profile” 创建一个.bash_profile的隐藏配置文件(如果你是为编辑已存在的配置文件，则使用"open -e .bash_profile"命令)：



3.输入“open -e .bash_profile”命令：



 

4.输入如下配置：

JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_40.jdk/Contents/Home
PATH=$JAVA_HOME/bin:$PATH:.
CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
export JAVA_HOME
export PATH
export CLASSPATH

然后保存关闭该窗口。

 

// 下面标红的路径换成你安装的 JDK 路径



5.使用"source .bash_profile"使配置生效，然后输入”java -version”，如果看到jdk版本为1.8则说明配置已经生效：

 



 

第四步 : 测试开发环境

 打开终端, 在命令提示符后面直接输入 : javac , 按回车键,系统会输出 javac 的帮助信息, 如果成功说明已经成功配置了JDK , 否则需要仔细检查上面的步骤的配置是否正确
安装Android开发环境分三个阶段：
- 安装SDK
- 安装模拟器
- 创建模拟器
