# 환율계산기

👉 [배포주소 바로가기](http://pleasedoit.s3.ap-northeast-2.amazonaws.com/index.html)

<br>

### 📈 디렉토리 구조

```
├── README.md
├── craco.config.js
├── package.json
├── public
│   ├── currencyInfo.json
│   ├── dummy.json
│   ├── favicon.ico
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── src
│   ├── App.jsx
│   ├── api
│   ├── assets
│   ├── components
│   ├── hooks
│   ├── index.jsx
│   ├── pages
│   ├── reportWebVitals.js
│   ├── setupTests.js
│   ├── style
│   └── utils
└── yarn.lock
```
<br>

### 🧐 프로젝트 빌드 및 실행 방법

1. 상단 `Code` 버튼을 눌러 레포지토리를 클론 받습니다.

```
$ git clone https://github.com/wanted-team2/1week_calculation.git
```

2. 패키지를 설치합니다.

```
$ yarn install
```

3. 서버를 실행합니다.

```
$ yarn start
```

3-2. 테스팅을 합니다.

```
$ yarn jest --watchAll
```

<br>

## 공통 명세

- [x] 송금액은 숫자만 입력되도록 한다.
- [x] 인풋 값이 1000 이상이고, 세 번째 자리마다 콤마(,)를 추가한다.

<br>
<br>

## 1️⃣ 1번 계산기

### 팀원

- 김지영
- 고병표

### 구현 명세

- [x] 드롭다운 메뉴 선택 시 변경된 환율을 표시한다.
- [x] Submit 버튼 클릭 시 환율에 따라 계산된 수취금액을 표시한다.
- [x] 올바르지 않은 송금액을 입력 시엔 수취금액 하단에 에러 메세지 `송금액이 바르지 않습니다` 표시
- 송금액이 0 미만일 때
- 송금액이 10,000 초과일 때
- 송금액을 입력하지 않았을 때

### 데모

| **수취국가 변경** | **에러 메세지 표시** |
| :-: | :-: |
| ![calc1-1](https://user-images.githubusercontent.com/68528752/151088275-473b80f5-41de-4dcd-9210-3e63013b1ee2.gif) | ![calc1-2](https://user-images.githubusercontent.com/68528752/151088821-8e464e8f-4ed0-489e-8a73-f67f9981edaf.gif) |

<br>


## 2️⃣ 2번 계산기

### 팀원

- 유제호
- 홍수연

### 구현 명세

- [x] 드롭다운 메뉴에 제시된 통화는 USD,CAD,KRW, HKD,JPY,CNY로 6가지다.
- [x] 드롭다운 메뉴 중 하나를 택하면 직전 select된 국가와 탭에 있는 국가의 자리가 바뀐다.
- [x] 사용자의 입력(인풋/셀렉트)이 들어갈 때 마다 동기화되어 바뀐다.
- [x] 날짜 포멧은 YYYY-Month-dd 형태여야한다.(ex: 2022-Jan-01)

### 데모

| **수취국가 변경** | **수취금액 표시** |
| :-: | :-: |
| ![calc2-1](https://user-images.githubusercontent.com/78653426/151075961-c843ce54-39c5-4963-abdf-7c34cafd41e0.gif) | ![calc2-2](https://user-images.githubusercontent.com/78653426/151075973-3c880218-09a3-49cb-9dec-e7e2ec73eed7.gif) |
