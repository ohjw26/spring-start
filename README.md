# hello-spring

Spring Boot 학습용 프로젝트입니다. 인프런 김영한님의 *스프링 입문* 강의를 따라가며 작성한 코드를 정리합니다.

## 기술 스택

- **Java** 17
- **Spring Boot** 4.0.6
- **Spring Web MVC** — 웹 애플리케이션
- **Thymeleaf** — 서버사이드 템플릿 엔진
- **Gradle** — 빌드 도구
- **JUnit 5** — 테스트

## 시작하기

### 요구 사항

- JDK 17 이상

### 실행

```bash
./gradlew bootRun
```

기본 포트(8080)로 실행됩니다. → http://localhost:8080

### 빌드

```bash
./gradlew build
```

빌드 산출물은 `build/libs/` 아래에 생성됩니다.

### 테스트

```bash
./gradlew test
```

## 프로젝트 구조

```
hello-spring/
├── build.gradle              # 빌드 설정 및 의존성
├── settings.gradle           # 프로젝트 이름 설정
├── gradlew, gradlew.bat      # Gradle Wrapper 실행 스크립트
├── gradle/wrapper/           # Gradle Wrapper 바이너리/설정
└── src/
    ├── main/
    │   ├── java/hello/hello_spring/
    │   │   └── HelloSpringApplication.java   # 애플리케이션 진입점
    │   └── resources/
    │       └── application.properties        # 애플리케이션 설정
    └── test/
        └── java/hello/hello_spring/
            └── HelloSpringApplicationTests.java
```

## 참고

- 패키지 이름이 `hello.hello-spring`이 아니라 `hello.hello_spring`인 이유: 자바 패키지 이름에 하이픈(`-`)을 사용할 수 없습니다.
- 추가 레퍼런스는 [`HELP.md`](./HELP.md) 참고.
