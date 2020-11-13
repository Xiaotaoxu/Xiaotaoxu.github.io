## github仓库操作的一些方法

对origin关键字的解释
##
git 默认用这个关键字来标识你克隆的原始远程仓库。
所以，当你clone了一个远程仓库到本地时，有时候你需要用git remote add origin <仓库地址>, 来为远程仓库在你本地取个别名，这样才能下次push的时候，push到origin对应的远程仓库中取。


## 
用github托管工作一般流程
1.git clone <仓库地址>
2.change your content
3.git add <your change>
4.git commit -m "your descrtion" // git commit -a
5.git push origin master  //主分支，不需要merge
  git push origin HEAD:refs/for/master //新分支，需要主分支merge， 现在在github上试验还是失败的.
  在push的时候，需要输入你github的用户名和密码。