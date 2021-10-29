## 개발 환경

```
Flutter 2.2.3
Dart 2.13.4
cocoapods 1.11.0
openjdk 11.0.11 2021-04-20

State Management : GetX
```

## 폴더 구조
[GetX Pattern](https://github.com/kauemurakami/getx_pattern#readme)

```
- /app
    - /core
        - /controllers  <----- 공용 컨트롤러
            - auth_controller.dart
        - /theme <----- 테마
        - /utils <----- 헬퍼, 키, 유용한 메소드 등
        - /values <----- 스트링값들
    - /data
        - /enums
        - /models
        - /providers
        - /services
    - /modules <----- 앱의 컴포넌트들
        - /some_module
            - /widgets <----- 각 모듈에서 쓰이는 위젯
            - controller.dart
            - some_module_page.dart
            - binding.dart
    - /widgets <----- 전역으로 쓰이는 위젯들
- main.dart <----- 실행지점
```

