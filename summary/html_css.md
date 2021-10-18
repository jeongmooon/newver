# HTML

## HTML Introduction

https://www.w3schools.com/html/html_intro.asp

- HTML : Hyper Text Markup Language
- 웹 페이지의 내용을 표시하는 언어
  - 웹 페이지의 콘텐츠 표시
    - 텍스트 콘텐츠
    - 멀티미디어 콘텐츠 : 이미지(그림, 사진), 비디오, 오디오
  - 웹 페이지의 구조 표시

## HTML Element

https://www.w3schools.com/html/html_elements.asp

```
<tagname>Contents</tagname>
=> tagname : Contents 종류, 특성 표시 / 구조 표시

<tagname> : 시작태그만 존재
=> Empty Element

빈 요소는 시작태그로만 종료된다는 의미로 self-closing 기호를 사용할 수 있음
<tagname />

- 기본 문법 : 사용하지 않음
- reactjs 라이브러리 : 반드시 사용


포함관계(Nested)
<tag1>
  <tag2>
    <tag3>Contents</tag>
  </tag2>
</tag1>
<tag4></tag4>

tag1 ~ tag2 관계
- tag1은 tag2의 Parent(부모요소)
- tag2는 tag1의 Children(자식요소)

tag1 ~ tag3 관계
- tag1은 tag3의 Ancestor(조상요소)
- tag3은 tag1의 Descendant(자손요소)

tag1 ~ tag4 관계
- tag1(tag4)은 tag4(tag1)의 Siblings(형제요소)

대소문자 구분하지 않음 => 소문자로 쓴는 것이 원칙
```

## HTML Attribute

https://www.w3schools.com/html/html_attributes.asp

- Attribute : 속성
- 추가정보를 제공

```
Ex)

<img src="이미지경로/파일이름" >

<a href="이동경로주소">링크이름</a>

속성이름="정보"
```

## HTML Basic

```
<!DOCTYPE html>
<html>
  <head>
    웹사이트(앱) 관련된 정보
  </head>
  <body>
    웹사이트의 콘텐츠
  </body>
</html>
```

- html 태그의 자식요소 : head, body
- head, body : 형제요소

## HTML TEXT Contents

### HTML Heading

https://www.w3schools.com/html/html_headings.asp

- h : (h)eading - 제목 표시
- h1 ~ h6

### HTML Paragraph

https://www.w3schools.com/html/html_paragraphs.asp

- p : (p)aragraph - 단락 표시

- hr : (h)orizontal (r)ules - 수평선 표시(단락 구분의미가 포함) / 빈 요소

```
<p>단락</p>
<hr />
<p>단락</p>
```

- HTML paragraph display

  - 한 단락안에서 Enter 강제 줄바꿈, space 강제 공백은 적용이 안됨

  ```
  <br /> : line (br)eak / 강제 줄바꿈, 빈 요소

  &nbsp; : (n)on-(b)reak (sp)ace - Entity code / 강제 공백 한 칸
  (& : ampersand)
  ```

### HTML Links

https://www.w3schools.com/html/html_links.asp

- a : (a)nchor
- attribute(속성) : href - (h)ypertext (ref)erence / 링크 연결 주소 정보

```
<a href="https://www.naver.com">네이버</a>
```

- 다른 페이지로 링크 연결
- 같은 페이지에서 상하 이동 - 북마크 기능

  - href에 #만 사용하게 되면 페이지의 처음으로 이동

### HTML Lists

https://www.w3schools.com/html/html_lists.asp

- ul : (u)nordered (l)ist - 순서없는 목록
- ol : (o)rdered (l)ist - 순서있는 목록
- li : (l)ist (i)tem - 항목

- dl : (d)ecription (l)ist - 설명 목록
- dt : (d)ecription (t)itle(theme) - 설명 목록 제목
- dd : (d)ecription (d)ata - 설명 목록 내용

### HTML Talbe

