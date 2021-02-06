# JavaScript 기본학습

JavaScript & Jquery를 활용한 반응형 웹 만들기

-----------------------
## 1. 기본구문 및 출력형태

* console.log(); 구문을 활용하여 출력
* 출력화면은 Web의 Console 화면에서 확인가능(하기 사진 참조)
* var @ 를 통하여 변수 지정 가능
* 논리 연산자 활용 가능
  - ! : 부정형
  - && : 둘 다 참이어야 참
  - || : 둘 중 하나만 참이어도 참


### 구현 및 코드
<kbd>![Javascript_Basic](/03_JavaScript/JS_실행화면/first_result.PNG "Javascript_Basic")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test1.html)

-----------------------
## 2. 조건문과 반복문

* 조건문: 하기와 같은 형태로 조건이 참인 경우와 거짓인 경우에 따라 출력값을 다르게 한다.
```
 if (left_val < right_val) {
            console.log("조건이 참인 문장을 실행합니다.");
        }
        else {
            console.log("조건이 거짓인 문장을 실행합니다.");
        }
```
* 반복문: 하기와 같은 형태로 조건을 만족할 때까지 안에 속해있는 구문을 반복 실행한다. 
```
for (var index = 0; index < array.length; index++) {
            console.log(array[index]);
        }
```

### 구현 및 코드
<kbd>![If_for](/03_JavaScript/JS_실행화면/if_for_test.PNG "If_for")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test2.html)

-----------------------
## 3. 함수선언 및 호출

* 함수 선언: function() { }
* 함수 호출: fuction '선언한 함수'('입력값') { } 
                   return 값이 있을 경우 받아옴
```
    <script>
        //함수 선언
        function greeting(name) {
            alert("Hellow World!" + name);
            console.log("숨겨진 로그");
        }

        function f(x) {
            return x*x;
        }
        //함수 호출
        greeting("Go");

        console.log(f(3));
    </script>
```

### 구현 및 코드
<kbd>![function_test](/03_JavaScript/JS_실행화면/function_test.PNG "function_test")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test3.html)

-----------------------
## 4. 문서 객체 선택 및 활용

* 문서객체선택
  - 단수선택
     - document.getElementById("아이디")
     - document.getElementBySelector("선택자")
  - 복수선택
     - document.getElementByName("이름")
     - document.getElementByClassName("클래스")
     - document.getElementBySelectorAll("선택자")

```
    <script>
        //함수 선언
        function greeting(name) {
            alert("Hellow World!" + name);
            console.log("숨겨진 로그");
        }

        function f(x) {
            return x*x;
        }
        //함수 호출
        greeting("Go");

        console.log(f(3));
    </script>
```

### 구현 및 코드
<kbd>![GetElementBy](/03_JavaScript/JS_실행화면/GetElementBy.PNG "GetElementBy")</kbd>

[코드보기1](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test4.html)<br>
[코드보기2](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test5.html)

----------------------
## + 문서객체를 사용한 시간 표시

<kbd>![Clock](/03_JavaScript/JS_실행화면/clock_test.PNG "Clock")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/js_test6.html)

-----------------------
## 5. Jquery를 활용한 문서 객체 선택 및 속성 조작

* $("Selector").method(매개변수,매개변수)
  - $(document).ready(function(){ }); : 문서를 불러와 이벤트를 연결
  - $(Selector).css(): 선택자 스타일 조작
  - $(Selector).attr(): 선택자의 속성 조작
  - $(Selector).text(): 선택자의 텍스트 조작
  - $(Selector).html(): 선택자의 HTML 태그 조작
  
### 구현 및 코드
<kbd>![Clock](/03_JavaScript/JS_실행화면/jquery1.PNG "Clock")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/jquery_test1.html)

<kbd>![Clock](/03_JavaScript/JS_실행화면/jquery2.PNG "Clock")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/jquery_test2.html)

------------------------
## 6. 이벤트
 
* $(Selector).method(function(event){  });
  - $(Selector).hover(function(){  },function(){  }); : 객체 위에 마우스 커서를 올리거나 내리면 이벤트 실행
  - $(Selector).click(function(){  }); : click 시 이벤트 실행
  - $(Selector).keydown(function(){ }); : 키보드를 누를 시 이벤트 실행

### 구현 및 코드
<kbd>![Input_Animation](/03_JavaScript/JS_실행화면/input_animation.PNG "Input_Animation")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/jquery_test4.html)


* $(Selector).on(eventName , event) : 이벤트 연결
* $(Selector).off(eventName , event) : 이벤트 제거
* $(Selector).animate(속성 객체, 시간, 콜백 함수)

### 구현 및 코드
<kbd>![Animation1](/03_JavaScript/JS_실행화면/animation1.PNG "Animation1")</kbd>
<kbd>![Animation2](/03_JavaScript/JS_실행화면/animation2.PNG "Animation2")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/03_JavaScript/jquery_test3.html)

--------------------------------
## 본문으로

[이전](https://github.com/kg4543/StudyHtml)
