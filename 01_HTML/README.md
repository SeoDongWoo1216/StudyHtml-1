# HTML 기본학습

태그, 요소, 속성에 의미 이해 및 HTML>CSS>JS 작성

-------------------------------------
## 1. 기본태그

* h1 ~ h6: 제목을 적는데 활용하며 1부터 6까지 내려갈 수록 글자크기가 작아짐 <br>
* p: 본문 글을 적는데 활용 <br>
* br: 줄 바꿈 <br>
* hr: 문단 바꿈 <br>
* a href="#" target="@":'HyperText referance'의 약어로 다른 주소를 연결 <br>
@ = "_self": 현재페이지에서 이동 <br>
@ = "_blank": 새창에서 이동 <br>

### + Stylish

* i: 이탤릭체 <br>
* b: 글자 굵게 <br>
* small: 작은 글자 <br>
* sub: 아래 첨자 <br>
* sup: 위 첨자 <br>
* ins: 밑줄 표시 <br>
* del: 취소선 <br> 


### 구현 및 코드
![text_header](/01_HTML/실행화면/text_header.png "기본구성")

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/text_header.html)

-------------------------------
## 2.목록 만들기 

* ul: 순서가 없는 목록
* ol: 순서가 있는 목록
* li: 목록요소 생성
 
 ### 구현 및 코드
![list_test](/# "목록구성")

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
![table_test](/01_HTML/실행화면/table_test.png "테이블구성")

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/table_test.html)

-------------------------------
## 4.미디어 

* img 태그
1. src: 이미지 경로 지정
2. alt: 이미지가 없을 때 나오는 문자
3.width: 너비 height: 높이

* audio,video 태그
1. src: 이미지 경로 지정
2.controls: 제어기 생성
3.(비디오의 경우) .width: 너비 height: 높이
 
 ### 구현 및 코드
![media_test](/01_HTML/실행화면/media_test.png "미디어구성")

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/media_test.html)

-------------------------------
## 5.입력 구성

* form: 입력양식의 내용을 넣을 틀을 만든다.
* input type ="@" name="#" value="데이터값"

@
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
* fieldset /// legend: 속해지는 하부 객체들을 감싸는 틀 생성 /// 내용 작성

 ### 구현 및 코드
![input_test](/01_HTML/실행화면/input_test.png "입력 구성")

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/01_HTML/input_test.html)

-------------------------------

## HTML5 돌아가기

[이전](https://github.com/kg4543/StudyHtml)
