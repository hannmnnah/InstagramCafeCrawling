## About the Project
### How do you find coffee shops?☕️ 
What search engines do you use? And what types of keywords do you use?
We can help you find a coffee shop that has the aesthetic or good pastry selection __#coffeegram, #coffeelover, #cafeseoul__. With __Seoul Café Map__ and __Café Chatbot__, we can help your coffee shop in Seoul!
 
#### It became a ritual for our generation to post a picture of a cup of coffee after spending a lovely afternoon at a coffee shop  [#coffeegram]. 
Thanks to our collective efforts to display the love of coffee shops, we often use Instagram to search and check out the coffee shops before visiting. When we look at the search results, we can view the kind of experience the coffee shop provides, such as the aesthetic and the popular drinks. 
Below is the search result for coffee shop mk2 in south Korea. Can you sense the vibe that the coffee shop offers when looking at people's posts? 
<img width='50%' src='https://user-images.githubusercontent.com/42338386/106733676-8421e800-6655-11eb-8750-af5f6b456fb3.png'> 

We often visit the coffee shops we find on Instragram to experience the #coffeegram. 
For those of you who use instagram to find your coffee shops, we have created #coffeegram based __Seoul Cafe Map 🗺 & Chatbot 🗣__
We can show you would expect from the coffee shops by classifying the cafes into either aesthetically or foodwise instagrammable cafes, and the signature menus, and how people usually take pictures at the cafe. 

## Seoul Cafe Map 🗺 & Chatbot 🗣

__Seoul Cafe Map__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105575023-bb69dc80-5dab-11eb-8856-2cc0e49d1fc1.gif'>

__Seoul Cafe Chatbot__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105578468-c7619880-5dc3-11eb-9a04-e7943c601fd8.gif'>


   
## Built with
__Instagram crawling, MongDB,Flask, AWS, Multinominal Naive Bayes, Google Vision API, BS4,Selenium, Kakao map API, HTML__



## Structure

<img src="https://user-images.githubusercontent.com/42338386/107241046-f0de1d80-6a6d-11eb-8697-ddce5065ae88.png" width="70%">


## Methods
### #Instagram Cafe Crawling | BS4, Selenium, AWS, boto3
#카페스타그램은 해당 카페의 분위기와 시그니처 메뉴같은 대략의 데이터를 내포하고 있습니다.  
사람 얼굴이 포함되지 않은 사진, 해시태그, 좋아요 수 등을 셀레니움을 통해 크롤링했습니다.
인스타그램은 ip, id를 기반으로 수상한 유저를 검출하여 접근을 막습니다. 
우리는 boto3, AWS를 통해 ip를 우회하여 크롤링을 진행하였습니다.

<img src="https://user-images.githubusercontent.com/42338386/106738618-7ff8c900-665b-11eb-9abc-f042b629643f.png" width='70%'>


### Extracting Patterns and Cafe Asthetics from the images| Google Vision API, Multinominal Naive Bayes 모델  
카페 별 게시글 패턴을 분류하기 위해 Google Vision API를 통해 이미지 Labels를 추출하였습니다.
추출된 Labels는 Naive Bayes 모델을 통해 View 맛집과 Menu 맛집으로 분류하였습니다.

### 서울 카페 지도 | HTML, Flask, Kakao map API
kakao map api를 활용하여 지도에 마커를 추가하고 카페 위경도와 대표메뉴, 영업시간 등을 입력하였습니다,또한 마우스 클릭시 팝업창을 띄우는 코드를 구현하였습니다. 

### 카페 챗봇 | Flask, Slack API 
Slack api와 flask 사용하여 슬랙메시지로 지역명과 명령문(뷰맛집, 디저트맛집) 입력시 카페명을 알려주는 코드를 구현하였습니다. <br><br><br>
   
## Contact
* 김경한 https://github.com/darenkim
* 방희란 https://github.com/Heeran-cloud
* 장한아 https://github.com/hannmnnah
* 정혜주 https://github.com/hjung53




