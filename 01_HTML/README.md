# HTML 기본학습

태그, 요소, 속성에 의미 이해 및 CSS & JavaScript를 활용할 HTML 작성

-------------------------------------
## 1. 기본태그

* h1 ~ h6: 제목을 적는데 활용하며 1부터 6까지 내려갈 수록 글자크기가 작아짐
* p: 본문 글을 적는데 활용
* br: 줄 바꿈
* hr: 문단 바꿈
* a href="#" target="@":'HyperText referance'의 약어로 다른 주소를 연결
 1. _self: 현재페이지에서 이동
 2. _blank: 새창에서 이동

### + Stylish

* i: 이탤릭체
* b: 글자 굵게
* small: 작은 글자
* sub: 아래 첨자
* sup: 위 첨자
* ins: 밑줄 표시
* del: 취소선 


### 구현 및 코드
<kbd>![text_header](/01_HTML/HTML_실행화면/text_header.png "기본구성")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/text_header.html)

-------------------------------
## 2.목록 만들기 

* ul: 순서가 없는 목록
* ol: 순서가 있는 목록
* li: 목록요소 생성
 
 ### 구현 및 코드
<kbd>![list_test](/01_HTML/HTML_실행화면/list_test.PNG "목록구성")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/list_test.html)

-------------------------------
## 3.테이블 만들기 

* table: 표만들기
* tr: 행(row) 삽입
* th: 첫 제목 셀 삽입
* td: 일반 셀에 내용 삽입
<br> \+ th,td colspan="@": @만큼 옆으로 확장
<br> \+ th,td rowspan="@": @만큼 아래로 확장
 
 ### 구현 및 코드
<kbd>![table_test](/01_HTML/HTML_실행화면/table_test.PNG "테이블구성")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/table_test.html)

-------------------------------
## 4.미디어 

* img + @
 1. src: 이미지 경로 지정
 2. alt: 이미지가 없을 때 나오는 문자
 3. width: 너비 height: 높이

* audio,video + @
 1. src: 이미지 경로 지정
 2. controls: 제어기 생성
 3. (비디오의 경우) .width: 너비 height: 높이
 
 ### 구현 및 코드
<kbd>![media_test](/01_HTML/HTML_실행화면/media_test.PNG "미디어구성")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/media_test.html)

-------------------------------
## 5.입력 구성

* form: 입력양식의 내용을 넣을 틀을 만든다.
* input type ="@" name="#" value="데이터값"
1. text: 입력창을 만든다.
2. passward: 표기 시 패스워드형태로 표현되는 입력창을 만든다.
3. file: 첨부파일 기능 생성
4. checkbox: 복수 선택이 가능한 box 생성
5. radio: 복수 선택이 불가능한 box 생성(동일 name="#" 지정)
6. hidden: 보이지 않는 input값 생성
7. button: 일반 버튼 생성
8. reset: 재시작 버튼 생성
9. submit: 제출 버튼 생성

* select: 리스트 박스 생성
 /+ option: 리스트박스에 들어갈 내용 생성
* fieldset / legend: 속해지는 하부 객체들을 감싸는 틀 생성 / 내용 작성

 ### 구현 및 코드
<kbd>![input_test](/01_HTML/HTML_실행화면/input_test.PNG "입력 구성")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/input_test.html)

-------------------------------
## 6.공간 분할 

* div 블록형식으로서 전체 공간분할
* span 인라인형식으로서 글자가 들어간 만큼만 공간분할

* 시맨틱 태그를 활용한 시맨틱 웹
  - 특정태그에 의미를 부여한 웹
  - 공간을 구분하여 의미를 부여 (하기 사진참조)
  
 ![div](/01_HTML/images/공간분할.PNG "공간분할")
 
 ### 구현 및 코드
<kbd>![space_test](/01_HTML/HTML_실행화면/space_test.PNG "공간분할")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/space_test.html)

-------------------------------
## 7.CSS 활용  
* 내부 스타일시트 적용
```
<!DOCTYPE html>
<html>
    <head>
        <title>
            세번째 웹페이지
        </title>
            <style>
                h1 {
                    color: whitesmoke;
                    background-color: black;
                }
                p{
                    color: red;
                    font-weight: bold;
                    font-style: italic;
                }
            </style>
    </head>
    <body>
        <h1>Hello world</h1>
        <p>내용입니다</p>
    </body>
</html>
```
* 외부 스타일시트 적용
 ```
 <!DOCTYPE html>
<html>
    <head>
        <title>
            두번째 웹페이지
        </title>
         <link rel ="stylesheet" href="styles/style.css" />
    </head>
    <body>
        <h1>Hello world</h1>
        <p>내용입니다</p>
    </body>
</html>
```
 ### 구현 및 코드
<kbd>![css_style](/01_HTML/HTML_실행화면/css_test.PNG "css_style")</kbd>

[내부 적용 코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/script_test.html)

[외부 적용 코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/css_test.html) / 
[외부 CSS 코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/styles/style.css)

[CSS 상세](https://github.com/kg4543/StudyHtml/tree/main/02_CSS)

-------------------------------
## Practice 
<kbd>![Practice](/01_HTML/HTML_실행화면/practice.PNG "Practice")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/form_practice.html)


-------------------------------
## 본 문서 돌아가기

[이전](https://github.com/kg4543/StudyHtml)
