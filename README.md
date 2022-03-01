# Revolution6

## **#1 뉴스기사 및 애널리스트 레포트에 대한 감성분석**


<pre>- Sentence: <i>str</i>, 분석할 문장
- Sentiment: <i>str</i>, Positive, Neutral, Negative 여부
</pre>

#### **데이터 불러오기**
<pre><code>data = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution6/master/data/Financial_Sentiment_Analysis.csv', index_col = 0)
</code></pre>

## #2 가짜뉴스에 대한 분류모형 

<pre><code>- title: <i>str</i>, 뉴스제목
- text: <i>str</i>, 뉴스 내용
- subject: <i>str</i>, 뉴스 카테고리
- date: <i>str</i>, 뉴스 일자 
</code></pre>

#### **데이터 불러오기**
<pre><code>fake_df = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/News_Fake_and_Real_Fake.csv')
true_df = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/News_Fake_and_Real_True.csv')
</code></pre>

## **#3 문장에 대한 유사도**

<pre><code>- description_x: <i>str</i>, 문장 x
- description_y: <i>str</i>, 문장 y
- ticker_x: <i>str</i>, 문장 티커 x
- ticker_y : <i>str</i>,  문장 티커 y
- same_security: <i>str</i>, 유사도 여부
</code></pre>

#### **데이터 불러오기**
<pre><code>test = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution6/master/data/text_similarity_test.csv', index_col = 0)
train = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution6/master/data/text_similarity_train.csv', index_col = 0)
</code></pre>


## **#4. 추천시스템 데이터 **

### 4-1) 넷플릭스 데이터
<pre><code>imdb_id : Unique show identifier.
title : Title of the show.
popular_rank : Ranking as given by IMDB when filtered by popularity.
certificate : Contains the age certifications received by the show. Many null values.
startYear : When the show was first broadcasted.
endYear : Year of show ending
episodes : Number of episodes in the show. 1 for movies.
type : Movie or Series
orign_country : Country of origin of the show
language : Language of the show.
plot : Synopsis of the show.
summary : Summary of the story of the show.
rating : Average rating given to the show.
numVotes : Number of votes received by the show.
genres : Genre the show belongs to.
isAdult : 1 If adult content present. 0 if not.
cast : Main cast of the show in list format.
image_url : Link to poster image.
</code></pre>

#### **데이터 불러오기**
<pre><code>df = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/netflix_list.csv')
</code></pre>

### 4-2) user rating data
 
 - The subset of 100,000 ratings from 700 users on 9,000 movies.

<pre><code>user_id : 각 user id
movie_id : 각 movie id
rating : 평점 
timestamp : 평점을 준 시각 
</pre></code>

#### **데이터 불러오기**
<pre><code>df = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution6/master/data/ratings_small.csv')
</code></pre>

