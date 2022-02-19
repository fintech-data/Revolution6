# Revolution6

## **#1 뉴스기사 및 애널리스트 레포트에 대한 감성분석**


<pre>- Sentence: <i>str</i>, 분석할 문장
- Sentiment: <i>str</i>, Positive, Neutral, Negative 여부
</pre>

#### **데이터 불러오기**
<pre><code>data = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution6/master/data/Financial_Sentiment_Analysis.csv', index_col = 0)
</code></pre>

## **#2 가짜뉴스에 대한 분류모형 **

<pre><code>- title: <i>str</i>, 뉴스제목
- text: <i>str</i>, 뉴스 내용
- subject: <i>str</i>, 뉴스 카테고리
- date: <i>str</i>, 뉴스 일자 
</code></pre>

#### **데이터 불러오기**
<pre><code>fake_df = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/News_Fake_and_Real_Fake.csv')

true_df = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/News_Fake_and_Real_True.csv')
</code></pre>

## #3. CNN 뉴스 요약 

<pre><code>- id: <i>str</i>, id
- article: <i>str</i>, 기사 본문
- highlights: <i>str</i>, 요약본
</code></pre>

#### **데이터 불러오기**
<pre><code>cnn_train = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/cnn_daily_mail_train.csv')
cnn_val = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/cnn_daily_mail_validation.csv')
cnn_test = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution6/master/data/cnn_daily_mail_test.csv')
</code></pre>

## **#4 문장에 대한 유사도**

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
