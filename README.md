# health_policy
2022 SKKU ML project

0. 발표자료<br/>
  지금까지 발표하는데 사용된 PDF 자료들이 있습니다. 12월 2일 마지막 발표에는 코랩과 주피터노트북 파일을 주로 사용했기에 따로 첨부하지 않았습니다.<br/>

1. 선행연구논문<br/>
  기존에 빅데이터분석 및 머신러닝을 이용해 정책 제언 및 동향을 연구한 자료가 있습니다. 또한, BERT 모델 관련 자료들이 포함되어 있습니다.<br/>

2. 원본데이터셋<br/>
  단어사전 구축을 위한 문서(dictionary_docs), 크롤링 코드를 이용해 수집한 네이버 블로그(naver_blog_data), 네이버 뉴스 데이터(naver_news_data)가 포함되어 있습니다.<br/>

3. 원본코드<br/>
  3.0 크롤링코드<br/>
    네이버 뉴스와 네이버 블로그 게시글을 크롤링하는데에 사용한 코드입니다. (네이버뉴스크롤링/블로그 크롤링)<br/>
  3.1 전처리코드<br/>
    보건정책관련 단어사전 구축을 위한 코드와 앞서 수집한 크롤링 데이터를 전처리한 코드로 구성되어 있습니다. (making_worddictionary -> blog_preprocessing/news_preprocessing -> data_analysis)<br/>
  3.2 분석모델코드<br/>
    앞서 전처리를 완료한 데이터를 입력하여 분석결과를 도출한 코드입니다. (korean keybert/KoreanBertopic/word2vector)<br/>

4. 데이터셋 및 라이브러리<br/>
  4.0 csv<br/>
    전처리 과정을 거쳐 토큰화한 컬럼을 추가한 데이터프레임을 포함하고 있습니다.(blog_data, news_data)<br/>
  4.1 pickle<br/>
    보건정책관련 문서에서 추출한 단어사전(word_dictionary)<br/>
    input을 위해 space로 구분한 토큰화완료된 리스트형 데이터(blog_nv, news_nv)<br/>
    input을 위해 comma로 구분한 토큰화된 리스트형 데이터(blog_cs, news_cs)<br/>
    input을 위해 comma로 구분한 토큰화된 데이터를 하나의 string 형태로 저장한 데이터(blog_cs_sum, news_cs_sum) 으로 구성되어 있습니다.<br/>
  4.2 사용라이브러리<br/>
    전체 코드를 작성하는데 사용한 라이브러리입니다.<br/>

5. 최종보고서<br/>
  최종보고서 파일입니다.<br/>

6. appendix<br/>
  데이터 수집 관련 내용(appendix_data)와 wordcount, wordcloud와 word2vec 모델을 구현하고 시각화한 내용(appendix_추가보고서)로 이루어져있습니다.<br/>
