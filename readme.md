# HTML 되새김 저장소 

![소낼름](https://user-images.githubusercontent.com/89917101/163997346-c6df8d3b-5e83-48ce-8ebc-ec91f7bb09ed.jpg)

```html
<소가 여물먹듯이
  정리한내용들을 
     곱씹으며 적용해보고 
        이해한것들을 저장하는곳>
```
## HTML (Hyper Text Markup Language)
하이퍼텍스트를 마크업 언어로 정의한 웹문서

- `Hyper Text` = 웹문서를 이루고있는 요소하나하나를 하이퍼텍스트라고한다.<br>
- `Markup Language` = 문서가 화면에 표시되는 형식을 나타내거나 구조를 명시하기위한 규칙들을 정의한언어  


 <span style="color : #fff5b1"> ⚡마크업언어와 프로그래밍언어의 차이?</span>

- `마크업언어`&nbsp;:&nbsp;&nbsp;tv를 어디에다 배치할것인지? / 구조를 명시하기위한 언어
- `프로그래밍언어`&nbsp;:&nbsp;&nbsp;tv를 어떻게 동작할것인지? / 시스템이나 소프트웨어를 구동시키기위한 언어

<hr>

## HTML , CSS , JavaScript 의 관계


- `HTML`&nbsp;:&nbsp;&nbsp;방안의 가구를 어떻게 배치할것인지? / 웹문서의 기본적인 골격을 담당
- `CSS`&nbsp;:&nbsp;&nbsp;벽지,가구색은 어떻게할것인지, 어떻게방을꾸밀것인지? / 각요소들의 레이아웃, 스타일링을 담당
- `JavaScript`&nbsp;:&nbsp;&nbsp;내가 어떤행동을했을때 무슨일이발생하는지? / 사용자와의 인터랙션(Interaction:상호작용)을담당
<hr>

## 웹관련 용어
- `웹표준(Web Standards)`&nbsp;:&nbsp;&nbsp;웹사이트에 접속한 사용자가 어떠한 운영체제나 브라우저를 사용하더라도 동일한 결과를 보이게 하기위해 표준적으로 사용되는 기술이나 규칙
- `웹접근성(Web Accessibility)`&nbsp;:&nbsp;&nbsp;웹 접근성은 장애를 가진 사람과 장애를 가지지 않은 사람 모두가 웹사이트를 이용할수 있게 하는 방식
- `웹 호환성(Cross Browsing)`&nbsp;:&nbsp;&nbsp;웹 브라우저버전, 종류와 관계없는 웹사이트 접근 / 웹표준의 준수를 통한 브라우저 호환성확보

<hr>

## HTML 용어
- `Tag`&nbsp;:&nbsp;&nbsp; Html에서 사용되는 명령어의 집합을 태그라고한다.
- `Opening tag`&nbsp;:&nbsp;&nbsp; 여는태그로, 태그의 시작을알리는 태그이다. 
- `Closing tag`&nbsp;:&nbsp;&nbsp; 닫는태그로, 태그의 끝을 알리는 태그이다.
- `Empty elements`&nbsp;:&nbsp;&nbsp;내용이없는 빈요소를 빈요소라 부른다.
- `Content`&nbsp;:&nbsp;&nbsp;태그와 태그사이에 존재하는 내용을 의미한다.
- `Element`&nbsp;:&nbsp;&nbsp; Opening Tag + Content + Closing tag 이다.
- `Nesting`&nbsp;:&nbsp;&nbsp; 요소의 중첩을 의미 / 포함관계를 구분하기위해 들여쓰기를 사용한다
- `Format`&nbsp;:&nbsp;&nbsp; 서식을 의미한다.
- `Formatting`&nbsp;:&nbsp;&nbsp; 서식을 설정하는것을 의미한다.
- `Rendering`&nbsp;:&nbsp;&nbsp;일반적으로 HTML, CSS, JavaScript 코드의 사용을 나타냄


<hr>

## HTML 태그의 사용
- 여는태그 <> 로시작해서 </>닫는태그로 끝마친다.
```html
<p>contents</p>
```
- 빈요소는 요소없이 사용된다.
```html
- 대표적인요소로는 ...

<br> , <hr> , <img> , <input> ,<link> , <meta> 
```
- 태그의 중첩은 들여쓰기로 포함관계(부자관계)를 나타낸다
```html
<div>
  <p></p>
</div>
```
<hr>

## 주석(Comments) 처리
주석은 코드에 메모를 하거나, 혹은 사용하지 않는 코드를 임시로 처리하기 위해 사용한다.
- html에서의 주석은 \<!-- --> 으로 사용된다
- [단축키]&nbsp; 주석처리할 부분을 선택후 Ctrl+/
```html
<!-- <p>이내용은 나타나지않음</p> -->
```
<hr>

## HTML 문서의 구조

- [단축키]&nbsp; !+Tab 으로 html기본 양식을 빠르게 작성할수있다.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```
- `<!DOCTYPE html>`&nbsp;:&nbsp;&nbsp; 문서의 타입을 html이라고 명시 / 생략가능하지만 쓰는것을 권장
- `html`&nbsp;:&nbsp;&nbsp; 페이지 전체의 컨텐츠를 감싸는 루트(root)요소
    - `lang`&nbsp;:&nbsp;&nbsp;웹접근성을위해 무슨언어인지 명시
- `head`&nbsp;:&nbsp;&nbsp; 웹브라우저 화면에 직접적으로 나타나진 않는 웹페이지의 정보
- `meta tag`&nbsp;:&nbsp;&nbsp; 문서의 일반적인 정보와 문자 인코딩을 명시
- `title`&nbsp;:&nbsp;&nbsp; 문서 상단 표시되는 제목을 의미
- `body`&nbsp;:&nbsp;&nbsp; 웹브라우저 화면에 나타나는 모든 콘텐츠

<hr>

## 블록(Block)과 인라인(Inline)
- `블록(Block)`&nbsp;:&nbsp;&nbsp;블록 레벨 요소는 언제나 새로운 줄에서 시작하고, 좌우 양쪽으로 최대한 늘어나 가능한 모든 너비를 차지
- `인라인(Inline)`&nbsp;:&nbsp;&nbsp;바로 이전 요소가 끝나는 지점부터 시작하여, 요소의 내용만큼만 차지<br>
&nbsp;　　　　　　　　인라인 요소는 어느 곳에서나 시작할수있음
> 포함규칙 
- 같은 형태의 다른 요소를 안에 포함할수있음 (블록>블록, 인라인>인라인)
- 대부분의 블록요소는 다른 인라인 요소도 안에 포함할수 있음
- 인라인요소는 블록요소를 포함할수없음

<hr>

## Html 태그
`<h1~h6>`&nbsp;:&nbsp;&nbsp;제목을 정의할때 사용된다. 

# H1 
## H2 
### H3 
#### H4 
##### H5 
###### H6

```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>
```
<hr>

`<p>`&nbsp;:&nbsp;&nbsp; 문단을 나타낼때 사용된다.
- 코드상 다음줄에 작성되더라도 p태그안에있는내용은 줄이 바뀌지않는다.
- 블록 레벨 요소이다.
- [단축키] 의미없는 문장생성 lorem+tab

<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Omnis labore iste porro beatae quia natus voluptate vero atque, minus nemo? Ut assumenda aliquid est accusamus voluptatem laborum, ab ex vero!</p>

```html
<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Omnis labore iste porro beatae quia natus voluptate vero atque, minus nemo? Ut assumenda aliquid est accusamus voluptatem laborum, ab ex vero!</p>
```
<hr>

`<br>`&nbsp;:&nbsp;&nbsp; 개행(줄바꿈)할때 사용된다.
- 문단사이에 여백을 두기위한 용도로 사용하지말것 이경우 \<p>태그로
  감싼후 CSS의 margin 속성으로 여백의 크기를 조절할것

A<br>B C

```html
A<br>B C
```

<hr>

`<q>`&nbsp;:&nbsp;&nbsp;안쪽의 텍스트가 짧은 인용문임을 나타냄 / 인라인 요소임
- 줄바꿈이 없는 짧은경우에 적합
- 인라인 요소이다.

<q>오늘 먹을 치킨을 내일로 미루지 마라</q>

```html
<q>오늘 먹을 치킨을 내일로 미루지 마라</q>
```

<hr>

`<blockquote>`&nbsp;:&nbsp;&nbsp;안쪽의 텍스트가 긴 인용문임을 나타냄 
- 줄바꿈이 필요한 긴경우에 적합
- p태그 안에 작성하면 안된다. / p태그 특성상 자식요소가 블록요소이면 자동으로 p태그가  닫힘처리됨
- 블록요소이다.
- cite 속성으로 출처를 명시할수있다.

<blockquote>B와 D사이에는 무엇이 있을까요? 
그렇습니다 C이죠.
이처럼 출생(Birth)과 죽음(Death)사이에는
치킨(Chicken)이 있습니다.
우리는 세상을 살아가며 많은 선택의 기로에 서게 됩니다. 
후라이드인가 양념인가
뼈있는 치킨일수도 있고
순살치킨일 수도 있습니다.
선택을 하기전 
어떻게하면 잘먹었다고 소문이날까 생각하며 
어떤종류의 치킨을 먹을지 신중히 선택하시기바랍니다.</blockquote>

```html
<blockquote>
B와 D사이에는 무엇이 있을까요? 
그렇습니다 C이죠.
이처럼 출생(Birth)과 죽음(Death)사이에는
치킨(Chicken)이 있습니다.
우리는 세상을 살아가며 많은 선택의 기로에 서게 됩니다. 
후라이드인가 양념인가
뼈있는 치킨일수도 있고
순살치킨일 수도 있습니다.
선택을 하기전 
어떻게하면 잘먹었다고 소문이날까 생각하며 
어떤종류의 치킨을 먹을지 신중히 선택하시기바랍니다.
</blockquote>
```
<hr>

`<pre>`&nbsp;:&nbsp;&nbsp; html에 작성한 내용 그대로 표현 (공백포함)
 - 코드,이모티콘 표현할때 용이함
 - 짧은 코드 표현은 \<code> 사용

<pre>
⊂_ヽ
　 ＼＼  Λ＿Λ
　　 ＼( ‘ㅅ' ) 두둠칫
　　　 >　⌒ヽ
　　　/ 　 へ＼
　　 /　　/　＼＼
　　 ﾚ　ノ　　 ヽ_つ
　　/　/두둠칫
　 /　/|
　(　(ヽ
　|　|、＼
　| 丿 ＼ ⌒)
　| |　　) /
 ノ )　　Lﾉ 
</pre>

```html
<pre>
⊂_ヽ
　 ＼＼  Λ＿Λ
　　 ＼( ‘ㅅ' ) 두둠칫
　　　 >　⌒ヽ
　　　/ 　 へ＼
　　 /　　/　＼＼
　　 ﾚ　ノ　　 ヽ_つ
　　/　/두둠칫
　 /　/|
　(　(ヽ
　|　|、＼
　| 丿 ＼ ⌒)
　| |　　) /
 ノ )　　Lﾉ 
</pre>
```

<hr>

`<figure>`&nbsp;:&nbsp;&nbsp;독립적인 콘텐츠를 표현 
- \<figcaption>요소를 사용해서 설명을 붙일수있음
- 이미지(img) , 코드조각(pre) , 인용문(blockquote) 시(p)등을 감쌀수있음

<figure>
(ㅇㅂㅇ)/)
  <figcaption>손흔드는이모티콘</figcaption>
</figure>

```html
<figure>
(ㅇㅂㅇ)/)
  <figcaption>손흔드는이모티콘</figcaption>
