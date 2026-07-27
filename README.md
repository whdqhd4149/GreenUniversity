# 🌱 GreenUniv

> 대학 홈페이지와 학사관리 기능을 구현한 JSP/Servlet 기반 팀 프로젝트

<br>

## 📌 프로젝트 소개

GreenUniv는 대학의 각종 정보를 제공하는 홈페이지와 학생·교수·강의 등을 관리하는 학사관리 시스템을 구현한 웹 프로젝트입니다.

JSP/Servlet 기반의 웹 개발 구조와 데이터베이스 연동 방식을 학습하기 위해 진행했습니다.

<br>

## 📅 프로젝트 정보

- **진행 기간**: 2025.08 ~ 2025.09
- **진행 형태**: 팀 프로젝트
- **담당 역할**: 관리자 페이지 화면 구성, 학생·교수 등록 및 DB 연동

<br>

## 🛠 기술 스택

### Backend

- Java 17
- JSP / Servlet
- JDBC

### Frontend

- HTML5
- CSS3
- JavaScript
- JSTL

### Database

- MySQL
- DBeaver

### Development Tools

- Eclipse
- Apache Tomcat
- GitHub
- Figma

<br>

## 🖥 주요 기능

### 대학 홈페이지

- 대학 소개 및 입학 안내
- 학사 안내 및 대학생활 정보 제공
- 커뮤니티 및 게시판
- 로그인 및 회원가입
- 학생 성적 및 학적 조회

### 학사관리 시스템

- 학생·교수 등록 및 목록 조회
- 학과 등록 및 관리
- 강의 등록 및 목록 조회
- 수강 현황 및 교육 운영 현황 조회

<br>

## 👨‍💻 담당 기능

### 1. 관리자 페이지 공통 화면 구성

- 학사관리 시스템의 관리자 화면 레이아웃 구성
- 상단 헤더, 왼쪽 사이드바, 본문, 하단 푸터 영역 배치
- 각 관리 기능의 본문 화면을 공통 구조 안에 배치
- 교육 운영 현황, 강의 목록, 강의 등록, 수강 현황 화면 구성

### 2. 학생 등록 및 DB 연동

- 학생 등록 화면에서 입력한 정보를 Controller에서 수신
- DTO, Service, DAO를 거쳐 학생 정보를 데이터베이스에 저장
- 입학연도, 학과코드, 순번을 조합하여 학번 자동 생성
- 등록된 학생 정보를 관리자 목록 화면에서 조회

```text
학생 등록 화면
→ StudentRegisterController
→ StudentService
→ StudentDAO
→ Database
```

### 3. 교수 등록 및 목록 조회

- 교수 등록 화면과 데이터베이스 저장 기능 구현
- 등록 화면에 학과 목록을 조회하여 출력
- 임용연도, 학과코드, 순번을 조합하여 교번 자동 생성
- 등록된 교수 목록 조회 및 검색 기능 구현

```text
교수 등록 화면
→ ProfessorRegisterController
→ ProfessorService
→ ProfessorDAO
→ Database
```

<br>

## 📂 담당 기능 구조

```text
controller
├── StudentRegisterController.java
└── ProfessorRegisterController.java

service
├── StudentService.java
└── ProfessorService.java

dao
├── StudentDAO.java
└── ProfessorDAO.java

dto
├── StudentDTO.java
└── ProfessorDTO.java

views
└── academic
    ├── operation
    └── personnel
        ├── student-register.jsp
        ├── students.jsp
        ├── professor-register.jsp
        └── professors.jsp
```

<br>

## 💡 프로젝트를 통해 배운 점

- JSP/Servlet 기반 웹 애플리케이션의 요청과 응답 흐름을 이해했습니다.
- Controller, Service, DAO, DTO로 역할을 분리하여 데이터베이스와 연동하는 과정을 경험했습니다.
- Git 브랜치와 Pull Request를 활용한 팀 협업 방식을 경험했습니다.
- 프로젝트 기간 내 상세한 입력값 검증과 중복 확인 기능까지 완성하지 못해, 유효성 검사의 중요성을 확인했습니다.
