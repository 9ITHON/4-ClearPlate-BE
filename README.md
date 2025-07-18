# 4-CLP-BE api 서버 입니다.

---

# [1] Git 규칙

## (1) 커밋 규칙
* **fix**: 버그 수정
* **docs**: 문서 수정
* **style**: 코드 포맷팅, 세미콜론 등 (로직 변경 없음)
* **chore**: 빌드, 패키지 관리, 파일 삭제 등 기타 작업 (간단하고 하찮은? 일들)
* **refactor**: 코드 리팩토링
* **test**: 테스트 코드 추가
* **feat**: 새로운 기능 추가

ex) 
feat: 한글

## (2) 브랜치 관리 전략
**GitHub Flow
* main (배포환경)
* feat/#이슈번호 (새로운 기능 추가시)


---

# [2] 이슈 작성 규칙

## (1) 이슈 제목 작성 규칙
* **[Feature]** 새로운 기능 추가
* **[Fix]** 버그 수정 
* **[Documentation]** 문서 관련
* **[Refactor]** 코드 리팩토링
* **[Test]** 테스트 관련
* **[Chore]** 기타 작업
* **[Hotfix]** 긴급 수정
* **[Security]** 보안 관련

ex) 
[Feature] 회원관리

# [3] 프로젝트 구조
```
src
    ├── main
    │   ├── java
    │   │   └── com
    │   │       └── qithon
    │   │           └── clearplate
    │   │               ├── ClearplateApplication.java
    │   │               ├── domain
    │   │               │   └── user
    │   │               │       ├── dto
    │   │               │       │   ├── request
    │   │               │       │   │   └── UserRequest.java
    │   │               │       │   └── response
    │   │               │       │       └── UserResponse.java
    │   │               │       ├── entity
    │   │               │       │   └── User.java
    │   │               │       └── repository
    │   │               │           └── UserRepository.java
    │   │               ├── global
    │   │               │   ├── common
    │   │               │   │   └── dto
    │   │               │   │       └── response
    │   │               │   │           └── ResponseDTO.java
    │   │               │   ├── config
    │   │               │   │   ├── SwaggerConfig.java
    │   │               │   │   └── WebConfig.java
    │   │               │   └── security
    │   │               │       └── SecurityConfig.java
    │   │               └── infra
    │   │                   └── gemini
    │   │                       ├── GeminiClient.java
    │   │                       └── dto
    │   │                           ├── request
    │   │                           │   └── GeminiRequest.java
    │   │                           └── response
    │   │                               └── GeminiResponse.java
    │   └── resources
    │       ├── application.yml
    │       ├── application.yml.sample
    │       ├── static
    │       └── templates
    └── test
        └── java
            └── com
                └── qithon
                    └── clearplate
                        └── ClearplateApplicationTests.java

```

