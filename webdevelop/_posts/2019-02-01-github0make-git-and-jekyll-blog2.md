---
layout: post
author: author1
title: [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (2)
date: 2019-02-01 09:20:05 -0600
description: >
  make github blog using github page and jekyll
---
# [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (2)

> Atom 에디터를 이용하여 블로그를 수정하는 방법  

## 1. Git Clone
저번에 복사해온 Jekyll파일들을 수정하기위해서는, 먼저 내 컴퓨터에 소스를 받고 관리해야한다.  
**'Git Bash'** 를 실행하고, 작업폴더를 생성한다.  

> cd c:  
> mkdir workspace  
> cd workspace  
> mkdir simpled2ev  
> cd simpled2ev  
> git clone http://github.com/simpled2ev/simpled2ev.github.io  
> ls  

<br>

[ 명령어 정리 ]
1. **'mkdir'** : 폴더를 만드는 명령어  
2. **'git clone'** : 깃 저장소를 복사해오는 명령어  
3. **'ls'** : 현재 디렉토리에 있는 파일과 폴더를 보여주는 명령어  

명령어를 모두 실행하면, 아래와 같이 모든 파일이 복사된 것을 볼 수 있다.  
![screenshot](/assets/img/blog/post-2019-02-01/git-clone1.JPG)  


## 2. Atom 에디터 설치
Atom이 아니더라도, 평소 선호하는 에디터를 사용하면된다.  
Edit Plus, Blackets 등이 있다면 그것을 사용해도 괜찮다.  
작성자는 Atom을 이용하여 파일을 수정할 것이다.  
Atom 사이트에 접속하여 **'Download'** 를 클릭한다.  
<https://atom.io/>  
![screenshot](/assets/img/blog/post-2019-02-01/atom-setting1.JPG)  

다운을 받은 후, Atom을 실행한다.  
이제 Git Clone을 실행하여 받은 내용을 Atom에서 열어야한다.  
화면 상단 도구에서 **'File > Open Folder'** 을 클릭하거나, **'Ctrl + Shift + O'** 를 눌러 창을 연다.  
아래와 같은 창이 뜨면, 작업 디렉토리를 클릭한다.  
![screenshot](/assets/img/blog/post-2019-02-01/atom-setting2.JPG)  

**'폴더선택'** 을 클릭하면 simpled2ev.github.io 프로젝트가 열리면서 파일 목록이 왼쪽에 뜰 것이다.  
![screenshot](/assets/img/blog/post-2019-02-01/atom-setting3.JPG)  


## 3. Jekyll 관련 파일
파일 확장자는 .md, .css, .js, .html, .yml 등이있다.  
.css, .js, .html 확장자는 웹 개발을 하다보면 보게되는데, .md와 .yml확장자는 아마 낯설 것이다.  
1. .md : 주로 블로그 포스팅 내용을 작성할 때 생성하는 파일이다.
파일 제목은 yyyy-mm-dd-title.md의 형식으로 작성하며, 내용은 Markdown 형식으로 작성한다.  
2. .yml : 설정파일을 작성한다.

주로 수정하게 되는 파일과 폴더 몇가지를 설명해보자면 아래와 같다.  
1. _config.yml : 블로그의 제목, 폰트, 주소 등의 정보를 담고있는 파일  
2. /_data/authors.yml : 블로그 포스트 하단에 작성자의 정보를 작성하는 파일  
3. 404.md : 페이지 url이 존재하지 않을 경우, 이 파일을 수정하여 커스터마이징 하면된다.  


## 4. _config.yml 수정
간단히 웹페이지의 title과 tagline을 수정해볼 것이다.  
우선 Atom에디터에서 _config.yml 파일을 연다.  
title과 tagline을 찾아 자신이 원하는 문구로 바꾸고, **'Ctrl + S'** 로 파일을 저장한다.  
> title: Yeong A Lee  
> tagline: Web Developer  

파일이 수정되면, Atom에서 해당 파일만 색이 바뀌게 보일 것이다.  
![screenshot](/assets/img/blog/post-2019-02-01/atom-setting4.JPG)  

이제 수정된 파일을 깃허브에 올리는 작업을 해야한다.  
**'Git Bash'** 를 실행하고, 작업 디렉토리로 이동한다.  

> cd c:/workspace/simpled2ev/simpled2ev.github.io  
> git add '_config.yml'  
> git commit -m '수정한 내용을 기록'  
> git push  

![screenshot](/assets/img/blog/post-2019-02-01/git-commit1.JPG)  

만약 git push 명령어를 처음 실행하게된다면, GitHub에 로그인하라는 창이 뜰 것이다.  
로그인을 완료하면 git push가 성공적으로 실행될 것이다.  
화면에 바로 반영되지는 않고, 30초~1분 뒤에 반영된다.  
조금 기다린 뒤에 https://simpled2ev.github.io 로 들어가면 변경된 화면을 확인할 수 있다.  

![screenshot](/assets/img/blog/post-2019-02-01/web-page1.JPG)  
