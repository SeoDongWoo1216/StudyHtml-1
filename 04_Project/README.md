## Project 상세

### 전체레이아웃
<kbd>![결과1](/04_Project/Project_실행화면/Result_01.JPG "전체레이아웃")</kbd>

--------------------------------------
### Main_header
<kbd>![main_header](/04_Project/Project_실행화면/main_header.PNG "main_header")</kbd>

* CSS
```
  #main-header {
    height: 40px;
    background-color: #faf7f7;
    position: relative;
}
```
---------------------------------------
### 제목
<kbd>![제목](/04_Project/Project_실행화면/제목.PNG "제목")</kbd>

* HTML
```
<h1 class="header-title">Interest</h1>
```
* CSS
```
.header-title {
    position: absolute;
    width: 200px;
    height: 40px;
    left: 50%;
    margin-left: -100px;
    background-image: url('../images/logo.png');
    background-repeat: no-repeat;
    text-indent: -9999px;
}
```
------------------------------------------
### 검색창
<kbd>![검색창](/04_Project/Project_실행화면/검색메뉴.PNG "검색창")</kbd>

* HTML
```
<div class="header-search-form">
            <form>
                <input type="search" class="input-search">
                <input type="submit" class="input-submit" value="검색">
            </form>
        </div>
```

* CSS
```
.header-search-form {
    float: left;
    padding: 7px;
}

.input-search {
    display: block;
    float: left;
    background-color: #ffffff;
    border: 1px solid #cccccc;
    border-radius: 15px 0 0 15px;
    box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.5);
    width: 120px;
    height: 26px;
    padding: 0 0 0 10px;
    font-size: 12px;
    color: #555555;
}
.input-submit {
    display: block;
    float: left;
    width: 50px;
    height: 26px;
    border-radius: 0 15px 15px 0;
    border: 1px solid #cccccc;
    margin-left: -1px;
}

.input-search:focus {
    border-color: rgba(82, 168, 236, 0.8);
    outline: 0;
    box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.5);
} 
```
-------------------------------------
### 상단 메뉴
<kbd>![상단_메뉴](/04_Project/Project_실행화면/outer_menu.PNG "상단_메뉴")</kbd>

* HTML
```
<div class="header-menu">
            <ul class="outer-menu">
                <li>
                    <a href="#">정보</a>
                    <ul class="inner-menu">
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                    </ul>
                </li>
            </ul>
            <ul class="outer-menu">
                <li>
                    <a href="#">사용자</a>
                    <ul class="inner-menu">
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                        <li><a href="#">데이터</a></li>
                    </ul>
                </li>
            </ul>
        </div>
```

* CSS
```
.outer-menu {
    float: left;
    width: 100px;
    height: 20px;
    line-height: 20px;
    padding: 10px 0;
    position: relative;
    text-align: center;
    font-size: 13px;
    font-weight: bold;
    z-index: 9999;
}

.outer-menu:hover {
    background-color: #e1dfe1;
}

.inner-menu {
    display: none;
    background: #ffffff;
    margin-top: 10px;
    width: 100%;
    border-top: 1px solid #cccacc;
    box-shadow: 0 2px 4px rgba(34, 25, 25, 0.5);
}

.inner-menu a {
    display: block;
    padding: 5px 10px;
    z-index: 5000;
}

.inner-menu:hover {
    background-color: #e1dfdf;
}
```

* jQuery
```
 $(".outer-menu").hover(function () {
                $(this).find(".inner-menu").css("display", "block");
            }, function () {
                $(this).find(".inner-menu").css("display", "none");
            });
```
------------------------------
### Navigation 메뉴
<kbd>![Navigation](/04_Project/Project_실행화면/main_navigation.PNG "Navigation")</kbd>

* HTML
```
    <nav id="main-navigation">
        <ul>
            <li><a href="#">Following</a></li>
            <li><a href="#">Categories</a></li>
            <li><a href="#">Everything</a></li>
            <li><a href="#">Popular</a></li>
            <li><a href="#">Gift</a></li>
        </ul>
    </nav>
```

* CSS
```
#main-navigation {
    height: 30px;
    background-color: #faf7f7;
    border-top: 1px solid #cfcaca;
    box-shadow: 1px 3px 3px rgba(34, 25, 25, 0.4);
}

#main-navigation>ul {
    overflow: hidden;
    text-align: center;
}

#main-navigation>ul>li {
    display: inline;
    padding: 0 5px;
    line-height: 30px;
    font-size: 13px;
    color: #524d4d;
    text-shadow: 0 1px 1px white;
}

#main-navigation>ul>li:hover {
    background: #e1dfdf;
    border-radius: 2px;
}
```
-------------------------------------
### Main_Section
<kbd>![main_section](/04_Project/Project_실행화면/main_section.PNG "main_section")</kbd>

