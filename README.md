## OurBnB

![Our B B](https://user-images.githubusercontent.com/71913557/111892238-f6e7f680-8a3c-11eb-96c2-fb8c37443997.gif)

## 프로젝트 기간

2021.03.02 ~ 2021.03.12

## 프론트엔드

- 허혜성
- 김연주
- 강민지

## 프론트엔드 기술스택

html, css, styled-componenet, scss, Javascript, CRA, React, react-hook

## 프론트엔드 구현목록

## 강민지

### Main

- daterangepicker를 통한 캘린더 구현
- 날짜, 인원수의 input value값을 querystring을 통해 axios API 통신

### DetailList Page

- react-router를 이용한 page간 props 전달, 이전 페이지에 입력하였던 예약 인원수를 detail list 상단에 표시
- roomtype 체크박스 폼 및 pricerange input 폼 모달창 구현
- filter조건에 따른 state 값을 배열에 담은 뒤 map을 통해 state 상태검사 및 params append, delete - 다중 필터구현(룸 타입을 추가하거나 가격을 조정할 경우 해당 조건에 따라 querystring이 추가되고 삭제되는 로직)
- 조건에 따라 state 상태값을 변경, translateX 값을 변경하여 scroll 기능 구현
- goole-map 활용, 위도와 경도를 서버에서 받아온 data로 부터 추출하여 새로운 state에 저장, maping 하여 fetch된 집들의 위치에 따라 map의 marker 전환 구현.
- Pagenation 구현

## 허혜성

### Footer

- 레이아웃 구현

### Detail Page

- UI 컴포넌트 및 레이아웃 구현
- react-router를 이용한 page간 props로 전달된 인원수와 예약일수를 활용하여 숙박이용 일수 및 총금액 구현
- token 여부에 따른 서비스 제한 및 제공여부 구현
- 디테일리스트에서 상세페이지로 넘어가는 동적라우팅 구현
- 숙박 정보 axios API 통신
- histoy.location.state를 사용하여 "체크인-체크아웃날짜/인원/숙박이용일수/1박금액/수수료/총금액/숙소정보(id,이름,이미지,룸타입,평점)"를 결제페이지로 전달

### My Page

- UI 컴포넌트 및 레이아웃 구현
- 예약 정보 axios API 통신
- Data Mapping을 통한 Menu Tap 구현


## 김연주

### Login 

- 레이아웃을 모달창으로 구현
- Kakao Developer 홈페이지를 참고하여 공개 API 표준 인증 방법 OAuth2.0 를 이용하여 인가코드로
  토큰을 받아 다시 fetch로 backend와 API통신
  

### payment

- 레이아웃 구현 후 결제창과 예약정보창 컴포넌트 분리
- 디테일 페이지와 결제페이지를 react-router로 page 이동
- location.state 사용하여 숙소, 총 금액, 인원을 을 props로 받아 결제창 UI에 구현
- 결제정보(숙소,예약날짜,가격,인원)을 fetch 함수를 이용하여 API통신
  