https://www.w3schools.com/html/html_tables.asp
https://www.tablesgenerator.com/html_tables

표 구성 요소 : 열(세로줄), 행(가로줄), 셀(칸)

- table
- thead : 표 구성 영역 - 열제목 영역
- tbody : 표 구성 영역 - 데이터 영역
- tr : (t)able (r)ow - 표의 행
- th : (t)able (h)eader - 열 제목 셀
- td : (t)able (d)ata - 데이터 셀

https://www.tablesgeno

## HTML MULTIMEDIA Contens(Embed Contents)

### HTML Images

https://www.w3schools.com/html/html_images.asp

- img : image - 이미지 파일을 HTML 페이지에 삽입 / 빈 요소
- attribute
  - src : 이미지 파일의 경로/이름 정보
  - alt : (alt)ernative : 대체 텍스트

```
<igm src="이미지파일 경로/이름"alt="이미지 설명글" />
```

### HTML File Paths

https://www.w3schools.com/html/html_filepaths.asp

```
URL
https://www.w3schools.com/html/html_filepaths.asp
https://www.w3schools.com/html/

File 경로
https://www.w3schools.com/html/html_filepaths.asp
```

- 인터넷 주소

  - IP : Internet Portocol - 인터넷에서 사용하는 실제 주소 (192.168.0.1)
  - Domain Name : IP주소를 대체하는 영어로 된 주소체계(www.naver.com)

- 파일 경로 = URL (Uniform Resource Locator)
  - 인터넷에서 사용하는 서버에 저장된 자원의 위치
  - 자세한 인터넷 주소

```
URL
https://codesandbox.io/s/html-css-b14r1?file=/summary/html_css.md

Domain Name
https://codesandbox.io/
```

- 절대주소(URL)
  - File 이나 Resource를 찾거나 이동하기 위한 기준 지점이 서버의 주소(IP, 도메인 주소)
  - 항상 같은 위치를 찾거나 이동할 수 있음

```
<a href="https://github.com/edu-ministori/addinedu_10/"></a>

<img src="https://codesandbox.io/s/html-css-hc9rd?file=/README.md" />
```

- 상대주소(URL)
  - File이나 Resource를 찾거나 이동하기 위한 기준 지점이 이동하거나 찾으려고 하는 파일의 위치
  - 상황이 따라서 경로/주소 표시 형태가 변형될 수 있음

```
<a href="README.md"></a>

../ : 상위폴더

<a href="../">

<img src="summary/images/img.png" />

<img src="images/img.png" />
```

###HTML Video

- video : 저장된 영상 파일을 해당 웹페이지에 삽입

```
<video>
  <source src="영상 경로/이름"type="video/mp4">
<video/>
```

- attribute

  - html5에서 추가된속성
  - name = "value" 형식에서 name만 쓰는 형식으로 변경
  - contrls : 동영상 컨트롤 버튼 표시
  - loop : 반복 재생
  - autoplay : 자동재생
  - muted : 음소거

### HTML Semantic Elements

https://www.w3schools.com/html/html5_semantic_elements.asp

- 영역을 구분하는 태그(요소)를 의미있게 구분하고 영역을 성정하도록하는 요소

> header : 웹페이지 상단영역 - 로고, 로그인, 메듀
>
> nav : (nav)igation : 웹사이트 메뉴
>
> section : 콘텐츠를 담는 영역
>
> aticle : 짧은 글 / 한 내용으로 완성되는 글
>
> aside : 부수적인 내용, 광고
>
> footer : 하단 영역 - 서버 로고, 주소, 연락처, 소유권

### HTML Block & Inline

https://www.w3schools.com/html/html_blocks.asp

- HTML Elementsd의 특성(디자인 개념)

  - Block의 요소

    - 항상 새 줄에서 표시됨(줄 바뀌어서 표시)
    - Block 요소로 만들어지는 영역의 가로길이가 전체 너비에 채워짐
    - div : (div)ision - container 요소

  - Inline 요소
    - 한 줄에 나란히 표시됨(줄 바뀌지 않음)
    - Iinline 요소로 만들어지는 영역의 가로길이가 콘텐츠 크기만큼 만들어짐
    - span : (span)

