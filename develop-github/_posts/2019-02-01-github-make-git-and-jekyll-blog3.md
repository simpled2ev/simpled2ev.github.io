---
layout: post
author: author1
title: [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (3)
description: >
  make github blog using github page and jekyll
---

# [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (3)

> Haroopad를 이용하여 블로그 포스트 올리는 방법 (작성중)

## 1. Haroo Pad 설치
GitHub Page와 Jekyll로 만든 블로그에서는 Markdown 형식으로 글을 써야한다.
하루패드는 **Markdown 형식의 글을 쉽게 쓸 수 있도록 도와주는 편집기** 이다.
하루패드 홈페이지에 접속하여 자신의 운영체제에 맞는 설치파일을 다운받는다.
<http://pad.haroopress.com/user.html>

![screenshot](/assets/img/blog/post-2019-02-01/haroo-pad-setting1.JPG)  

설치파일 다운로드가 완료되면, 'Haroopad-v0.13.1-win-x64.exe' 파일을 실행한다.
설치 과정에서 따로 설정해야할 것은 없으므로 Default값 으로 진행한다.
Next> 를 누르고, Install 을 누르면 설치가 완료된다.
설치가 완료되면 시작화면에 'haroopad'라는 것이 생겼을 것이다. 더블클릭하여 실행한다.
아래와 같은 화면이 보이면 성공한 것이다.

![screenshot](/assets/img/blog/post-2019-02-01/haroo-pad-setting2.JPG)  

마크다운을 처음 접하는 사람이라면, 화면 왼쪽 하단의 파란 아이콘을 클릭하여 도움을 받을 수 있다.
마크다운을 작성하는 간단한 방법을 알려주는 도구이다. 포스팅 내용을 작성한다.

![screenshot](/assets/img/blog/post-2019-02-01/haroo-pad-setting3.JPG)  

## 2. Blog Post 올리기
Post 파일은 '메뉴/_post/' 경로에 올려야한다.  
작성자의 경우 'hydejack/_post' 라는 폴더가 있었는데, 폴더명을 'webdevelop/_post' 로 변경했다.  
폴더명은 자신의 블로그에 넣을 메뉴로 만들어주면된다.  
파일을 만들 디렉토리에서 오른쪽마우스를 클릭하고, **'new file'**을 누르면,  
'Enter the path for new file'이라고 뜰 것이다.  
포스팅할 파일의 이름은 **'yyyy-mm-dd-title.md'** 의 형식으로 맞추는 것이 좋다.   
작성자는 아래와 같이 파일을 생성하였다.  

![screenshot](/assets/img/blog/post-2019-02-01/make-post1.JPG)  

완료되었으면, haroopad에서 작성한 글을 복사하여 파일에 붙여넣기한다.  
포스팅 내용 맨 위에 아래 내용을 복사 붙여넣기한다.  

> `---`  
> layout: post  
> author: author1  
> title: [ GitHub ] GitHub, Jekyll을 이용한 블로그 제작 (3)  
> date: 2019-02-01 09:20:05 -0600  
> description: description 내용  
> `---`  

1. author : 글 작성자의 프로필을 포스팅 하단에 적는 것. '_data/authors.yml' 에서 수정할 수 있다.  
2. title : 해당 글의 포스팅 제목  
3. date : 글을 작성한 날짜 (파일 제목형식이 yyyy-mm-dd-title이라면, 생략 가능)    
4. description : 글에 대한 설명  

![screenshot](/assets/img/blog/post-2019-02-01/make-post2.JPG)  

이제 작성한 파일을 git에 commit해야한다.  

**'Git Bash'** 프로그램을 실행한다.  
> cd c:/workspace/simpled2ev/simpled2ev.github.io/webdevelop/_posts  
> git add '2019-02-01-github-make-git-and-jekyll-blog3.md'  
> git commit -m 'add post'  
> git push  

![screenshot](/assets/img/blog/post-2019-02-01/make-post3.JPG)  
30초 ~ 1분 정도 기다리고 나서 사이트에 접속하면, 새로운 글이 생겼을 것이다.  

![screenshot](/assets/img/blog/post-2019-02-01/make-post4.JPG)  



## 3. Markdown 사용 방법
1. 글머리  
```   
# : <h1>  
## : <h2>  
### : <h3>  
#### : <h4>  
##### : <h5>  
###### : <h6>  
```   
<br>

2. 코드블럭  
> '>' 을 이용한 코드블럭  
<br>

3. 한줄 긋기  
---------------------------------------   
```  
* * *  
***  
*****  
- - -  
---------------------------------------     
```   
<br>

4. 이미지 삽입
```   
![screenshot](/assets/img/blog/post-2019-02-01/make-post4.JPG)   
```   
<br>

5. 링크 삽입  
```   
<http://simpled2ev.github.io/>  
```   