</figure>
```

<hr>

`<hr>`&nbsp;:&nbsp;&nbsp;단독으로 문단과 문단사이를 나눌때 사용(수평선)

<p>치킨</p>
<hr>
<p>피자</p>

```html
<p>치킨</p>
<hr>
<p>피자</p>
```

<hr>

`<abbr>`&nbsp;:&nbsp;&nbsp;약어(abbreviation)를 표현할때 사용 
- 속성 title과 같이쓸 경우 약어 위에 마우스를 올려놓으면 그뜻이 툴팁으로 표시됨

<abbr title="Hyper Text Markup Language">HTML</abbr>

```html
<abbr title="Hyper Text Markup Language">HTML</abbr>
```

<hr>

`<address>`&nbsp;:&nbsp;&nbsp;주소를 나타낼때 사용
- 사람, 단체 , 조직에 대한 연락처 정보표시(주소,연락처)

<address>
  <a href="friedsunfish@gmail.com">friedsunfish@gmail.com</a><br>
  <a href="tel:+82-10-1234-1234">(010) 1234-1234</a>
</address>

```html
<address>
  <a href="friedsunfish@gmail.com">friedsunfish@gmail.com</a><br>
  <a href="tel:+82-10-1234-1234">(010) 1234-1234</a>
</address>
```

<hr>

`<cite>`&nbsp;:&nbsp;&nbsp;인용의 출처를 표시할때 사용
- \<blockquote>,\<q>요소가 가진 저작물의 출처를 표시할때 사용

<p>조선시대에도 치킨이 있었다 <q>신가요록 신료찬요</q>에 기록된 포계라는 음식은 기름에 볶은 닭을 밀가루옷을 입혀 익힌뒤 간장과 참기름 식초등으로 맛을낸 음식이다. 이미 조선시대 사람들도 간장치킨의맛을 알았던것....

<cite>https://namu.wiki/w/%EC%82%B0%EA%B0%80%EC%9A%94%EB%A1%9D</cite></p>

```html
<p>조선시대에도 치킨이 있었다 <q>신가요록 신료찬요</q>에 기록된 포계라는 음식은 기름에 볶은 닭을 밀가루옷을 입혀 익힌뒤 간장과 참기름 식초등으로 맛을낸 음식이다. 이미 조선시대 사람들도 간장치킨의맛을 알았던것....

