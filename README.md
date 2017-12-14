# jenkins
使用docker-jenkins的自动化构建+部署

## docker-jenkins和docker-ngnix安装在同一台电脑上

## docker-jenkins和docker-ngnix安装在两台电脑上

这两种操作其实是一样的：
1. 为jenkins安装publish over ssh插件
2. 配置ssh远程操作
![](https://raw.githubusercontent.com/jackgreentemp/jenkins/master/Jenkins%E5%9C%A8mac%E7%94%B5%E8%84%91build%E4%B9%8B%E5%90%8E%E5%B0%86%E4%BB%A3%E7%A0%81%E9%83%A8%E7%BD%B2%E5%88%B0%E5%8F%A6%E4%B8%80%E5%8F%B0%E7%94%B5%E8%84%91%E7%9A%84%E8%99%9A%E6%8B%9F%E6%9C%BAlinux/%E7%B3%BB%E7%BB%9F%E7%AE%A1%E7%90%86-%E7%B3%BB%E7%BB%9F%E8%AE%BE%E7%BD%AE-publish%20over%20ssh.png)
3. 在Jenkins工程配置中，将build之后的文件通过ssh发送到服务器放置代码的目录
![](https://raw.githubusercontent.com/jackgreentemp/jenkins/master/Jenkins%E5%9C%A8mac%E7%94%B5%E8%84%91build%E4%B9%8B%E5%90%8E%E5%B0%86%E4%BB%A3%E7%A0%81%E9%83%A8%E7%BD%B2%E5%88%B0%E5%8F%A6%E4%B8%80%E5%8F%B0%E7%94%B5%E8%84%91%E7%9A%84%E8%99%9A%E6%8B%9F%E6%9C%BAlinux/%E7%B3%BB%E7%BB%9F%E7%AE%A1%E7%90%86-%E7%B3%BB%E7%BB%9F%E8%AE%BE%E7%BD%AE-publish%20over%20ssh.png)
