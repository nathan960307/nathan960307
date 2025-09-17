## 프로젝트 개요

### 프로젝트명  
**카페 메뉴 관리 서비스**

### 링크  
- [GitHub](https://github.com/prgrms-be-devcourse/NBE5-6-1-Team03)  
- [일정 관리](https://trello.com/b/itm14CbP/nbe5-6-1)
- [데모 화면 제작]()  - 추가 필요

### 개요  
로컬 카페 **“Grids & Circles”**의 원두 메뉴를 온라인으로 관리하고 주문받을 수 있는 **웹 기반 주문 관리 시스템**입니다.  
CRUD 기반의 메뉴 등록·조회·수정·삭제 기능을 제공하며, MyBatis와 Spring을 활용해 DB와 연동했습니다.  
또한, JSP 기반의 화면을 통해 메뉴를 카드 형태로 출력하고, 장바구니 및 주문 요약 화면을 구현했습니다.

### 진행 배경  
- 카페 사장의 원두 판매 관리 간소화  
- 하루 주문(전날 오후 2시 ~ 당일 오후 2시) 집계 및 배송 프로세스 구현  
- 실무형 **CRUD + DB 연동 학습 목적**으로 진행  

### 기간 / 인원  
- **2025.04.22 ~ 2025.04.28 (7일)**  
- **팀 프로젝트 (5명)**  
- **본인 역할**  
  - 메인 페이지 및 메뉴 조회 화면 구현  
  - MyBatis 기반 메뉴 조회 SQL 작성 및 연동  
  - JSP 카드 UI로 메뉴 출력
 
--- 
## ERD

- ** 사진 추가 필요**  
- ** 테이블 설명 추가 필요** 
--- 

## 사용 기술 및 라이브러리

### Backend  
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white"/>
  <img src="https://img.shields.io/badge/MyBatis-005B9F?style=flat"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white"/>
</p>

### Frontend  
<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/JSP-007396?style=flat"/>
</p>

### Tools & ETC  
<p>
  <img src="https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=flat&logo=intellijidea&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Tomcat-F8DC75?style=flat&logo=apachetomcat&logoColor=black"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>
</p>


---
## 담당 기능

### 기획 / 설계
- **메인 페이지 & 메뉴 조회 화면** 기획 및 UI 구조 설계  
- 메뉴 데이터를 카드 형식으로 출력하는 **JSP 화면 구조** 설계  
- DB 테이블 설계 참여 (Menu, Order, OrderItem)  

### Server
- **메뉴 조회 API 구현** (Spring + MyBatis)  
- MyBatis 매퍼 XML 작성 및 SQL 최적화  
- JSP와 Controller 연동을 통한 메뉴 리스트 출력  
- Tomcat 환경에서 서버 실행 및 디버깅 지원

  ---
## 결과 & 회고

- **결과**
  - 메인/메뉴 **SSR 페이지** 배포 완료  
  - 메뉴별 이미지 **썸네일(목록)**·**상세 1장** 노출 구현  
  - Controller–Service–DAO(MyBatis)–JSP 구조로 **읽기(READ) 흐름 안정화**

- **잘한 점**
  - FE–BE **Model 키·뷰 경로 합의**로 연동 매끄러움 (`menus`, `imageMap`, `menu`, `image`)
  - 이미지 **일괄 조회 → menuId 그룹핑(imageMap)** 으로 **N+1 쿼리 회피**
  - 작은 단위 **feature 브랜치 + PR**로 빠른 피드백 사이클 유지

- **아쉬운 점**
  - 범위가 **READ 중심**이라 **REST API / C·U·D, 페이지네이션·검색** 미포함
  - 상세 화면은 **이미지 1장 표시** (DB/서비스는 1:N 가능 구조였음)

- **배운 점**
  - **SSR(HTML) vs REST(JSON)** 책임과 표현의 차이 체득
  - 업로드/정적 **경로 매핑 분리**의 중요성 (엑박·경로 이슈 예방)
  - 초기에 **인터페이스 문서화**(Model 키/뷰 경로)가 협업 비용을 크게 줄임
  - 
  ---
## 트러블 슈팅
- **추가예정**
