# 고진석 포트폴리오

## 😃Intro
안녕하세요, "지속적인 학습과 실천을 통해 성장하는 개발자" 고진석 입니다. 웹개발에 대한 열정을 가지고 있으며, 
사용자 친화적인 사이트를 제작하고 운영하는 개발자가 되는 것을 목표로 하고 있습니다.

## 🗂Project
제가 진행해왔던 프로젝트입니다.
팀장으로써 프로젝트를 진행할 때는 프로젝트의 일정 관리, 팀원들의 의견 조율 등의 경험을 할 수 있었으며
팀원으로써 팀장의 지시나 요구사항에 따라 프로젝트를 진행을 하는 등의 경험을 쌓을 수 있었습니다.

### 1. Are You T(rip mate)?
* 여행 동행 친구 모집 사이트(KH정보교육원 - 1조 팀프로젝트)
  - 프로젝트 상세 설명 : https://github.com/2311PublicDataWebApp/AreYouT.git
  - 개발 기간 : 2024년 2월 15일 ~ 2024년 2월 26일
  - 담당 역할 : 팀장, MVC패턴을 활용한 관리자 기능(회원 관리, 1대1 문의쪽지함, 쪽지 관리, 게시판 관리) 구현, JSP를 통한 웹 페이지 제작
* Back-End
  - 사용 언어: JAVA
  - 사용 기술: Spring FrameWork, OracleDB
* Front-End
  - 사용 언어: JavaScript/CSS/HTML
  - 사용 기술: BootStrap, JQuery
* 기능구현
  - 일반 회원 관리
  ![image](https://github.com/2311PublicDataWebApp/AreYouT/assets/152952078/f1db10f9-66d8-49fd-8536-68f670ac1680)
  * 체크 된 회원을 한번에 일괄적으로 묶어서 블랙리스트에 등록 할 수 있도록 구현
1)	체크된 회원 없이 블랙리스트 등록을 시도할 경우
- 회원값을 저장하는 배열의 길이가 0이므로 “체크된 회원이 없습니다.” 메세지 출력
2)	블랙리스트 등록 성공
- 체크된 회원의 목록이 저장된 배열을 구분자 “,”으로 연결하여 문자열로 변환하고 input 태그에 저장
- 회원들의 목록정보가 담긴 input태그의 value값을 RequestParam으로 가져와 배열로 변환하고 순차적으로 블랙리스트 등록 처리
- 선택된 회원 정보의 블랙리스트 등록 여부값을 모두 'N'에서 'Y'로 바꾼 뒤 자동 새로고침