## HTML ID, Class

https://www.w3schools.com/html/html_id.asp
https://www.w3schools.com/html/html_classes.asp

- HTML Elment에 이름을 지정해주는 attribute

> ID
>
> - 하나의 HTML 문서내에서 고유해야함 : 하나만 존재
> - 하나의 HTML Element에 여러개 ID 이름을 지정할 수 있음
> - 대체적인 데이터을 고유하게 표시할 때 사용

```
<h1 id="heading">제목</h1>
<h1 id="heading">제목</h1>(동일 제목 사용x)

<p id="pargraph">단락</p>
<p id="sentence chapter">단락</p> (사용x)
```

> Class
>
> - 하나의 HTML 문서내에서 여러 Element에 사용할 수 있음
> - 하나의 HTML Element에 여러가지 이름을 사용할 수있음
> - 스타일을 공통 적용, 효과 여러 곳에 동일하게 적용할 때 사용

```
<h1 class="heading">제목</h1>
<h1 class="heading">제목</h1> (사용가능o)

<p class="pargraph">단락</p>
<p class="sentence chapter">단락</p> (사용o)
```

# CSS

## CSS Introduction

https://www.w3schools.com/css/css_intro.asp

- CSS : Cascading Style Sheets

> cascading : 연속적인
>
> 동일한 HTML Element에 대해서 여러가지 스타일링 적용
>
> - 가장 마지막에 적용된 파일이 HTML Element에 적용되어 화면에 표시

## CSS Syntax(문법, 구문)

https://www.w3schools.com/css/css_syntax.asp

- selector(선택자)
- declatrtion(선언)

```
선택자 (선언 - property(속성):value(값): )
```

## CSS Selector(선택자)

https://www.w3schools.com/css/css_selectors.asp

- 스타일링을 할 대상(HTML Element)을 선택

> Simple Selector(단순 선택자)
>
> - name(tag), id, class 3가지를 사용하여 선택지를 표현
>   Combinator Selcetion(복합 선택자)
>
> Psuedo-class(가상 클래스)
>
> Psuedo-element(가상 요소)

### Element(tag) Selector

- 요소의 이름을 선택지로 사용
- 해당 요소를 모두 선택해서 스타일링 적용

```
p()
div()
```

### ID Selctor

```
#HEADING {}
```

### Class Selector

```
.sentence {}
```

> 선택적 연결 표현
>
> - 여러 요소중에 특정 요소를 선택하기 위해서 사용

```
<p id="para">

p#para{}

p.sentence{}

#para.sentence{}
```

## CSS 작성방식

- External : 외부파일
- Internal : html 파일 내부에 작성 style태그 사용
- Inline : html element에 직접 작성

## Color 이론

> 색 혼합 방식
>
> - 가산 혼합 : 빛 혼합
>
>   - 혼합하는 색이 많을 수록 밝아짐; 모든 색을 혼합 => 흰색
>   - 스크린 : 빛의 정보 이용
>   - 칼라모드 : R(ed)G(reen)B(lue)
>
> - 감산 혼합 : 잉크 혼합
>   - 혼합하는 색이 많을 수록 어두워짐; 모든 색을 혼합 => 검은색
>   - 프린트 : 잉크 색을 이용
>   - 컬러모드 : C(yan)M(agten)Y(ellow)(black)K