* CSS
```
#main-section {
    width: 90px;
    margin: 0 auto;
}

@media (max-width: 919px) {
    #main-section {
        width: 690px;
    }
}

@media (min-width: 920px) and (max-width: 1149px) {
    #main-section {
        width: 920px;
    }
}

@media (min-width: 1150px) and (max-width: 1379px) {
    #main-section {
        width: 1150px;
    }
}

@media (min-width: 1380px) {
    #main-section {
        width: 1380px;
    }
}
```

* jQuery
```
<script src="js/masonry.pkgd.min.js"></script>
<script src="js/imagesloaded.pkgd.min.js"></script>

$(document).ready(function () {
$("#main-section").imagesLoaded(function () {
                $("#main-section").masonry({
                    itemSelector: ".paper",
                    columWidth: 230,
                    // isAnimated: true
                });
            });
           });
```

---------------------------
### Paper
<kbd>![paper](/04_Project/Project_실행화면/paper.PNG "paper")</kbd>

* HTML
```
        <div class="paper">
            <div class="paper-holder">
                <a><img width="190" src="images/nintendo/대난투.jpeg"></a>
            </div>
            <p class="paper-description">슈퍼마리오 대난투<br><a href="http://prod.danawa.com/info/?pcode=6215762">$51</a></p>
            <div class="paper-content">
                <a class="paper-link" href="#">
                    <img src="https://placekitten.com/30/30">
                </a>
                <p class="paper-text">'스매시(스틱 튕기기)'를 중심으로 한 조작 시스템의 체계와 기본 게임 
                시스템의 대부분은 이미 이 시점에서 확립되어 있었다. 이후 작품에도 몇 시스템이 추가되지만, 
                이 시점에서 정해진 시스템에 관해서는 이후에도 거의 변경되지 않는다.</p>
            </div>
```

* CSS
```
.paper {
    width: 190px;
    margin: 3px;
    /* margin-top: 10px; */
    padding: 15px 15px 0;
    font-size: 11px;
    background: #ffffff;
    box-shadow: 0 1px 3px rgba(34, 25, 25, 0.4);
    border-radius: 10px;
}

.paper-holder img{
    border-radius: 7px;
}

.paper-description {
    margin: 10px 0;
}

.paper-content {
    margin: 10px -15px 0 -15px;
    padding: 10px 15px;
    background: #f2f0f0;
    overflow: hidden;
}

.paper-link {
    display: block;
    float: left;
}

.paper-text {
    float: left;
    width: 150px;
    margin-left: 10px;
}
```

* jQuery
```
$(document).ready(function () {
$(".paper").click(function () { showLightBox(this); });
                              });
             
        function showLightBox(obj) {
            var img_src = obj.getElementsByTagName("img")[0].src;
            $("#random_image").attr({
                src: function () {
                    return img_src; 
                   }
            });
            $("#darken-background").show();
            $("#darken-background").css("top", $(window).scrollTop());
            $("body").css("overflow", "hidden");
        }
         //그리드내 이미지 클릭해서 '팝업레이아웃' 보이게 하기
        //선택한 이미지 주소 전달
```
-------------------------------------
### 팝업레이아웃
<kbd>![결과2](/04_Project/Project_실행화면/Result_02.JPG "팝업레이아웃")</kbd>

* HTML
```
<div id="darken-background">
        <div id="lightbox">
            <div class="user-information">
                <a class="user-information-image" href="#">
                    <img src="https://placekitten.com/30/30">
                </a>
                <div class="user-information-text">
                    <h3>User</h3>
                    <p id="random_text">바꿔보자</p>
                </div>
            </div>
            <hr class="lightbox-splitter">
            <img id="random_image" src="#" width="600">
        </div>
    </div>
```

* CSS
```
#darken-background {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 100%;
    display: none;
    background: rgba(0, 0, 0, 0.9);
    z-index: 10000;
    overflow-y: scroll;
}

#lightbox {
    width: 700px;
    margin: 20px auto;
    padding: 15px;
    border: 1px solid #333333;
    border-radius: 5px;
    background: white;
    box-shadow: 0 5px 5px rgba(34, 25, 25, 0.4);
    text-align: center;
}

.user-information {
    overflow: hidden;
    text-align: left;
}

.user-information-image {
    float: left;
    width: 70px;
}

.user-information-text {
    float: right;
    width: 620px;
}

.lightbox-splitter {
    margin: 10px 0;
}
```

* jQuery
```
$(document).ready(function () {
$("#darken-background").click(function () { hideLightBox() });
$("#lightbox").click(function (event) { event.stopPropagation() }); //(사진영역을 눌러도 꺼지지 않게함)
                               });
  
        function hideLightBox() {
            $("#darken-background").hide();
            $("body").css("overflow", "auto");
        }
```
--------------------------------
## 본문으로

[이전](https://github.com/kg4543/StudyHtml)
