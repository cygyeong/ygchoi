---
title: "android) aab 파일을 apk로 변환하기 "
excerpt: "aab 파일을 apk로 변환하기 "

categories:
  - ReactNative
tags:
  - [ReactNative, android]

permalink: /ReactNative/1/

toc: true
toc_sticky: true

date: 2023-12-28
last_modified_at: 2023-12-28
---

## 🐻 문제
ab 파일을 apk로 변환

## 🐿️ 해결
aab 파일은 apk와 달리 바로 기기에 깔리지 않는다. 

<https://github.com/google/bundletool/releases>


여기서 bundletool를 설치한다. 

터미널로 해당 bundletool이 설치된 곳으로 이동한 후 

```
java -jar "bundletool-all-[설치한 bundletool 버전 작성].jar" build-apks —bundle="[aab 파일이 있는 경로/aab파일 이름.aab]" —output="universal.apks" —mode=universal
```

이렇게 하면 커맨드를 실행한 터미널 경로에 universal.apks가 생성된다. 

apks를 zip으로 확장자 이름을 변경해준다. 

해당 압축파일을 압축해제 하면 apk가 나온다. 
```

## 🐰 과정


## 🦊 주의사항
- aab 파일의 경로 잘써주자
- bundletool 버전을 정확하게 써주자