<cite>https://namu.wiki/w/%EC%82%B0%EA%B0%80%EC%9A%94%EB%A1%9D</cite></p>
```

<hr>

`<bdo>`&nbsp;:&nbsp;&nbsp;텍스트 쓰기 방향을 지정할때 사용
>속성
- dir="ltr"&nbsp;:&nbsp;&nbsp;텍스트를 왼쪽에서 오른쪽으로
- dir="rtl"&nbsp;:&nbsp;&nbsp;텍스트를 오른쪽에서 왼쪽으로

<p>산토끼 토끼야 어디를 가느냐</p>
<p><bdo dir="rtl">산토끼 토끼야 어디를 가느냐</bdo></p>

 
```html
<p>산토끼 토끼야 어디를 가느냐</p>
<p><bdo dir="rtl">산토끼 토끼야 어디를 가느냐</bdo></p>
```

<hr>

`<b>`&nbsp;:&nbsp;&nbsp;다른 부가적인 목적 없이 단순히 굵게 표현
- 중요하지않지만 굵게 표현할때 사용 / 표시의의미
- 굵은 글씨로 표시

<p><b>치킨</b> 먹고싶당 으아아아</p>

```html
<p><b>치킨</b> 먹고싶당 으아아아</p>
```

<hr>

`<strong>`&nbsp;:&nbsp;&nbsp;중대하거나 긴급한 콘텐츠를 나타낼때 사용 
- 중요표시의 의미
- 굵은 글씨로 표시

<p><strong>치킨값인상!</strong> 으아아아</p>

```html
<p><strong>치킨값인상!</strong> 으아아아</p>
```

<hr>

`<i>`&nbsp;:&nbsp;&nbsp;어떠한 이유로 주위와 구분해야하는 경우 사용
- 기술용어, 외국어구절, 등장인물의 생각등 
- 보통 기울임꼴로표시됨 / 구분의의미

<p><i>Life is C(chiken) between B(Birth) and D(Death)</i></p>

```html
<p><i>Life is C(chiken) between B(Birth) and D(Death)</i></p>
```

<hr>

`<em>`&nbsp;:&nbsp;&nbsp;텍스트의 강세를 나타낼때 사용
- 강조의의미

<p>이제 밥먹을 시간이다!<em>치킨!!</em></p>

```html
<p>이제 밥먹을 시간이다!<em>치킨!!</em></p>
```

<hr>

`<mark>`&nbsp;:&nbsp;&nbsp;현재 맥락에 관련이 깊거나 중요해 표시 또는 하이라이트한 부분을 나타낼때사용
- 색깔로 해당부분이 칠해짐
- 연관성표시의 의미

<p><mark>치킨을 먹을때</mark>에 남은뼈가 후라이드였는지 양념이었는지 모르게하라</p>

```html
<p><mark>치킨을 먹을때</mark>에 남은뼈가 후라이드였는지 양념이었는지 모르게하라</p>
```

<hr>

`<small>`&nbsp;:&nbsp;&nbsp;덧붙이는 글이나, 저작권과 법률 표기등의 작은 텍스트를 나타냄
- 책밑부분 어려운 단어의 설명을 표기할때 사용

<p>만병통치킨</p>
<small>만병통치킨:모든병은 치킨으로 치료할수있다</small>

```html
<p>만병통치킨</p>
<small>만병통치킨:모든병은 치킨으로 치료할수있다</small>
```

<hr>

<span style="color : #fff5b1"> ⚡sup,sub 구분요령?</span>

p 머리가 위에가있어서 위첨자요소

b머리가 아래에 가있어서 아래첨자요소

<br>

`<sup>`&nbsp;:&nbsp;&nbsp;거듭제곱의 표시 또는 서수표기시 사용
- 위첨자 요소 / 작게 위쪽에 표시됨

2²
```html
<p>2<sup>2</sup></p>
```

<hr>

`<sub>`&nbsp;:&nbsp;&nbsp;화학식의 원소수표기 , 수학에서의 변수표기시 사용
- 아래첨자요소 / 작게 아래쪽에 표시됨

H₂O
```html
<p>H<sub>2</sub>O</p>
```

<hr>

`<del>`&nbsp;:&nbsp;&nbsp;제거된 텍스트의 범위표시
- 가운데에 취소선으로 표시됨

<del>가운데 취소선</del>

```html
<del>가운데 취소선</del>
```

<hr>

`<ins>`&nbsp;:&nbsp;&nbsp;추가된 텍스트의 범위표시
- 밑줄로 표시됨

<p>가장 맛있는 음식은 <del>통닭</del> <ins>치킨</ins> 이다.</p>

```html
<p>가장 맛있는 음식은 <del>통닭</del> <ins>치킨</ins> 이다.</p>
```

<hr>

`<code>`&nbsp;:&nbsp;&nbsp;짧은 코드 조각을 나타낼때 사용
- 인라인 코드요소
- 긴 코드는 pre태그로 감싸고 code태그로 사용
- 폰트가 다르게 표시됨

<p>자바스크립트 코드의 일부분입니다.</p>
<code>promt("알림창");</code>

```html
<p>자바스크립트 코드의 일부분입니다.</p>
<code>promt("알림창");</code>
```

<hr>

`<kbd>`&nbsp;:&nbsp;&nbsp;키보드입력, 음성입력등을 표시할때 사용

<p>화면전환 = <kbd>alt</kbd>+<kbd>tab</kbd></p>

```html
<p>화면전환 = <kbd>alt</kbd>+<kbd>tab</kbd></p>
```

<hr>

`<a>`&nbsp;:&nbsp;&nbsp;URL로 연결할수있는 하이퍼링크를 만들때 사용
- href 속성을 통해 다른 페이지나 같은페이지의 어느위치, 파일, 이메일주소 등 
>속성

🧩href

href 속성 사용시 경로는 2가지 유형으로 작성가능하다

1.절대경로

  <a href="https://www.mozilla.com">Mozilla</a>

```html
<a href="https://www.mozilla.com">Mozilla</a>
```

2.상대경로

<a href="폴더이름(경로)/이동할파일.html">다른파일</a>

```html
<a href="폴더이름(경로)/이동할파일.html">다른파일</a>
```

🧩target

1. target="_self" / 현재창에서 열림

<a href = "https://www.mozilla.com" target="self">Mozilla</a>

```html
<a href = "https://www.mozilla.com" target="_self">Mozilla</a>
```

2. target="_blank" / 새탭에서 열림

<a href = "https://www.mozilla.com" target="_blank">Mozilla</a>
```html
<a href = "https://www.mozilla.com" target="_blank">Mozilla</a>
```

<hr>

## 엔티티(Entity)

`<`  =  \&lt;

`>`  =  \&gt;

`"`  =  \&quot;

