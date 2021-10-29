## 빌드 방법

# 공통
- [비밀 - 프리즘 서버, 모바일 노션](https://www.notion.so/koreaspacedata/4b0ba090ec0440d1a9fa57a11f00f43a)에서 
GoogleServices 키 파일들을 다운받아 android/app/google-services.json 과 ios/Runner/GoogleService-Info.plist 에 각각 위치시킨다.

# Android
- android/key.properties 생성
```
storePassword=ksdprism
keyPassword=ksdprism
keyAlias=key
storeFile=<key.jks 파일의 경로>/key.jks
```
