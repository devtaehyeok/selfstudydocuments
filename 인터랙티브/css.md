# CSS 레이아웃 기초

div
section

span
img

각각 공통점이 있음.

css display 속성이 다르기 때문

div는 꽉 참 display : block; box
span은 자기 영역만 display : inline -> 크기 조절 불가능

레이아웃은 박스로 div 만듬.
2단 3단 컬럼
태그로는 div section article header footer nav

span {
    dislpay : inline-block;



}

block, inline, inline-block, none
flex 

max-width : 1000px

css box model 기본
![](/images/css/css_223133.png)

![](/images/css/css_223244.png)

border-box 최신 브라우저만 지원함.
패딩 보더가 포함됨 width, height

아무것도 없는 형태로 만들기 css reset

eric myer

display-block 알아서 화면에 맞게 채워줌
스크롤 안생김
디스플레이 블록 엘리먼트를 적당히 쌓아준다
margin 0 border 0 패당 5%
width 하면 가로 스크롤이 생길 수 있음
100에 패딩 5%생기면 스크롤 생김

rem root em 디폴트를 쓰겠다. 기본적으로 브라우저 16px