`'`  =  \&apos;

`&` = \&amp;

`빈스페이스` = \&nbsp;

<hr>

## Visual Studio Code 관련
>설치

구글 - Visual Studio Code 검색 - Download - Mac / window 다운로드링크 클릭
>세팅

자동으로 언어팩 설정 문구뜨지않는경우 - 확장(테트리스모양)에서 korean 검색후 다운로드

- `live sever`&nbsp;:&nbsp;&nbsp;웹페이지에서 실시간으로 변경사항을 확인할수있음
- `Auto Rename Tag`&nbsp;:&nbsp;&nbsp;앞부분태그를 수정하면 뒤에태그도 같이 자동으로 수정됨
- `prettier`&nbsp;:&nbsp;&nbsp;들여쓰기나 잘못쓰여진부분 자동으로 수정해줌 (처음에는 습관을위해 사용하지않고 나중에사용)<br>

⚡prettier 사용방법<br>
- 수정범위 드래그후 오른쪽클릭 - 문서서식 - 포맷터선택 prettier<br>

⚡prettier prettier 들여쓰기개수 수정방법<br> 
- `A.` 확장(테트리스모양버튼) - 작은톱니바퀴 확장 설정
- `B.` 왼쪽하단 톱니바퀴선택후 검색 prettier tab 수정

