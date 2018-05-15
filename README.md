# 几个年轻人学点手艺

* 通过这个项目学习react
* 通过这个项目学习Ant
* 根据以往的项目，抽取了常用的东西出来，方便以后有类似的项目的时候能快速开发



## 模板

```
- Dashboard
  - Analytic
  - Monitor
  - Workspace
- Form
  - Basic Form
  - Step Form
  - Advanced From
- List
  - Standard Table
  - Standard List
  - Card List
  - Search List (Project/Applications/Article)
- Profile
  - Simple Profile
  - Advanced Profile
- Result
  - Success
  - Failed
- Exception
  - 403
  - 404
  - 500
- User
  - Login
  - Register
  - Register Result
```

## 开始

```bash
$ git clone https://github.com/gui-sukla/sgaiAdmin.git
$ cd sgaiAdmin
$ npm install
$ npm start         # visit http://localhost:8000
```




## 兼容

Modern browsers and IE11.

## 伙伴

成员|描述|评价
-|-|-
大小宇|中单|cary全场
zhang645|打野|随时GANK
凯茜|ADC|好好发育
皮|上单|上单稳住
sukla|辅助|买眼打酱油

### git pull

## 清除变更

### git checkout .

## 添加文件到本地仓库

### git add 

## 查看服务器地址

### git remote

## 检查本地仓库文件状态

### git status

## 保存变更到本地仓库

### git commit -m "备注"

## 提交变更到服务器主分支

### git push origin master

## 创建分支

## 合并分支

## 删除分支

## 多人开发

### 创建一个组织

### 添加成员

### 添加一个项目

### 将一个已有的项目添加进来

#### 第一步要设置当前的项目的remote

##### 删除本地项目原来的remote-->git remote rm origion

##### 设置为当前组里添加的哪一个项目的ssh路径-->git add origion git@github.com:weblzzds/sgaiAdmin.git

#### 第二步要将两个项目的分支合并

##### 设置对应的分支-->git branch --set-upstream dev origin/<branch>

##### 允许两个不同的项目合并-->git pull origin master --allow-unrelated-histories

#### 第三步要设置开发人员的ssh并添加到sshkeys

##### 生成ssh公钥(在gitbash终端)-->ssh-keygen -t rsa -C "git的用户名"

##### 终端中一路回车最后生成了ssh在这个目录-->Your public key has been saved in /c/Users/Sukla/.ssh/id_rsa.pub.

##### 使用cat命令查看文件内容-->cat /c/Users/Sukla/.ssh/id_rsa.pub

##### 将cat返回的内容全部copy添加到项目的sshkeys中