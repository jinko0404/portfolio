# 고진석 포트폴리오

## 😃Intro
안녕하세요, "지속적인 학습과 실천을 통해 성장하는 개발자" 고진석 입니다. 웹개발에 대한 열정을 가지고 있으며, 
사용자 친화적인 사이트를 제작하고 운영하는 개발자가 되는 것을 목표로 하고 있습니다.

## 🗂Project
제가 진행해왔던 프로젝트입니다.
팀장으로써 프로젝트를 진행할 때는 프로젝트의 일정 관리, 팀원들의 의견 조율 등의 경험을 할 수 있었으며
팀원으로써 팀장의 지시나 요구사항에 따라 프로젝트를 진행을 하는 등의 경험을 쌓을 수 있었습니다.

### 🛫1. Are You T(rip mate)?
* 여행 동행 친구 모집 사이트(KH정보교육원 - 1조 팀프로젝트)
  - 프로젝트 상세 설명 : [https://github.com/2311PublicDataWebApp/AreYouT.git](https://github.com/2311PublicDataWebApp/AreYouT)
  - 개발 기간 : 2024년 2월 15일 ~ 2024년 2월 26일
  - 담당 역할 : 팀장, MVC패턴을 활용한 관리자 기능(회원 관리, 1대1 문의쪽지함, 쪽지 관리, 게시판 관리) 구현, JSP를 통한 웹 페이지 제작
* Back-End
  - 사용 언어: JAVA
  - 사용 기술: Spring FrameWork, OracleDB
* Front-End
  - 사용 언어: JavaScript/CSS/HTML
  - 사용 기술: BootStrap, JQuery
* 기능구현
  - 관리자 페이지
    ![image](https://github.com/2311PublicDataWebApp/AreYouT/assets/152952078/f1db10f9-66d8-49fd-8536-68f670ac1680)
    * 체크 된 회원을 한번에 일괄적으로 묶어서 블랙리스트에 등록 할 수 있도록 구현
      1)	체크된 회원 없이 블랙리스트 등록을 시도할 경우
        - 회원값을 저장하는 배열의 길이가 0이므로 “체크된 회원이 없습니다.” 메세지 출력
      2)	블랙리스트 등록 성공
        - 체크된 회원의 목록이 저장된 배열을 구분자 “,”으로 연결하여 문자열로 변환하고 input 태그에 저장
        - 회원들의 목록정보가 담긴 input태그의 value값을 RequestParam으로 가져와 배열로 변환하고 순차적으로 블랙리스트 등록 처리
        - 선택된 회원 정보의 블랙리스트 등록 여부값을 모두 'N'에서 'Y'로 바꾼 뒤 자동 새로고침
  - 검색 기능
    ![image](https://github.com/jinko0404/portfolio/assets/152952078/10f4bc45-8f66-4a4e-9cb8-0e0e302d962d)
    * 검색 타입과 키워드를 입력하여 원하는 검색 결과가 목록에 나타날 수 있도록 검색 구현
      1)	select 태그를 이용하여 검색 타입 설정 후 input태그에 검색 키워드 입력
      2)	타입과 키워드 값을 RequestParam을 이용하여 문자열 변수에 저장
      3)	각각의 변수에 저장된 타입 값과 키워드 값에 따른 검색 결과를 목록창에 GET형식으로 출력
  - 쪽지 기능
    ![image](https://github.com/jinko0404/portfolio/assets/152952078/0ef87099-7f8c-4de4-b003-9c7a2d6b3cd6)
    * CRUD 형식으로 보낸 이와 받는 이 아이디를 쪽지 정보 테이블에 저장하여 쪽지를 주고받는 방식으로 쪽지기능 구현
      1)	제목, 받는이, 내용 중 하나라도 안쓰고 전송 버튼을 누를 시
        - 쪽지 정보를 DB서버에 입력하는 것을 실패하므로 “메세지 전송에 실패하였습니다.”메세지 출력
      2)	쪽지 전송 성공
        - 쪽지 정보가 DB서버에 저장되고 쪽지함 목록 페이지로 이동

### :wine_glass:2. Red Oasis
* 와인 및 와이너리 정보 공유 커뮤니티(KH정보교육원 - 가팀 팀프로젝트)
  - 프로젝트 상세 설명 : [https://github.com/2311PublicDataWebApp/AreYouT.git](https://github.com/2311PublicDataWebApp/RedOasis)
  - 개발 기간 : 2024년 2월 15일 ~ 2024년 2월 26일
  - 담당 역할 : 팀원, JSP를 통한 웹 페이지 제작 및 네이버 지도 API를 활용한 와이너리 소개 메뉴 및 와인 소개 메뉴 구현
* Back-End
  - 사용 언어: JAVA
  - 사용 기술: Spring FrameWork, OracleDB
* Front-End
  - 사용 언어: JavaScript/CSS/HTML
  - 사용 기술: BootStrap, JQuery, Ajax
* 기능구현
  - 와이너리 소개(와이너리 지도)
    ![image](https://github.com/jinko0404/portfolio/assets/152952078/af0079d5-299c-4690-92da-ab1973e8d986)
    * 와이너리 등록 시 해당 와이너리의 주소로 좌표 값을 구하여 해당 좌표에 마커 표시
      1)	마커 클릭 시 해당 좌표의 와이너리 상세 소개 페이지 이동
      2)	네이버 지도 API 활용
      3)	마커에 마우스를 가져다 댈 시 해당 와이너리의 이름 표시
  - 와인 소개
   ![image](https://github.com/jinko0404/portfolio/assets/152952078/63a718d3-c3c8-4b27-84b3-739c518985e8)
    * 키워드를 입력하여 원하는 검색 결과가 목록에 나타날 수 있도록 검색 구현
    * 카테고리 별로 목록 조회 할 수 있도록 구현
      1) 카테고리 혹은 키워드를 RequestParam으로 받아 온 뒤에 Keyword값이 null 일시 category값을 넘겨주어 SELECT문 실행
         * 카테고리 값이 NULL일 시 전체 결과 출력
      2) 키워드 값이 null이 아닐 시 Keyword 값을 넘겨주어서 SELECT문 실행후 이름을 기준으로 검색된 결과값 반환
  - 댓글 기능
    ![image](https://github.com/jinko0404/portfolio/assets/152952078/ad36c13c-fdb0-43b5-8c1b-6160e1272e29)
    * CRUD 형식으로 구현
      1)	별점 기능 구현 : 와인 번호와 별점을 저장 하여 각 댓글의 점수 평균을 구하여 와인에 별점 부여
      2)	삭제 버튼 : 로그인한 세션의 회원 정보를 활용하여 자신이 쓴 댓글만 삭제버튼 출력
      3)	댓글 작성 완료 시 redirect로 새로고침
## 📞Contact
  - 이메일 : kojinsug0404@gmail.com
  - 깃허브 : https://github.com/jinko0404
