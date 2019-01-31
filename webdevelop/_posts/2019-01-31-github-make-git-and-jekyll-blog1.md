---
layout: post
author: author1
title: [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (1)
description: >
  make github blog using github page and jekyll
---
# [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (1)
> 구글링을 하다보면 https://devtest/github.io 형식으로 되어있는 사이트들을 본 적이 있을 것이다.  
> GitHub Page, Jekkyll을 이용하여 개발 블로그를 생성할 것이다.  

## 1. GitHub 회원가입 및 로그인
깃허브 계정이 있어야 블로그를 제작할 수 있으므로 회원가입을 미리 해야한다.  
먼저, 깃허브 사이트에 접속한다.  
<https://github.com/>  
![screenshot](/assets/img/blog/post-2019-01-31/github-signup-view.JPG)  

<br>
Username, Email, Password를 입력한 후, **'Sign up for GitHub'** 를 누른다.  
가입 시 입력한 이메일 주소로 들어가면, Github에서 메일이 온 것을 확인할 수 있다.  
이메일 인증을 진행한 후, 깃허브에 로그인을 한다.

<br>

## 2. Git 설치
깃 설치 사이트에 접속하면 자동으로 다운이 진행된다.  
<https://git-scm.com/download/win>  
![screenshot](/assets/img/blog/post-2019-01-31/git-site.JPG)  
<br>
설치할 때 뜨는 것 중에서 따로 설정해야할 것은 없으므로 **Default값** 으로 진행한다.  
**Next>** 를 계속 누르고, **Install>** 을 누르면 설치가 완료된다.  
<br>

![screenshot](/assets/img/blog/post-2019-01-31/git-setup1.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup2.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup3.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup4.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup5.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup6.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup7.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup8.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup9.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup10.JPG)  
![screenshot](/assets/img/blog/post-2019-01-31/git-setup11.JPG)  
<br>
설치가 완료되면, Git Bash라는 프로그램이 생길 것이다.  
깃허브에 로그인되어있는 상태로 Git Bash를 실행하면 된다.  
![screenshot](/assets/img/blog/post-2019-01-31/git-bash1.JPG)  

<br>
위와 같은 화면이 나오면, 아래 명령어를 입력한다.  
> git config --global user.name "깃허브유저네임"  
> git config --global user.email "깃허브이메일"  

![screenshot](/assets/img/blog/post-2019-01-31/git-bash2.JPG)  

<br>

## 3. Jekyll Themes 적용
<http://jekyllthemes.org/>  
지킬 테마 사이트에 접속하여 마음에 드는 테마를 고른다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes1.JPG)  

<br>
나는 Hydejack 라는 테마를 골랐다.  
마음에 드는 테마를 골랐다면, **Homepage** 를 클릭한다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes2.JPG)  

<br>
Hydejack관련 GitHub 문서에 들어오게 된다.  
Hydejack 소스코드를 내 Repository에 복사하여 수정하기위해 **Fork** 를 누른다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes3.JPG)  

<br>
Fork가 완료되면, 해당 Repository에 들어가서 **Settings** 메뉴를 클릭한다.  
Repository Name을 변경한 후, Rename을 눌러준다.  
**Repository Name == 블로그 주소** 이기 때문에, **'깃허브유저네임.github.io'** 로 입력한다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes4.JPG)  

<br>
Rename을 누르면, 아래와 같이 깃허브유저네임/깃허브유저네임.github.io 로 변경된 것을 볼 수 있다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes5.JPG)  

<br>
나의 경우 Published가 되는데 10분 정도 걸렸다.
다른 블로그에서는 1분 정도 걸린다고 써져있는 것으로 봤을 때,
사람마다 걸리는 시간이 다른 것 같으므로 404페이지가 계속 뜬다면 기다려야한다.  
<br>
아래 사진은 블로그를 다 만들고 포스팅을 하는 것이어서 테마가 약간 수정되었다.  
사이트를 들어갔을 때 아래와 같이 뜨면 성공적으로 완료된 것이다.  

![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes6.JPG)  
