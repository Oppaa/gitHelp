
##gitHelp

>**场景：** rebase master后若冲突不断可用

```bash
$ git merge-base master 'branch'
$ git reset [commit]
$ git add .
$ git commit -m 'ok'
```


>**场景：** 提交代码基本姿势

```bash
$ git checkout master 
$ git pull
$ git checkout 'branch'
$ git pull --rebase origin 'branch'
$ git rebase master
$ git push origin 'branch'
```


>**场景：** 小心翼翼地更新本地代码

```bash
$ git fetch origin master:'branch'
$ git diff 'branch'
$ git merge 'branch'
$ git branch -d 'branch'
```

>**场景：** apply分支变化

```bash
git cherry-pick <commit id>
```

=======


#### node&npm

```bash
npm -v                  #显示版本，检查npm 是否正确安装。

npm install express     #安装express模块

npm install -g express  #全局安装express模块

npm view express dependencies

npm update express

npm list                #列出已安装模块

npm show express        #显示模块详情

npm update              #升级当前目录下的项目的所有模块

npm update express      #升级当前目录下的项目的指定模块

npm update -g express   #升级全局安装的express模块

npm uninstall express   #删除指定的模块

npm cache clear         #清理
```

#### scss

```bash
sass --watch --scss style.scss:style.css

* nested：嵌套缩进的css代码，它是默认值。
* expanded：没有缩进的、扩展的css代码[常用]
* compact：简洁格式的css代码。
* compressed：压缩后的css代码。

sass --style compressed test.sass test.css
```


#### mongodb

```bash
mongod  //启动

use admin  // 切换至admin后才能关闭
db.shutdownServer() 
```
