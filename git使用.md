# 下载



下载链接：https://git-scm.com/

![image-20210910130310014](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910130310014.png)



# 安装



![image-20210910104312124](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910104312124.png)![Snipaste_2021-09-10_10-55-02](C:\Users\WYF\Desktop\git PPT+ 演示程序\Snipaste_2021-09-10_10-55-02.png)

左图：成功安装后同时添加的三个软件，我们只使用Git Bash执行命令；

右图：Git bash的界面，一般右键需要提交的文件夹，选择“git bash here”即可开始输入命令



# 配置

## 配置用户名

#### `git config --global user.name 'name'`

![2](C:\Users\WYF\Desktop\git PPT+ 演示程序\2.png)

## 配置邮箱

#### `git config --global user.email 'email'`

![3](C:\Users\WYF\Desktop\git PPT+ 演示程序\3.png)



# 初始化本地版本库

#### `git init`

![4](C:\Users\WYF\Desktop\git PPT+ 演示程序\4.png)



# 创建文件并提交本地库

## 第一步：在文件夹中创建文件，添加内容

### 

![5](C:\Users\WYF\Desktop\git PPT+ 演示程序\5.png)



## 第二步：分别提交到暂存区，本地库

#### `git add file //将文件提交到暂存区`

#### `git commit -m "这是注释" // 将文件提到本地库`

![6](C:\Users\WYF\Desktop\git PPT+ 演示程序\6.png)



# 修改文件并提交本地库

#### `git add file` 

#### `git commit -m` 

![image-20210910120214083](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910120214083.png)



# 版本回退或前进

查看带有版本号的显示日志（从最近开始）`git reflog` 

回退上一版本 `git reset --hard HEAD^`

回退 / 前进到某一版本：`git reset --hard 版本号`

#### （1）查看带有版本号的显示日志

![7](C:\Users\WYF\Desktop\git PPT+ 演示程序\7.png)



#### （2）回退上一版本

![image-20210910120719843](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910120719843.png)



#### （3）回退 / 前进到某一版本

![image-20210910120916564](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910120916564.png)



# 创建分支

#### 创建分支：`git branch <name>`

![image-20210910121916540](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910121916540.png)



#### 查看分支：`git branch`

![image-20210910121928470](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910121928470.png)



#### 切换分支：`git checkout <name>`或者`git switch <name>`

![](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910121942193.png)



#### 创建+切换分支：`git checkout -b <name>`或者`git switch -c <name>`

![image-20210910122044994](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910122044994.png)



# 合并分支

#### 合并某分支到当前分支：`git merge <name>`

![image-20210910122456741](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910122456741.png)



# 删除分支保存分支内容

#### 删除分支：`git branch -d <name>`

![image-20210910123219063](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910123219063.png)



#### 删除分支并保存分支内容 `git merge --no-ff -m "merge with no-ff" <name>`![image-20210910123350014](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910123350014.png)



# 撤销修改

#### `git  checkout -- file.name`

![image-20210910123521221](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910123521221.png)





# 删除文件

#### `rm test.txt`

![image-20210910123602736](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910123602736.png)





# 生成并添加ssh公钥

#### 生成 / 添加公钥

#### `mkdir key_backup`

#### `ssh-keygen - t rsa -C "1959198478@qq.com"`

![image-20210910123855770](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910123855770.png)



##### 这里要注意：.pub文件里面存的就是我们需要的公钥代码

![image-20210910130535040](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910130535040.png)



#### 新建公钥

![8](C:\Users\WYF\Desktop\git PPT+ 演示程序\8.png)





#### 添加公钥

![image-20210910124621113](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910124621113.png)





# 本地仓库推送GitHub仓库

#### 第一步：新建远程库

![9](C:\Users\WYF\Desktop\git PPT+ 演示程序\9.png)



![image-20210910124856026](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910124856026.png)



#### 本地仓库关联远程仓库 —— git remote add origin 远程仓库地址

![image-20210910125027406](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910125027406.png)



#### 本地仓库master主分支推送到远程仓库—— git push -u origin master 远程地址

![image-20210910125039221](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910125039221.png)





# 本地仓库克隆

#### `git clone 远程仓库地址`

![image-20210910125340348](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910125340348.png)



# 常见冲突

## 分支与主分支同时修改文件

#### 1、在分支dev里修改第三行

![image-20210910125819462](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910125819462.png)



#### 2、切换至主分支master，同样修改第三行

![](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910125855617.png)



#### 3、合并时提示有冲突

![](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910130026109.png)



#### 解决方法：修改冲突部分内容，再次提交即可

![image-20210910130043255](C:\Users\WYF\AppData\Roaming\Typora\typora-user-images\image-20210910130043255.png)