> RGB 모드
>
> 컴퓨터가 사용하는 숫자 진법 : 2진법(0,1)
>
> 데이터 저장 최소 단위 : bit
>
> - 저장 공간 1칸 : 0.1에 하나를 저장
>   정보 표현 최소 단위 : byte(1byte = 8bit)
>
> RGB 컬러모드
>
> - Red, Green, Blue 각각 1byte씩으로 색 정보 표현
> - 1byte = 8bit => 3byte = 24bit 트루컬러
>
> - CSS에서 색 표현 방식
> - 10진수 표시 방식(0~9)
>   - rgb(150, 200, 56)
> - 16진수 표시 방식(0~9, A~F)
>   - 2진수 4자리 => 16진수 1자리
>   - 2진수 24bit => 16진수 6자리
>   - #1AFFD3

> 컴퓨터 용량 단위
>
> - 1000byte = 1KB
> - 1000KB = 1MB
> - 1000MB = 1GB
> - 1000GB = 1TB

> 투명 모드
>
> - transparent, opacity, alpha
>
> CSS 표현
>
> - opacity : HTML Elment
> - igba : 색의 투명도 조절

## CSS 상속

- 조상요소, 부모요소에 적용된 css style에 자식요소, 자손요소에 상속되어 적용되는 현상

```
-html

<div class="parent">
  <p class="child">단락</p>
</div>

-css
```

## CSS Property Category

- HTML Contents Styling

  - Text Contents
  - Multimedia Contents Styling

- HTML 구조 Styling

### CSS Text

https://www.w3schools.com/css/css_text.asp

> color
>
> 글꼴 색

> text-align
>
> - left, center, right, justify(양쪽맞춤)

> text-decoration : 텍스트 line
>
> - overline, line-through, underline, name

> text-indent : 들여쓰기

> letter-spacing : 자간
>
> - 양수, 음수값 아용 가능

> ling-height : 줄 높이
>
> - 텍스트 높이를 포함한 전체 줄 높이
> - 고정값 : px
> - 배수값 : 단위없이 숫자, 글꼴 크기에 비례

> white-space : 줄바꿈 설정
>
> - wrap(기본), nowrap

### CSS Font

> font-family
>
> - 글꼴 종류 적용
> - 글꼴 종류를 여러개 적용
>   - 순서대로 폰트를 찾아서 적용
> - 폰트는 사용자 컴퓨터에서 찾는 것이 기본

```
p(font-family:"맑은 고딕", 돋움, sans-serif;)

=> 맑은 고딕 폰트를 찾고 있으면 적용, 없으면 돋움 폰트를 찾고 있으면 적용, 없으면 sans-serif(브라우저 기본 폰트) 적용
```

> 폰트 카테고리
>
> - 고딕(sans-serif), 명조(serif)

> 웹 폰트
>
> - font-family 속성은 브라우저에서 렌더링을 할 때 클라이언트에서 폰트를 찾는 기능
> - font 파일을 서버에 저장 후 클라이언트 요청에 따라 Resource를 전송할 때 font 파일도 같이 전송해서 font-family 속성이 전송된 폰트를 사용할 수 있도록 하는 폰트 사용 방식
> - 사용자의 디바이스(client)에 저장된 폰트에 상관없이 서버에 저장된 폰트를 사용하므로 모든 사용자가 동일한 폰트를 사용할 수 있게 해줌
> - 웹에서 사용할 수 있는 형식의 폰트 파일 : woff, eof