⚡자동 포맷터 사용<br> 
- 설정에서 fomat on save - Format On Save 항목 체크
>단축키


### 🥝 에디터 창 제어

- 현재 창닫기 - Ctrl + w

- 닫은창 다시 열기 - Ctrl + Shift + t

- 사이드바 토글 - Ctrl + b

- 사이드바 탐색기 - Ctrl + Shift + e

- 사이드바 전체검색 - Ctrl + Shift + f 

- 에디터 확대 - Ctrl + +(=)

- 에디터 축소 - Ctrl + -

### 🍉 소스코드 편집

- 들여쓰기 - Tab / 커서있는부분을 기준으로 들여쓰기

  - Ctrl+] / 커서가어디에있든 상관없음

- 내어쓰기 - Shift + Tab

  - Ctrl+[ 

- 아래에 행 삽입 -&nbsp; Ctrl + Enter 

- 위에 행 삽입 - &nbsp; Ctrl + Shift + Enter

- 현재 행 이동 -&nbsp; Alt + ↓/↑

- 현재 행 복사 - &nbsp; Alt + Shift + ↓/↑

- 현재 행 삭제 -&nbsp; Ctrl + Shift + k

- 주석 토글 - &nbsp;Ctrl + /



<hr>

## 기타 용어 정리

- `메타데이터 콘텐츠(Metadata Content)`&nbsp;:&nbsp;&nbsp; 문서의 메타 데이터(정보), 다른문서를 가르키는 링크 등을 나타내는 요소
- `플로우 콘텐츠(Flow Content)`&nbsp;:&nbsp;&nbsp; 웹 페이지상에 메타데이터를 제외하고 거의 모든 요소, 보통 텍스트나 임베디드 콘텐츠를 포함
- `섹션 콘텐츠(Section Content)`&nbsp;:&nbsp;&nbsp; 웹 문서의 구획을 나눌때 사용
- `헤딩 콘텐츠(Heading Content)`&nbsp;:&nbsp;&nbsp;섹션의 제목과 관련된요소
- `프레이징 콘텐츠(Phrasing Content)`&nbsp;:&nbsp;&nbsp;문단에서 텍스트를 마크업 할때 사용 / 구문콘텐츠
- `임베디드 콘텐츠(Embedded Content)`&nbsp;:&nbsp;&nbsp;이미지나 비디오 등 외부 소스를 가져오거나 삽입할 때 사용되는 요소 / 내장 콘텐츠
- `인터랙티브 콘텥츠(Interactive Content)`&nbsp;:&nbsp;&nbsp;사용자와의 상호작용을 위한 컨텐츠 요소 / 대화형 콘텐츠

## 마크다운 작성문법정리

`코드삽입`
\`\`\`+(사용언어 ex) javascript, html)
~ 코드내용 ~
\`\`\`
<hr>
`접기/펼치기 만들기`
<details>
<summary>접기/펼치기</summary>
<div markdown="1">

div 에 markdown attribute 를 1 로 
하는 이유 -> div 안에서 markdown 을 사용하기 위해서 지정함

</div>
</details>

```html
<details>
<summary>접기/펼치기</summary>
<div markdown="1">

 *내용

</div>
</details>
```
