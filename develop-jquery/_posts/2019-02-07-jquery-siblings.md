---
layout: post
author: author1
title: [ jQuery ] Siblings
date: 2019-02-07 15:17:05 -0600
description: >
  형제 요소를 찾는 함수 Siblings 사용법
---
# [ jQuery ] Siblings - 형제 요소를 찾는 함수 사용법
## Siblings
jQuery에서 자주 사용하는 Siblings는 자신을 제외한 형제 요소들을 찾는 함수이다.  
나의 경우, 형제 객체들에 class를 추가하거나 삭제할 때 많이 이용한다.  
사용법은 아래와 같다.  
<br>  
> 객체.siblings( [selector] )

<br>  

```c
<ul>   
     <li>list item 1</li>   
     <li>list item 2</li>   
     <li class="third-item">list item 3</li>   
     <li>list item 4</li>   
     <li>list item 5</li>   
</ul>
```
<br>

이런 코드가 있을 때, 클래스가 'third-item'의 형제 요소를 찾으려고한다.  
아래와 같이 작성한다면, list item1 부터 list item 5 까지 third-item을 제외하고 요소를 가져온다.  
```c
$("li.third-item").siblings()
```

활용법은 다음과 같다.  
ex 1. 'third-item'을 클릭했을 때, 다른 li들의 색상을 변경하는 법  

```c
$(".third-item").click(function() {  
  $(this).siblings().css("background-color", "red");  
});
```

ex 2. 'third-item'의 형제요소들의 개수를 가져오는 법  
```c
$(".third-item").siblings().length
```

<br>

참고 사이트 : <https://api.jquery.com/siblings/>
