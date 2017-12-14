# jenkins
使用docker-jenkins的自动化构建+部署

## docker-jenkins和docker-ngnix安装在同一台电脑上

## docker-jenkins和docker-ngnix安装在两台电脑上

这两种操作其实是一样的：
1. 为jenkins安装publish over ssh插件
2. 配置ssh远程操作
3. 在Jenkins工程配置中，将build之后的文件通过ssh发送到服务器放置代码的目录
