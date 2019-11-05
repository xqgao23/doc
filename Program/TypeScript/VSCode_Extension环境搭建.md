# VSCode Extension环境搭建

本文重点介绍VS Code Extension的安装搭建, 安装环境在WSL下.

## 安装nodejs, npm

``` bash
sudo apt-get install nodejs
sudo apt-get install npm
```

## 安装Yeoman 和 VS Code EXtension Generator

``` bash
sudo npm install -g yo generator-code
```

这时需要的工具已安装完成, 现在开始做一个插件

## 先生成新扩展项目目录及代码框架

``` bash
yo code
```

## 编译

``` bash
cd helloworld
code ./
```

然后按下F5编译. 这个时候可能出现编译错误, 需要安装下node-typescript

## 安装node-typescript

``` bash
sudo apt-get install node-typescript
```

可能还有其他错误, 如
> Cannot find moudule 'vscode'

可以通过执行 ` npm install `  解决.
