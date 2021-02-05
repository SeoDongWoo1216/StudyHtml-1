# CSS 기본학습
CSS를 활용한 기본 구조 및 스타일링 지정

-----------------------
## 1.기본 선택자

* 선택자{스타일 속성: 스타일 값;}

1. 전체 선택자: *로 표기
2. 태그 선택자: 태그 그래도 표기
3. 아이디 선택자: '#id' 형태로 표기
4. 클래스 선택자: '.class' 형태로 표기
5. 자손 선택자: 선택자 > 선택자
6. 후손 선택자: 선택자 선택자

### 구현 및 코드
<kbd>![selector_id](/02_CSS/CSS_실행화면/selector_id_test.PNG "기본선택자")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_id_test.html)

[HTML_6장_참고](https://github.com/kg4543/StudyHtml/tree/main/01_HTML)

-----------------------
## 2.반응/상태/구조 선택자
* 반응선택자
1. :active : 마우스로 클릭 시 이벤트 발생
2. :hover : 마우스 커서가 올라가면 이벤트 발생

* 상태선택자(input 태그에 사용)
1. :checked: check 상태의 input 태그 선택
2. :focus: 현재 focus 상태의 input 태그 선택
3. :enabled: 사용가능한 상태의 input 태그 선택
4. disabled: 사용불가능 상태의 input 태그 선택

### 구현 및 코드
<kbd>![selector_child](/02_CSS/CSS_실행화면/selector_child_test.PNG "반응&상태")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_child_test.html)

* 구조선택자
1. :first-child: 형제 관계에서 첫번째
2. :last-child: 형제 관계에서 마지막
3. :nth-child(n): 형제관계에서 'n-1'번째
4. :nth-last-child(n): 형제관계에서 거꾸로 'n-1'번째    

### 구현 및 코드
<kbd>![selector_struct](/02_CSS/CSS_실행화면/selector_struct_test.PNG "구조")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_struct_test.html)

## HTML5 입력 태그

[이전](https://github.com/kg4543/StudyHtml)

