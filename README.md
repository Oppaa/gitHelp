gitHelp
=======

>**场景：** rebase master后若冲突不断，可用

```bash
$ git merge-base master 'branch'
$ git reset [commit]
$ git add .
$ git commit -m 'ok'
```


---


>**场景：** 提交代码基本姿势

```bash
$ git checkout master 
$ git pull
$ git checkout 'branch'
$ git pull --rebase origin 'branch'
$ git rebase master
$ git push origin 'branch'
```

---


>**场景：** 小心翼翼地更新本地代码

```bash
$ git fetch origin master:'branch'
$ git diff 'branch'
$ git merge 'branch'
$ git branch -d 'branch'
```

