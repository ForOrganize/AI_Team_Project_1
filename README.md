# 극성수기 여행 경비 안내 웹 개발

## 프로젝트 시나리오

- 웹 사이트 크롤링을 통해 필요 데이터를 수집하고 목적에 따른 결과를 내는 프로젝트
- 기본적으로 네이버 항공권 사이트(https://m-flight.naver.com/) 에서 데이터를 수집하며, 필요하다면 원하는 사이트를 크롤링하여 데이터 수집
- DB, HTML 등을 사용하여 실제 서비스처럼 결과물 제작


## 개발 배경 및 목표

- 전체적인 국내 여행 수요가 줄어 들었으며, 가성비 풍조에 따라 해외 여행을 선호하는 20-30대의 국내 여행 수요 증가를 위해 저렴한 경비를 편리하게 알 수 있는 서비스의 필요성을 파악
- 항공기, 교통편, 숙소 등의 비교적 고정적인 여행 비용을 조회할 수 있는 서비스 개발
- 목표로 설정한 김포-제주 간의 극성수기(7-8월)정보를 사용자의 니즈(날짜, 가격대, 출발지, 지역)에 맞춰 보여주고 옵션에 따라 합산한 금액을 출력

## 데이터 수집 및 분석

- 네이버 항공권, 호텔 사이트를 크롤링하여 데이터 수집 구글 클라우드 플랫폼의 빅쿼리에 적재
  - 빅쿼리는 데이터의 양이 많을 때 강점이 있는 DB지만 해당 프로젝트에선 분석과 운영의 용이함, 간단한 방식으로 파이썬 연동 등의 이유로 사용
- 항공권 데이터
  -  날짜, 항공사 이름, 출발 공항, 출발 시간, 도착 시간, 좌석 정보, 성인 1인을 기준으로 한 요금을 수집, 또한 필요에 따라 요일과 출발 시간대를 데이터에서 추출하여 포함
  -  제주행 편도 항공권과 김포행 편도 항공권을 합쳐 약 22000개의 데이터(왕복은 편도+편도로 계산된다)
- 

## 웹 개발

## 구조
