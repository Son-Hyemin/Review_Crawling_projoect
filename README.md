# Review_Crawling_projoect
크롤링 데이터 솔루션을 통한 데이터 수집

## 1. 프로젝트명
Re.staurant ( Review Restaurant. 네이버 식당 리뷰를 크롤링 하여 성향판단 )

* **진행기관** <br/>
  \- Tmax Tibero : TABA2기 ( 캠퍼스 SW 아카데미 지원사업) <br/>
  \- CCCR : 한국클라우드컴퓨팅연구조합 <br/>
  \- 과학기술정보통신부 <br/>
  \- 단국대학교

## 2. 프로젝트 개요
**크롤링 데이터 솔루션을 통한 데이터 수집**
<br/>
<br/>
\- 워드 클라우드를 통한 키워드 분석으로 리뷰 키워드를 쉽게 보여준다 <br/>
\- 성향판단 모델을 통한 성향별 리뷰를 분류하여 서비스 제공 <br/>
\- 누구나 손쉽게 리뷰를 판단할 수 있는 서비스를 제공한다

<br/>

> ### 주제 선정
>
**1) 현재 리뷰 시스템의 문제점 파악**
  >
  허위리뷰를 통한 바이럴 마케팅의 기승과 네이버 리뷰의 별점 삭제로 인한 다양한 시점의 리뷰 접근의 어려움.
<br/>
<br/>
<br/>
**2) 대상자 및 주제 선정**
>
* **서비스 대상자** <br/>
코로나 19 엔데믹 후 증가하는 여행객들을 대상으로 선정 <br/>

![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/5c43c572-5e02-4f5a-a301-2d985dc001ec)
<br/>

* **리뷰 주제 선정** <br/>
 관광 지출액 비율중 식음료의 비율이 가장 높아 제공 서비스를 식당 리뷰로 선택 <br/>

![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/a7fccf72-49c3-4511-9fd8-f4ef93433d80) 
<br/>
( 출처 : 한국관광데이터 관광 지출액 2022.06~2023.05)



## 3. 개발환경
* **FRONT/BACK-END** <br/>
  \- React <br/>
  \- Figma <br/>
  \- Spring Boot <br/>

* **DATA BASE** <br/>
  \- TIBERO6 <br/>

* **데이터 수집** <br/>
  \- Jupyter <br/>

* **KVM** <br/>
  \- Docker <br/>

* **CI/CD/CB** <br/>
  \- Git Hub <br/>

* **Communication HUB** <br/>
  \- Notion <br/>

## 4. 프로젝트 진행 과정

![KakaoTalk_20240119_231258829_02](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/d0ef617f-9c63-48dc-9800-ca0809b136f1)


## 5. Architecture

### System Architecture
![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/7fe1a648-4eb5-4c13-b442-096bf5b8251b)

<details>
  <summary> Architecture 상세보기 </summary>

  ### 1) Server
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/2bed2282-f6a3-4925-ab1a-0be8b9cc55e2)

  ### 2) Data Base
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/832939f5-c2df-408b-a796-59f024e26231)

  ### 3) Crawling
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/4f73ea45-8f96-47dc-9b4f-b74a6cc8b082)

  ### 4) Model
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/2bfc9b0d-3c9c-43a7-a2ca-70354738855a)

  <!-- 내용 -->
</details>

<br/>

## 6. 자연어 처리 방법
한글 자연어 처리를 위해 KonLpy의 Okt를 사용하였으며 필요한 형태소 및 단어들을 보완작업하여 자연어 처리 완성도를 증가하였다. <br/>
 ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/5f184be5-ec67-428c-8291-e4d9ffe246ae)

<br/>

## 7. UI/UX

> 주요 기능 소개 <br/>
>
   1\) 검색창에 식당이름 혹은 음식 입력 시 관련 식당리스트 출력(인기검색 5위까지 확인 가능) <br/>
   2\) 식당을 선택하면 해당 식당의 상세 정보와 워드클라우드로 구현된 리뷰 키워드 확인 가능 <br/>
   3\) 리뷰 키워드 워드클라우드는 부정/중립/긍정으로 원하는 성향 선택 가능 <br/>
   4\) 워드클라우드에서 특정 키워드 선택 시 키워드가 포함된 리뷰 목록 출력 <br/>
   5\) 식당의 위치를 지도로 확인 가능

<details>
  <summary>UI/UX 상세보기</summary>

  ### (1) 홈 화면 소개 - 검색기능
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/2a07a2f5-9fd9-47a1-bae2-0a10c31c3553)

  ### (2) 홈 화면 소개 - 인기검색어
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/7e212849-39fa-47d5-bf62-38aa48b57fea)

  ### (3) 결과 화면 소개 - 워드클라우드
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/320359ec-9e08-4527-8f60-5a7b2b350719)

  ### (4) 결과 화면 소개 - 리뷰 성향 분류
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/e2a1752a-231b-4e20-b671-5ec325c7679e)

  ### (5) 부가 기능 소개 - 지도 및 로딩화면
  ![image](https://github.com/Son-Hyemin/Review_Crawling_projoect/assets/120477911/c484126d-fb3d-455f-9f81-53e5b66de4e4)

  <!-- 내용 -->
</details>


