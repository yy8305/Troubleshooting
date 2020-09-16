# 환경
- react-native-cli : 2.0.1
- pod : 1.9.3

# 에러 내용
- React native ios 세팅하던중 에뮬레이터 실행이 안됨
- react-native run-android 는 정상 동작
- react-native run-ios 시 cocoapods 관련 에러 발생
```
error Could not find "Podfile.lock" at /Users/[NAME]/Project/sample/ios/Podfile.lock. Did you run "pod install" in iOS directory?
```

# 해결
- 프로젝트 폴더로 이동후 아래 명령어 실행
```
    $ cd ios 
    $ pod repo update
    $ pod install
```


# 참고
-  https://github.com/react-native-community/cli/issues/487#issuecomment-513208098