> - 웹 폰트 서비스
>   - 개발자가 웹 폰트 파일 변환 작업없이 바로 웹 폰트를 사용할 수 있게 해 줌
>   - 구글 폰트(Google Font) : 영문 (https://fonts.google.com/)
>   - 눈누 폰트(Noonnu) : 한글 (https://noonnu.cc/index)

> font-size
>
> - px로 크기 설정

> font-weight
>
> - font 굵기 : normal/bold, 100 ~ 900 : 100단위 숫자(항상 모든 굵기가 존재하는 것은 아님)

> font-style
>
> - 이탤릭체(기울일꼴)

### CSS links

- 4가지 상태 구분을 해서 각각 스타일링 할 수 있음

```
a:link : 일반 상태
a:visited : 방문한 상태
a:hover : 마우스를 갖다댄 상태
a:active : 마우스 버튼을 누른 상태
```

### CSS list

- 목록에 자동으로 생성되는 기호, 숫자 제거

```
p{
  list-style-type:none;
}
```

### CSS Table

- Table 테두리 속성은 틈이 벌어져 있는 테두리가 기본
- border-collapse:collapse 설정 => 테두리 사이 틈을 제거

## Box Styling

- Box : 네모난 형태 영역, 콘텐츠 => HTML 모든 요소

> Box model(Box에 스타일링 속성의 모음)
>
> - 크기
> - 여백
> - 테두리
> - 배경(추가 속성) : 콘텐츠 영역과 안쪽 여백 영역에만 적용

## height / width

> - auto : default - 값을 지정하지 않았을때 적용되는 값
>   -width : 너비가 부모요소를 기준으로 전체가 채워짐
>   -height : 높이가 시작요소를 기준으로 지정됨
>
> - px : px 단위로 고정된 수칙값 적용
>
> - % : % 단위로 유동적인 수치값 적용 -부모요소를 기준으로 부모요소의 크기가 변경되면 맞춰서 같이 변경됨 => 반응형 웹페이지에 사용
>   - width : 부모 요소를 기준으로 일정 비율만큼 적용
>   - height : 부요 요소를 기준으로 일정 비율만큼 적용, 부모 요소가 auto 일때는 적용되지 않음

### padding

> 개별 적용
> -padding-top
> -padding-right
> -padding-bottom
> -padding-left

> 축약표현
>
> - 값 4개 : 4방향 각각 수치값 적용
> - 값 3개 : top right-reft bottom
> - 값 2개 : top-bottom right-reft
> - 값 1개 : 4방향 전체 균일 적용

### border

- 테두리 스타일 : 굵기 형태 색
- 테두리 방향

```
border: 굵기 형태 색;

bordder: 1px sold red;

border-top: 1px sold red;
border-right: 1px sold red;
border-left: 1px sold red;
border-bottom: 1px sold red;
```

### margin

- 바깥 여백
- 사용 방법 : padding과 같음

## Multimedia Contents Styling

- 배경색, 배경이미지

> 배경색 : backgruon-color
>
> - (R)ed, (G)reen, (B)lue, (A)lpha
> - 색 코드값
>   - 색 이름
>   - 16진수 : #FF{R} KF{G} FF{B}
>   - 10진수 : rgb(200{R:0~255},125{G:0~255}.38{B:0~255})
>   - 10진수 + 투명 : rgba(200,125,38,0,5{A:0-11})

> 배경이미지 : background-image
>
> - url() : 이미지 파일 경로/이름
> - 특징 : 이미지 반복시켜서 영역을 채우는 기본 성질
>
> - 배경이미지 반복 : background-repeat
>   - repeat(default), no-repeat, repeat-x, repeat-y
> - 배경이미지 고정 : background-attachent
>   - fixed : 고정
> - 배경이미지 위치 : background-position
>   - x, y 좌표값 표시

## Box model 과 Block/Inline 관계

- Block 요소는 박스 모델이 제대로 적용
- Inline 요소는 박스 모델이 제대로 적용되지 않음
  - width/height, margin이 적용되지 않음

> 한줄에 여러 박스를 표시하면서, 박스모델도 적용
> inline-block 성질을 사용

### dislpay 속성

> 한줄에 여러박스를 표시하면서, 막스모델도 적용
> inlin- block 성질을 사용

- 박스가 화면에 표시될 때 변경
- 값 : block, inline, inline-block

## Multimedia Contents Styling

> 콘텐츠 크기(이미지, 비디오), 여백 스타일링 => Box Model

## Layout Styling

> 구분 영역(박스) 크기,여백 스타일링 => Box Model
>
> 구분 영역의 배치

### Flex

> display: Flex;
>
> - Flex 에서 적용
>
> flex-direction
>
> - row(default), row-reverse, column, column-resverse
>   flex-wrap
