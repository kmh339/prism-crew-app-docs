## **Features**
- user 인스턴스를 생성하고 지니고 있는 컨트롤러
- StateMixin을 통해 user의 상태변화를 변경
- 초기의 RxStatus = empty

## _startApp()
- 앱 시작 시, 호출
- userProvider를 통해 user 인스턴스 생성
- 성공 시, RxStatus = success
- 실패 시, RxStatus = error

## authenticate()
- username: 사용자 아이디
- password: 사용자 패스워드
- shouldAutoLogin: 자동로그인 선택 여부
- 로그인페이지를 통해 로그인을 시도하면 userProvider를 통해 user 인스턴스 생성

## deAuthenticate()
- 로그아웃 메소드
- RxStatus = error