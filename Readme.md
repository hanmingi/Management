# Clan Management System (Spring Boot + Gradle + Thymeleaf)

## 프로젝트 개요

이 프로젝트는 **클랜원** 및 **일정**을 관리하기 위한 Spring Boot 기반의 RESTful 웹 애플리케이션입니다. 사용자는 클랜원 정보를 조회, 추가, 삭제할 수 있으며, 일정 역시 관리할 수 있습니다. 또한, HTML 템플릿 엔진인 **Thymeleaf**를 사용하여 웹 페이지에서 결과를 시각적으로 확인할 수 있습니다.

## 주요 기술 스택
- **Java**: 17
- **Spring Boot**: 3.3.4
- **Gradle**: 8.3 (최신 버전 사용)
- **Thymeleaf**: HTML 템플릿 엔진
- **H2 Database**: 인메모리 데이터베이스 (개발 및 테스트용)
  - **JPA (Java Persistence API)**: 데이터베이스 연동
- **Lombok**: 보일러플레이트 코드 제거를 위한 도구

## 기능 설명

### 1. **클랜원 관리**
- **조회**: 모든 클랜원을 조회합니다.
- **추가**: 새로운 클랜원을 추가합니다.
- **삭제**: 클랜원을 삭제합니다.

### 2. **일정 관리**
- **조회**: 모든 일정을 조회합니다.
- **추가**: 새로운 일정을 추가합니다.
- **삭제**: 일정을 삭제합니다.

## API 엔드포인트

### 클랜원 관련 API
- **GET /api/clan-members**: 모든 클랜원을 조회합니다.
- **POST /api/clan-members**: 새로운 클랜원을 추가합니다. (JSON 형식으로 데이터를 전송)
- **DELETE /api/clan-members/{id}**: 해당 ID를 가진 클랜원을 삭제합니다.

### 일정 관련 API
- **GET /api/schedules**: 모든 일정을 조회합니다.
- **POST /api/schedules**: 새로운 일정을 추가합니다. (JSON 형식으로 데이터를 전송)
- **DELETE /api/schedules/{id}**: 해당 ID를 가진 일정을 삭제합니다.

## 설치 및 실행 방법

### 1. **프로젝트 클론**
```bash
git clone https://github.com/your-repo/clan-management-system.git
cd clan-management-system