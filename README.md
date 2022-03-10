# hanghae99_6th_week1_team12
# 프로젝트 소개
## 국밥여지도
국밥을 사랑하는 사람들이 모여 국밥을 더 재밌고 알차게 즐길 수 있습니다!
특정 국밥 메뉴(굴국밥, 돼지국밥 등)를 판매하는 내 위치 주변의 식당 정보와<br/>
내가 좋아하는 국밥을 맛있게 즐기는 나만의 레시피 정보를 공유해보세요 :)
![국밥여지도logo](https://user-images.githubusercontent.com/101086604/157632341-f0b3bf12-d24d-4f83-9ccb-b0785379ebbc.png)
http://hyeonjun.shop/
##  1.제작 기간 & 팀원 소개
2022.03.07 ~ 03.10
- 유현준
- 안대륜
- 김예림
## 2. 시연 연상 
[![국밥여지도영상](https://i.ytimg.com/an_webp/Jch7Okq-Whc/mqdefault_6s.webp?du=3000&sqp=CIDxppEG&rs=AOn4CLAMGi6bchbLpe8R0nHfYaBLHiW2Wg)](https://www.youtube.com/watch?v=Jch7Okq-Whc)
## 3. 초안
▼아래 링크를 눌러 주세요
![국밥여지도초안](https://velog.io/@kr4460/%ED%95%AD%ED%95%B4-99-6%EA%B8%B0-1%EC%A3%BC%EC%B0%A8-12%EC%A1%B0-S.A)
## 4. 사용 기술
- Hosting - AWS EC2 </br>
- Backend - Python(Flask, jinja2), JWT </br>
- Frontend - HTML / CSS / JavaScript(Ajax) </br>
- DB - mongoDB </br>
## 5. api 리스트
![국밥여지도 api 리스트](https://user-images.githubusercontent.com/101086604/157633596-a01cf3ce-34c1-4bb7-8ec2-160652060be9.PNG)
## 6. 구현 기능
1. 모바일 반응형 웹 디자인 구현
2. 로그인/회원가입 기능 구현
- Hash함수 이용한 회원가입
- ID 중복확인
- PW 일치 확인
- 입력 정보 중 공란 및 DB 내 중복된 정보가 있을 시 Alert.
- JWT 토큰 이용하여 로그인 구현
- 로그인 버튼 클릭 시, 발급된 JWT 토큰으로 DB에서 유저 정보 확인 후 메인 페이지로 이동
3. 로그인 정보에 따라 다음 기능 구현</p>
&gt;  1 메인페이지
- 메인 페이지에서 메뉴 클릭 시, 해당 메뉴에 대한 상세페이지로 이동(Jinja2)
- 메인 페이지에 닉네임 표출(Jinja2)
- 로그아웃 시 로그인 페이지로 이동.</p>
&gt;  2 상세 페이지
- 상세 페이지에서 유저의 주소 정보 기반 해당 메뉴를 판매하는 국밥집을</br>
  카카오맵API에서 검색 및 지도 마커, 검색목록 표출(Jinja2/kakaoMap API, Ajax)
- 리뷰 등록/표출 구현 (Ajax, mongoDB)
- 리뷰 존재 여부에 따라, 리뷰 리뷰 목록의 text 변경.
## 7. 팀원 별 리뷰
<details>
    <summary>
        유현준
    </summary>
    <div markcown="1">
        웹프로젝트를 완성시키는 것도 처음이지만, 팀장으로서 이를 리드하는 것은 더더욱 처음이었기 때문에, 아직도 팀원 모두가 유의미하게 성장하는데 많이 보탬이 되지 못했던 것 같아, 많은 아쉬움이 남는다. 그럼에도 불구하고, 갑작스런 웹 미니 프로젝트를 통해, '개발'이란 작업은 완벽하게 개념을 숙지하고 뛰어드는 작업이 아니라, 문제를 실시간으로 해결해가면서 개념을 숙지하고, 배워나가는 작업이라는 것을 뼈저리게 느낄 수 있었다. 그리고 개발자 간에 협업을 어떻게 하는 것이 좋을지 많은 고민을 남게 한 시간이었다. 개인적으로, 깃헙을 잘 활용하는 법을 좀 더 배워야겠다.
    </div>
</details>
<details>
    <summary>
        안대륜
    </summary>
    <div markcown="1">
        1주차 미니프로젝트를 진행하는 동안 벽을 느끼게되었고 ,시작전에 더 철저히 준비해서 올껄 이라는 후회와 제 실력이 너무나 부족함을 깨닫게 되었습니다 그러면서 자연스럽게 팀원분들을 의지하게되어 죄송한마음이 컸었고, 이번에 일단 한번 프로젝트를 준비하면서 부딪쳐본것을 경험삼아 포기하지 않고 얼른 나도 성장해서 다음 프로젝트에서는 2인분이상해서 팀원들을 커버할수있는실력을가지기위해 잠을 더줄이고 열심히 하기로 결심하게되었습니다..
    </div>
</details>
<details>
    <summary>
        김예림
    </summary>
    <div markcown="1">
        시작전에 많은 공부를 하고 했으면 좋았을 것이라고 생각했다. 그리고 가장 중요한 것은 협업하는 툴을 잘 다루는 법을 배워서 잘 커뮤니케이션 하는 것이 중요하다는 생각이 들었다. 기여한 바가 작지만 그래도 팀장님께서 하드캐리해주신 덕분에 프로젝트를 잘 끝낼 수 있어서 감사하다. 
    </div>
</details>