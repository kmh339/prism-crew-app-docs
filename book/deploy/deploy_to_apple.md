# 애플에 배포하기
- Xcode를 실행한 후, 메뉴바에서 Product > Archive 선택
- 아카이빙이 완료된 후(반드시 flutter build ios가 된 상태여야함), Organizer(Archives) 콘솔창에서 Runner의 버전을 확인한다.
- 배포하고자 하는 버전이 맞다면 해당 아카이브를 distribute app 한다.
- 이후 나오는 설정들은 기본값으로 해두고 마지막에 upload 버튼을 클릭한다.
- 만약 아카이브 이후 창이 뜨지않는다면 메뉴바에서 Windows > Organizer 로 콘솔창을 연다.
- [앱스토어 커넥트 - 마이앱스](https://appstoreconnect.apple.com/apps) 에서 프리즘 크루앱을 선택한다.
- TestFlights 탭에서 빌드된 버전을 확인한다. (약 15분 ~ 30분 소요)
- 이상이 없으면 자동으로 테스트플라이트를 통해 배포가 된다.
- 해당 버전을 스토어에 배포하려면 AppStore 탭에 Build 항목에 앱을 업로드 하고 각 텍스트 필드를 작성한 후, Submit for Review를 클릭한다.