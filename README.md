# 0814_Web

## 참고 링크

https://codesandbox.io/

https://www.w3schools.com/

https://github.com/edu-ministori/frontend_08

## HTML

### Introduction

https://www.w3schools.com/html/html_intro.asp

> 웹 페이지 구조 표시

> 웹 페이지 컨텐츠 표시
> - 텍스트 컨텐츠
> - 멀티미디어 컨텐츠 : 이미지, 비디오, 오디오 등

### HTML Elements

https://www.w3schools.com/html/html_elements.asp

`(backtick) - 백틱 세개를쓰면 박스가 생김
```
<tagname>Contents</tagname>

* 시작 태그만 있는 경우 : Empty Element
```

> 포함관계(Nested)
```
<html>
  <body>
    <h1>Heading</h1>
  </body>
</html>
```

> html-body-h1 관계
> 
> html : body와 관계 - 부모요소 / h1과 관계 - 조상요소
> 
> body : html과 관계 - 자식요소 / h1과 관계 - 부모요소
> 
> h1 : body와 관계 - 자식요소 / html과 관계 - 자손요소

### HTML Attribute

https://www.w3schools.com/html/html_attributes.asp

### HTML Headings

https://www.w3schools.com/html/html_headings.asp

h1~h6 : 제목태그 (h=heading)

### HTML Paragraph

https://www.w3schools.com/html/html_paragraphs.asp

### HTML Links

https://www.w3schools.com/html/html_links.asp

a=anchor 

> URL=Uniform Resource Locator 파일식별자(위치표시), 가장 넓은 의미의 인터넷 주소
> 인터넷 주소
> - IP (Internet Protocol) : 숫자로 구성된 주소
> - Domain Name : www.naver.com / DNS (Domain Name Server)
> - ex) blog.naver.com/blog/12345 => URL

### HTML File Paths

https://www.w3schools.com/html/html_filepaths.asp

> 절대 vs 상대
> - 경로 위치 표시 방식
> - 경포 표시 기준의 변경 여부 (기본도메인 생략하고 ///만붙는거는 상대, 도메인 전체는 절대)
> - 절대 경로: https://www.naver.com/blog/image.jpg
> - 상대 경로: /blog/image.jpg || image.jpg

### HTML Lists

https://www.w3schools.com/html/html_lists.asp

> 중첩목록 (Nested List)

+ 추가 메모

원페이지에서 위치 이동은 북마크 기능을 이용해서 한다.
북마크를 이용할때는 이동 위치를 id값으로 정의한다.

unordered list > ul
ordered list > ol

ul과 ol 안에는 li (list item) 태그로 한 항목씩 넣는다.
ol 태그를 사용하면 자동으로 1. 2. 3. 으로 순서가 붙는다.

제목태그는 h1~h6 까지있음
숫자가 작을수록 큰제목

a태그를 넣을때는 li 안으로 들어가야함

https://ko.wikipedia.org/wiki/HTMLhttps://ko.wikipedia.org/wiki/HTML

여기에 있는 목차 만들기 연습 (숙제)

### HTML Table

https://www.w3schools.com/html/html_tables.asp

Table Generator : https://www.tablesgenerator.com/html_tables

### HTML Images

https://www.w3schools.com/html/html_images.asp

alt="" > 이미지가 화면에 보이지 않을 때 텍스트로 대신 표현 (=alternative)
img 는 종료태그 없음 (empty element)

### HTML Videos

https://www.w3schools.com/html/html5_video.asp

video 태그 삽입
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
</video>

** controls 도 attribute 이나 =""없이 이름만 쓴다. 기능은 영상에 재생버튼 나타나게 함

비디오에 쓸수있는 어트리뷰트 참고 (주요 controls autoplay muted loop)
https://www.w3schools.com/tags/tag_video.asp

크롬 정책 상 오디오포함 자동재생은 불가 / 영상만 자동재생 가능
-> muted 를 추가하면 자동재생 가능

<video controls autoplay muted loop>
      <source
        src="https://www.w3schools.com/html/mov_bbb.mp4"
        type="video/mp4"
      />
    </video>

### HTML Youtube

https://www.w3schools.com/html/html_youtube.asp

유투브 영상 음소거/자동재생 하는 법
-> 아이프레임 내 유투브 링크 뒤에 ?autoplay=1&mute=1 추가

웹사이트 템플릿 참고 사이트
https://freebiesbug.com/psd-freebies/website-template/


추가 메모

클라이언트 서버 모델


ios 앱 개발 > swift 언어 (front-back 공통)

안드로이드 앱 개발 > kotlin 언어 (구 자바> 현 코틀린)

웹(front) > html(언어,내용), css(디자인), js

서버(back) > php, jsp(자바와 연결), asp, node.js, python


rendering: 서버에서 보낸 소스코드를 브라우저가 해석하여 시각적인 사이트형태로 화면에 보여주는 것


interpreter(언어): 한줄 한줄 소스 번역 php,jsp,asp

*java와 jsp는 다름

compiler(언어): 프로그래밍 언어를 통으로 번역 ex) C,C++,JAVA,C#

*rendering 안에는 interpreting&compiling 작업 불포함


깃허브 md 문법

#(제목)

##(소제목)

###(소제목의 하위)


head: meta info -> 사이트를 설명하는 부수적인 정보 (화면에 보이는 컨텐츠X)

body: 실제 브라우저에 보이는 컨텐츠


종료태그가 없는 태그(=empty element): <br> (노컨텐츠 태그)


조상태그

부모태그

자식태그 (조상태그에서는 자손태그)

*속성유전


attribute 형태 - <시작태그="">


<hr> Horizontal Rules 약자, 수평선 그어주는 태그

<p>랑 같이쓰면 단락만큼 선 생김
  

p태그 안에서 치는 엔터/스페이스바는 여러번 눌러도 공백1칸으로만 인식됨
  

br = (line) break
  
&nbsp; = 공백 한칸 (여러칸 띄우고싶으면 이걸 여러번 넣으면 됨)
  

target="_blank" 새 탭 열기
  
*href 처럼 a 태그 안에다가 넣어서 사용
  
  
### HTML Block & inline
https://www.w3schools.com/html/html_blocks.asp

> 영역의 특성
>
> - 블럭요소 : 가로길이 - 부모요소에 채워짐 / 세로길이 - 자식요소에 맞춰짐
> - 인라인 요소 : 가로길이와 세로길이 모두 자식요소에 맞춰짐
  
> 포함관계

> 블럭요소 : 다른 블럭요소, 인라인 요소, 콘텐츠 포함 가능
> 인라인 요소 : 다른 인라인 요소, 콘텐츠 포함 가능, 블럭요소는 포함 불가능
> 예외 : a - 인라인 요소이지만 블럭 요소를 포함 가능

### HTML Id & Class
https://www.w3schools.com/html/html_id.asp

https://www.w3schools.com/html/html_classes.asp

> id attribute

> id로 붙여주는 이름은 한 HTML 문서내에서 고유해야 함.(한번만 사용)
> id는 한 대상의 HTML Element에 하나의 이름만 지정할 수 있음.
> class attribute

> class로 붙여주는 이름은 한 HTML문서내에서 여러번 중복 사용할 있음.
> class는 한 대상의 HTML Element에 여러개의 이름을 지정할 수 있음.
  
### CSS 상속

> 부모요소에 적용된 CSS 속성이 자식요소에 적용되는 것을 상속이라고 한다.

### Web Font

> 웹에서 사용하는 폰트는 브라우저에서 렌더링 되기 때문에 기존에는 사용자 pc에 설치되어 있는 폰트를 사용
> 사용자 pc에 설치된 폰트를 찾지 않고 서버에 폰트를 저장해서 사용하는 방식 -> 웹폰트 방식

