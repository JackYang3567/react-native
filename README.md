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
安装Android开发环境分三个阶段：
- 安装SDK
- 安装模拟器
- 创建模拟器
