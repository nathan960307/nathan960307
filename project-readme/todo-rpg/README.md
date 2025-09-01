## 프로젝트 개요

### 프로젝트명  
**TODO-RPG**

### 링크  
- [GitHub - ToRPG ver1](https://github.com/prgrms-be-devcourse/NBE5-6-2-Team04)  
- [GitHub - ToRPG ver2](https://github.com/prgrms-be-devcourse/NBE5-6-3-Team04)  
- [API 명세서](#)  - 추가 필요
- [일정 관리](#)   - 추가 필요

### 개요  
**Developer TODO-RPG (ToRPG)** 는 개발자 지망생과 커리어 전환자를 대상으로 한 **성장 관리 서비스**입니다.  
TODO 리스트 관리에 RPG 게임 요소(레벨, 경험치, 스탯, 퀘스트 등)를 접목하여, 사용자가 학습과 목표 달성을 **게임처럼 즐기면서 성취감**을 느낄 수 있도록 설계했습니다.  

- **ver1 (기본 기능 개발)**  
  - 목표(Goal)와 투두(Todo) 생성/수정/삭제  
  - 가이드 커리큘럼 제공  
  - 포트폴리오용 활동 기록 기능 구현  

- **ver2 (리팩토링 및 확장)**  
  - JWT 기반 인증/인가
  - 엔티티 및 서비스 구조 리팩토링  
  - **FullCalendar 기반 일정 관리 UI 적용**  
  - **추천 문제 크롤링 → TODO 생성/체크 → 경험치(XP) 부여** 기능 구현 

이를 통해 단순한 할 일 관리 앱을 넘어, **개발자 성장 과정을 데이터로 증명하고 관리할 수 있는 RPG형 플랫폼**으로 발전시켰습니다.  

### 진행 배경  
- 개발자 지망생 및 커리어 전환자들이 **체계적으로 목표를 관리하고 성장 과정을 기록할 수 있는 도구의 부족**  
- 기존 TODO 서비스들은 단순한 일정 관리에 그쳐, **학습 동기 부여와 성취감 제공이 부족**  
- RPG 게임 요소(레벨, 경험치, 퀘스트 등)를 접목해 **목표 달성을 재미있게 지속할 수 있는 방식**을 실험  
- 팀 프로젝트를 통해 **Spring Boot + JPA 기반 실무형 서비스 설계 및 협업 경험**을 쌓기 위함  


### 기간 / 인원  
- **2025.05.01 ~ 2025.06.20 (약 7주)**  
- **팀 프로젝트 (5명)**  
- **본인 역할**  
  - 목표(Goal)·투두(Todo) **CRUD 기능** 구현 및 대시보드 연동  
  - **FullCalendar 기반 일정 관리 UI** 적용 및 서버 연동  
  - **추천 문제 크롤링 → TODO 생성/체크  기능 구현   
 
--- 
## ERD

- **사진 추가 필요**  
- **테이블 설명 추가 필요**  

--- 

## 사용 기술 및 라이브러리

### Backend  
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Data%20JPA-59666C?style=flat&logo=hibernate&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white"/>
</p>

### Frontend  
<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=flat&logo=thymeleaf&logoColor=white"/>
  <img src="https://img.shields.io/badge/FullCalendar-3A87AD?style=flat"/>
</p>

### Tools & ETC  
<p>
  <img src="https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=flat&logo=intellijidea&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apachemaven&logoColor=white"/>
</p>


---
## 담당 기능

### 기획 / 설계
- **대시보드 화면** 기획 및 UI 구조 설계 (목표·투두 통합 관리)  
- **FullCalendar 기반 일정 관리 UI** 적용 및 서버 연동 설계  
- 목표(Goal)·투두(Todo) 관련 **DB 테이블 설계 참여**  

### Server
- 목표(Goal)·투두(Todo) **CRUD API 구현** (Spring Boot + JPA)  
- **FullCalendar 일정 연동 API** 구현  
- **추천 문제 크롤링 → TODO 자동 생성/체크 로직** 구현  
- Controller–Service–Repository 구조로 리팩토링 및 디버깅 지원  

---
## 결과 & 회고

- **결과**
  - 목표(Goal)·투두(Todo) CRUD 기능 구현 완료  
  - FullCalendar 기반 일정 관리 화면 및 서버 연동 적용  
  - 추천 문제 크롤링 → TODO 생성/체크 → XP 부여 흐름 구현  
  - 대시보드에서 목표와 투두를 한눈에 관리할 수 있는 UI 제공  

- **잘한 점**
  - 기능 단위 **브랜치 전략**과 **PR 리뷰**를 통해 협업 효율을 높임  
  - **대시보드·캘린더·투두 기능 간 연동**을 명확히 설계해 확장성 확보  
  - 크롤링과 TODO 연계를 통해 단순 일정 관리에서 **차별화된 기능** 제공  

- **아쉬운 점**
  - 기간 한정으로 인해 **인증/인가·보안·배포** 등은 최소화  
  - **테스트 코드 부족**으로 리팩토링 시 안정성 확보에 어려움  
  - UI는 기능 위주 구현이라 **디자인 완성도 부족**  

- **배운 점**
  - **기능 기획 단계에서 DB·UI 구조를 먼저 합의**하는 것이 협업 비용을 크게 줄임  
  - **SSR 기반 뷰 렌더링과 동적 캘린더 연동 차이**를 경험하며 프론트-백엔드 연결을 깊게 이해  
  - 크롤링 데이터를 서비스 로직과 연결하면서 **외부 데이터 활용·확장성 설계의 중요성** 체득  


---
## 트러블 슈팅
- **추가 예정**  
