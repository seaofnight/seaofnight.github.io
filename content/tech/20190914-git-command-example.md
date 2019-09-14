Title: git-command-example
Date: 2019-09-14 18:20
Modified: 2019-09-14 18:20
Category: git
Tags: git
Slug: git-command-example
Authors: yjkim 
Summary: git

# common 명령어 
* git init 
    * 일반 폴더에서 깃 저장소로 만들어 준다. 

* git config 
    * 깃 저장소의 설정을 변경한다. 예시로 유저명, 메일등을 설정 할 수 있다. 

```sh 

$ git config --global user.name "yjkim1@gmail.com" 
$ git config --global user.email "yjkim1@gamil.com"

```

* git help 

* git status 

# upload, download 관련 

* git add
    * git 에 업로드 하기 위하여는 add commit 의 순서를 거치는데 우리가 어떤 파일을 로컬 레포에 저장할 것이다 라는 명령어이다. 
```sh 
$ git add . # current folder 
$ git add readme.md # readme.md 
```


* git commit 
    * commit 시에는 message 를 날려주면 된다. 
```sh 
$ git commit -m "add pelican source" 

# 그러면 아래와 같이 로그에 출력이 되며 깃헙에도 메시지가 올라가게 된다. 
$ git log 
commit 4fb60f7260f17fee8cc5b6e4eaf779d8997a2a5a (HEAD -> gh-pages, origin/gh-pages)
Author: yjkim <seaofnight@hanmail.net>
Date:   Sat Sep 14 18:58:04 2019 +0900

    add pelican source
```

* git branch 

* git checkout 
    * git branch 간에 이동을하거나 삭제를 하고자 할떄 사용한다. 
```sh 
$ git checkout branch_name 
# 변경하면 폴더도 해당 브렌치에 맞도록 변경이 된다. 
```

* git push 
    * local 레포에 있는 변경사항을 원격 레포로 업로드 한다. 
```sh 
$ git push origin master 
# 다른 레포지토리로 업로드 하고 싶으면 이렇게 하면 된다. 
$ git push -u origin gh-pages

# 원격 레포의 브랜치 삭제 : git push --delete <remote-name> <branch-name>
$ git push --delete origin gh 
```

* git pull 
    * git 원격 레포에 있는 내용을 가져오는 명령이다.
