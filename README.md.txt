# 프로젝트 소개

## 국밥여지도

국밥을 사랑하는 사람들이 모여 국밥을 더 재밌고 알차게 즐길 수 있습니다!

특정 국밥 메뉴(굴국밥, 돼지국밥 등)를 판매하는 내 위치 주변의 식당 정보와
내가 좋아하는 국밥을 맛있게 즐기는 나만의 레시피 정보를 공유해보세요 :)

![국밥여지도logo](https://user-images.githubusercontent.com/80900915/140594405-631a3712-421e-4549-92b6-feeb3aa0cea2.png)

http://hyeonjun.shop/

##  1.제작 기간 & 팀원 소개

2022.03.07 ~ 03.10
- 유현준
- 안대륜
- 김예림

## 2. 시연 연상 

[![가벼운식탁](https://img.youtube.com/vi/96KFZ_nZlzk/0.jpg)](https://youtu.be/96KFZ_nZlzk)

## 3. 초안
▼아래 링크를 눌러 
![](https://media.vlpt.us/images/kr4460/post/8f14b048-e64c-445e-b66a-476fd73cc706/%EC%8A%AC%EB%9D%BC%EC%9D%B4%EB%93%9C1.JPG)

## 4. 사용 기술

* Server: AWS EC2 (Ubuntu 18.04 LTS)
* Framework: Flask (Python)
* Database: MongoDB
* front-end : HTML5, CSS3, Javascript, jquery, bootstrap

## 5. 핵심 기능

* 로그인/회원가입
  - 아이디 중복확인 기능
  - 회원가입시 아이디, 비밀번호 유효성 검사
  
* 메인페이지
   * 카드출력 (필터)
     <br>키워드 클릭 시 카드출력
   * 상세페이지 이동
     <br>카드 클릭 시 해당 상세페이지 이동
   * 스크롤 top 버튼
     <br>누르면 페이지 상단으로 이동
     
* 상세페이지
    * 댓글기능
     <br>로그인한 사용자만 댓글 작성가능
     <br>클릭한 메뉴별 댓글 불러오기

## 6. trouble shooting

<details>
    <summary>
        웹 스크래핑한 db와 댓글을 저장하는 db가 달라 /detail page에 원하는 댓글을 불러오기 어려운 문제
    </summary>
    <div markcown="1">
        detail page에 jinja2 템플릿을 사용해 불러온 데이터를 post를 이용해 댓글과 detail page정보를 함께보내 불러오기 해결
    </div>
</details>

<details>
    <summary>
        쿠키 path 설정 문제
    </summary>
    <div markcown="1">
        메인페이지에서 상세페이지로 넘어갈 때 로그인정보가 없다는 에러가 떠서 상세페이지로 이동할 수가 없었다.<br/>
        원인은 로그인 성공시 받은 token을 쿠키에 저장할 때 path경로 설정이 잘못되어서 쿠키를 메인페이지에만 사용할 수 있게 되어있었기 때문이었고 path경로를 재설정하니 해결되었다.
    </div>
</details>

<details>
    <summary>
        카드별로 해당하는 상세페이지를 나타낼 때 id값으로 상세정보를 가져오는 방법
    </summary>
    <div markcown="1">
        mongodb의 id값을 이용할 때 objectID()를 이용해서 가져오면 해결
    </div>
</details>

<details>
    <summary>
        bootstrap의 템플릿을 이용하니 메인페이지 카드의 정렬이 되지 않음
    </summary>
    <div markcown="1">
        템플릿을 없애고 직접 css로 모양을 잡아 flex로 정렬함
    </div>
</details>