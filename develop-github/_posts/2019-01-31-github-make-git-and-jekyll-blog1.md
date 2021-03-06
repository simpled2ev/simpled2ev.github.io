---
layout: post
author: author1
title: [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (1)
description: >
  make github blog using github page and jekyll
permalink: /develop-github/2019-01-31-github-make-git-and-jekyll-blog1.md
---
# [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (1)
> GitHub Page, Jekyll을 이용하여 블로그를 만드는 방법

## 1. GitHub 회원가입 및 로그인
깃허브 계정이 있어야 블로그를 제작할 수 있으므로 회원가입을 미리 해야한다.  
먼저 깃허브 사이트에 접속한다.  
<https://github.com/>  
![screenshot](/assets/img/blog/post-2019-01-31/github-signup-view.JPG)  

<br>
Username, Email, Password를 입력하고, **'Sign up for GitHub'** 를 누른다.  
가입 시 입력한 이메일 주소로 들어가면 GitHub에서 메일이 왔을 것이다.  
이메일 인증을 진행한 후, 깃허브에 로그인을 한다.

<br>

## 2. Git 설치
Git 설치 사이트에 접속하면 자동으로 설치파일이 다운된다.  
<https://git-scm.com/download/win>  
![screenshot](/assets/img/blog/post-2019-01-31/git-site.JPG)  
<br>
설치 과정에서 따로 설정해야할 것은 없으므로 **Default값** 으로 진행한다.  
**Next>** 를 누르고, **Install** 을 누르면 설치가 완료된다.  
<br>

<table>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup1.JPG"> </td>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup2.JPG"> </td>
  </tr>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup3.JPG"> </td>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup4.JPG"> </td>
  </tr>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup5.JPG"> </td>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup6.JPG"> </td>
  </tr>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup7.JPG"> </td>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup8.JPG"> </td>
  </tr>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup9.JPG"> </td>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup10.JPG"> </td>
  </tr>
  <tr>
    <td> <img src="/assets/img/blog/post-2019-01-31/git-setup11.JPG"> </td>
    <td> </td>
  </tr>
</table>


<br>
설치가 완료되면, **'Git Bash'** 라는 프로그램을 실행하고, 아래 명령어를 입력한다.  
```c
git config --global user.name "깃허브유저네임"  
git config --global user.email "깃허브이메일"  
```

<img src="/assets/img/blog/post-2019-01-31/git-bash2.JPG">

<br>

## 3. Jekyll Themes 적용
지킬 테마 사이트에 접속하여 마음에 드는 테마를 고른다.  
<http://jekyllthemes.org/>  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes1.JPG)  

<br>
나는 'Hydejack' 이라는 테마를 골랐다.  
마음에 드는 테마를 골랐다면 **Homepage** 를 클릭한다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes2.JPG)  

<br>
Hydejack 관련 GitHub 문서에 들어오게 된다.  
Hydejack 소스코드를 내 Repository에 복사하여 수정할 것이다.   
**'Fork'** 를 누른다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes3.JPG)  

<br>
Fork가 완료되면, 해당 Repository에 들어가서 **Settings** 메뉴를 클릭한다.  
Repository Name을 변경한 후, **Rename** 을 눌러준다.  
**'Repository Name = 블로그 주소'** 이기 때문에, **'username.github.io'** 로 입력한다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes4.JPG)  

<br>
Rename을 누르면, **'username/username.github.io'** 로 변경된다.  
![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes5.JPG)  

<br>
나의 경우 Published가 되는데 10분 정도 걸렸다.  
다른 블로그에서는 1분 정도 걸린다고 써져있는 것으로 봤을 때,  
사람마다 걸리는 시간이 다른 것 같으므로 404페이지가 계속 뜬다면 기다려야한다.  
<br>
이 포스팅은 블로그를 다 만들고 작성하는 것이므로, 아래사진은 테마가 수정된 것이다.  
사이트를 들어갔을 때 아래와 같이 보인다면 완료된 것이다.  

![screenshot](/assets/img/blog/post-2019-01-31/jekyll-themes6.JPG)  
