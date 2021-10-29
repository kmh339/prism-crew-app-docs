## Features
- offer의 상태관리 컨트롤러
- offer를 RxOffer로 받아옴
- offer의 상태에 따라 statusColor, statusText 변경

## updateReadAt()
- offer의 readAt을 현재 시간으로 업데이트 하는 메소드
- 기획의도에 따라 null일때만 readAt을 삽입하도록 구현
- offer의 상태에 따라 offerList 탭의 RedDot(Badge)를 체크하는 로직인 checkAssignedUnread() or checkMyOfferUnread()를 호출

## changeOfferStatus()
- offer의 상태를 변경시켜주는 메소드
- offerCard의 상태태그와 색상도 함께 변경

## acceptOffer()
- offer 수락 메소드
- 현재 offerCard를 내업무 탭으로 이동

## startOffer()
- offer 시작 메소드
- 작업 시작 전 사진을 찍는 메소드를 호출
- beforePhoto가 정상적으로 찍혔으면 다이얼로그를 띄우고 offer의 상태를 inProgress로 변경
- 대쉬보드 카운트도 업데이트

## cancleOffer()
- offer 배정 취소 메소드
- 내업무 탭에 있던 offerCard를 배정요청 탭으로 이동

## stopOffer()
- offer 중지 메소드
- offerstatus = aborted

## finishOffer()
- offer 완료 ㅔ소드
- 작업 완료 후 사진을 찍는 메소드 호출
- afterPhoto가 정상적으로 찍혔으면 다이얼로그를 띄우고 offer의 상태를 completed로 변경