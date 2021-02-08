
## 방금 인친이 올린 게시글 속 카페와 비슷한 내 주변 카페 없나?☕️ 
뭐라고 검색하실건가요? 삼성동 카페? 
방금 인친이 올린 인스타그램 게시글 속 카페같이 __#콘크리트 느낌, #에스프레소가 맛있는, #지금 내 주변의!__ 카페에 가고 싶은 당신, __서울 카페 지도__ 와 __서울 챗봇__ 이 선택을 도와줄게요!

### [#카페스타그램] 카페에서 만족스러운 시간을 보낸 후, 그 기분을 인스타그램에 기록하는 일종의 의식
때문에 우린 처음 가는 카페에 방문하기 전 인스타그램에 카페를 검색해보곤 합니다. 어떤 사진들이 업로드되는지 보면 그들이 카페에서 어떤 시간을 보냈는지, 어떤 메뉴가 맛있는지 가보지 않고도 알 수 있습니다. 아래는 카페 mk2를 검색한 모습입니다. 이미지가 모여져 있는 모습에서 카페의 분위기가 느껴지지않나요? 

<img width='50%' src='https://user-images.githubusercontent.com/42338386/106733676-8421e800-6655-11eb-8750-af5f6b456fb3.png'> 

그리고 우리는 종종 #카페스타그램 속 모습을 소비하기 위해 인스타그램 속 카페를 방문합니다.  
그들을 위한 #카페스타그램 기반 카페 분류 __서울 카페 지도 🗺 & 챗봇 🗣__
내가 있는 지역의 뷰 맛집/ 메뉴 맛집 카페는 물론, 시그니처 메뉴, 사람들은 이 카페에서 어떤 사진을 찍었는지, 이 카페에서 어떤 것을 기대하면 좋을지 보여줄게요!

## 서울 카페 지도 🗺 & 챗봇 🗣

__서울 카페 지도__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105575023-bb69dc80-5dab-11eb-8856-2cc0e49d1fc1.gif'>

__서울 카페 챗봇__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105578468-c7619880-5dc3-11eb-9a04-e7943c601fd8.gif'>


   
## Keyword
__Instagram crawling, MongDB,Flask, AWS, Multinominal Naive Bayes, Google Vision API, BS4,Selenium, Kakao map API__



## 카페 분류 구조

<img src="https://user-images.githubusercontent.com/72846750/105801786-40880800-5fdd-11eb-8ca0-d878457cb5e8.png" width="70%">

## 프로젝트 과정

### #카페스타그램 크롤링 | BS4, Selenium, AWS, boto3
#카페스타그램은 해당 카페의 분위기와 시그니처 메뉴같은 대략의 데이터를 내포하고 있습니다.  
사람 얼굴이 포함되지 않은 사진, 해시태그, 좋아요 수 등을 셀레니움을 통해 크롤링했습니다.
인스타그램은 ip, id를 기반으로 수상한 유저를 검출하여 접근을 막습니다. 
우리는 boto3, AWS를 통해 ip를 우회하여 크롤링을 진행하였습니다.

<img src="https://user-images.githubusercontent.com/42338386/106738618-7ff8c900-665b-11eb-9abc-f042b629643f.png" width='50%'>


### 이미지에서 카페 패턴, 분위기 검출 | Google Vision API, MultinominalNaive Bayes 모델  
이미지의 패턴을 ~하기 위해 Google Vision API를 통해 이미지 Labels를 추출하였습니다.
추출된 Labels는 Naive Bayes 모델을 통해 View 맛집과 Menu 맛집으로 분류하였습니다.

### 서울 카페 지도 | Flask, Kakao map API
kakao map api를 통해 만든 html페이지를 Flask로 구현하였습니다. 

### 카페 챗봇 | Flask, Slack API 
Slack api를 통해  Flask로 구현하였습니다. 
   






