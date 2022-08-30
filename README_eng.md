## About the Project
### How do you find coffee shops?☕️ 
What search engines do you use? And what types of keywords do you use? We can help you find a coffee shop with the aesthetic or good pastry selection
__#coffeegram, #coffeelover, #cafeseoul__. With __Seoul Café Map__ and __Café Chatbot__, we can help your coffee shop in Seoul!
 
#### It became a ritual for our generation to post a picture of a cup of coffee after spending a lovely afternoon at a coffee shop  [#coffeegram]. 
Thanks to our collective efforts to display the love of coffee shops, we often use Instagram to search and check out the coffee shops before visiting. When looking at the search results, we can view the kind of experience the coffee shop provides, such as the aesthetic and the popular drinks. For example, below is the search result for coffee shop mk2 in south Korea. Can you sense the vibe that the coffee shop offers when looking at people's posts?

<img width='50%' src='https://user-images.githubusercontent.com/42338386/106733676-8421e800-6655-11eb-8750-af5f6b456fb3.png'> 

We often visit the coffee shops we find on Instragram to experience the #coffeegram. 
For those of you who use instagram to find your coffee shops, we have created #coffeegram based __Seoul Cafe Map 🗺 & Chatbot 🗣__.
We can show what you would expect from the coffee shops by classifying the cafes into either aesthetically or foodwise instagrammable cafes and displaying representative images.

## Seoul Cafe Map 🗺 & Chatbot 🗣

__Seoul Cafe Map__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105575023-bb69dc80-5dab-11eb-8856-2cc0e49d1fc1.gif'>

__Seoul Cafe Chatbot__  

<img width='70%' src='https://user-images.githubusercontent.com/42338386/105578468-c7619880-5dc3-11eb-9a04-e7943c601fd8.gif'>


   
## Built with
__Selenium, MongDB, Flask, AWS, Multinominal Naive Bayes, Google Vision API, BS4, Kakao map API, HTML__



## Structure

<img src="https://user-images.githubusercontent.com/42338386/107241046-f0de1d80-6a6d-11eb-8697-ddce5065ae88.png" width="70%">


## Methods
### #Instagram Cafe Crawling | BS4, Selenium, AWS, boto3
The Instagram posts that hashtag the coffee shops capture the aesthetic and the most popular items. We crawled images(without people’s faces), hashtags, number of likes, etc. using Selenium. 

<img src="https://user-images.githubusercontent.com/42338386/106738618-7ff8c900-665b-11eb-9abc-f042b629643f.png" width='70%'>


### Extracting Patterns and Cafe Aesthetics from the images| Google Vision API, Multinominal Naive Bayes Classifier  
To determine if the cafe appeals to the customers looking for aesthetics or foods, we extracted image labels using Google Vision API. If the images of cafe are associated with more labels such as building, architecture than food related labels such as coffee, the cafe was categorized as a instagrammable cafe for its aesthetics. We used Naive Bayes model to classify the cafes into two groups. 
Using the hashtag comments, we were able to extract signature food and beverages, locations, and etc. 


### Seoul Cafe Map | HTML, Flask, Kakao map API
We used Kakao Map API to display the add markers to the map, popular food and beverages, and the hours. These informations are shown on pop-ups that could be accessed through clicking the markers.  

### Seoul Cafe Chatbot | Flask, Slack API 
Using Slack API and Flask, we have implemented a chat bot where if you enter area and the cafe type (e.g. [bot] YongSan: asthetic cafes), you will receive a list of cafes in the area that are consistent to the type of cafes that you are looking for.  <br><br><br>
   
## Contact
* Daren Kim https://github.com/darenkim
* Heeran Bang https://github.com/Heeran-cloud
* Hannah Jang https://github.com/hannmnnah
* HyeJoo Jung https://github.com/hjung53




