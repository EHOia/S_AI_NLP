# Section 4. 언어 모델(Language Modelling) - 다음에 올 단어를 예측해보자

## 언어 모델(Language Modelling)의 개념과 활용사례 - GitHub Copilot
### 언어 모델
앞이나 뒤에 있는 단어나 문장을 통해 다음에 올 단어나 문자를 예측하는 알고리즘
- 수학적으로는 이전 단어들을 토대로 다음에 올 단어의 확률을 예측하는 문제로 볼 수 있음
>"푸른 하늘에 __이 떠있다."라는 문장에서 앞뒤 정보인 "푸른, 하늘, 떠있다"라는 단어를 통해 __에 들어갈 단어가 "구름"이라는 것을 예측

### 언어 모델의 활용사례
- 검색어 자동 완성
- GitHub Copilot
  - 소스코드의 일부분만 입력하면 이후 내용을 자동 완성

## N-Gram 언어 모델
이전에 존재하는 k개의 단어에 기반해서 다음에 올 단어를 예측하는 언어 모델 방법론 (N=k+1)
- N=2인 경우 이전에 존재하는 1개의 단어에 기반해서 다음에 올 단어를 예측, 3일 경우에는 이전에 존재하는 2개의 단어에 기반해 다음에 올 경우를 예측
  - Uni-Gram : 1개의 단어가 한묶음
  - Bi-Gram : 2개의 단어가 한묶음

- N의 개수는 상황마다 다르기 때문에 각 문제에 맞게 적절한 값을 설정해야 함
>7-gram<br/>
P(the | its water is so transparent that)<br/>
: 앞의 6개 단어를 통해 이후 7번째에는 the라는 단어가 올 것을 예측

### N-gram 모델 - Count에 기반한 방법
다음 단어가 올 확률은 해당 단어 조합이 등장한 횟수(Count-C-)에 기반해서 계산

### Count에 기반한 N-Gram 언어 모델 실습
[```N-gram_example.ipynb```](https://github.com/EHOia/S_AI_NLP/blob/main/N-gram_example.ipynb)
