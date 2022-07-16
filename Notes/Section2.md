# Section 2. 자연어 처리란?

## 자연어 처리 응용 문제영역
- Machine Translation
  - 하나의 언어를 다른 언어로 번역하는 문제영역
- Sentiment Analysis
  - 문장의 감정상태를 분석해서 긍정/부정, N개의 다른 감정 상태를 분류하는 문제영역
- Spam Filtering
  - 텍스트가 스팸인지 아닌지를 분류하는 문제영역
- Image Captioning
- Text Summarization
  - 텍스트에 대한 요약문을 자동으로 만들어내는 문제영역
- Question Answering
  - 질문에 대한 정답 텍스트를 찾아내는 문제영역
- Dialogue Generation
  - 봇이 자동으로 텍스트를 생성해내는 문제영역

**자연어 처리 문제영역에 기반한 AI 기술의 응용 분야**
- Chatbot : 자동으로 고객 상담을 진행하는 챗봇 기술
- Translation : 자동 번역
- SentimentAnalysis : 고객의 리뷰 텍스트를 통한 Sentiment Analysis
- RecommendationSystem : 고객의 텍스트 로그를 토대로 고객에게 최적화된 품목 추천

## 자연어 처리 용어
*코퍼스(Corpus)* : 말뭉치, 자연어 처리를 위해 모아놓은 텍스트 묶음. 소설, 뉴스기사, 위키피디아 등에서 수집한 텍스트 등이 코퍼스가 될 수 있음.
*토큰(Token)* : 전체 문자열을 분석하고자 하는 단위로 나눈 것. 상황에 따라 문장/단어/형태소 단위가 될 수 있음.
*어휘 집합(Vocavulary Set)* : 처리하는 문제 영역의 전체 단어 집합. 어휘 집합에 포함되지 않은 단어는 <UNK(Unknown)>라는 특수 토큰으로 처리됨.

## 자연어 처리 트렌드 변화
자연어 처리 분야는 전통적으로 확률 통계 기법에 기반한 알고리즘들을 사용하였으나, 한계점이 존재.
따라서 최근에는 딥러닝 기법에 기반한 자연어 처리 기법이 일반적인 트렌드가 됨.
BERT, GPT 등 대규모 모델의 Pre-Training된 파라미터에 Task에 따라 필요한 레이어를 추가하는 Transfer Learning(Fine-Tuning)이 주를 이룸.