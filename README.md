# 2021_FarmCompetition

## 채점 서버 - Visual Studio Code 연동 테스트

### Requirements
* Node.js 설치 환경
* python3, Flask가 설치된 리눅스 또는 Docker 실행가능 환경
* Visual Studio Code

## 서버 열기

### Docker 환경
1. server/dockerbuild.bat 로 도커 빌드
2. 빌드 후 optional setting -> Local host: 8888 로 컨테이너 실행 
    1. <img src="https://user-images.githubusercontent.com/48395704/115210879-fcb72180-a139-11eb-9f60-3aab531efce7.png" width="40%" height="40%">
4. 컨테이너 실행 후 127.0.0.1:8888 로 접속
5. 접속에 성공하면 서버 열린거


## Visual Studio Code Extension 빌드

- 빌드 세팅
필요 모듈 설치 

```
cd vscode-extension
yarn install
```

1. src/extension.ts 를 열고 F5 누르면 확장 프로그램 빌드 시작
2. 빌드 후에 디버깅 모드로 들어가는데, 새로 뜬 창에 C++ 코드 입력 후 우클릭 -> Judge 클릭
    1. <img src="https://user-images.githubusercontent.com/48395704/115213315-5ddff480-a13c-11eb-971b-12acae56ca7f.png" width="60%" height="60%">
4. Judge 클릭하면 서버에서 C++ 코드를 실행시킨 결과를 받아옴
    1. <img src="https://user-images.githubusercontent.com/48395704/115213596-a1d2f980-a13c-11eb-8187-3001511da1d9.png" width="60%" height="60%">

### 실행 gif
![vsbuild](https://user-images.githubusercontent.com/48395704/115215973-01ca9f80-a13f-11eb-8476-18ecc1af59f1.gif)

