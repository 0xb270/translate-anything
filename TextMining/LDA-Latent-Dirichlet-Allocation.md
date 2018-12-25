[Original](https://ai.stanford.edu/~ang/papers/nips01-lda.pdf)

# 잠재 디리클레 할당

**David M. Blei**, **Andrew Y.Ng** and **Michael I. Jordan**

University of California, Berkeley
Berkeley, CA 94720


## 초록

본 연구는 [나이브베이즈(navie-Bayse)](https://ko.wikipedia.org/wiki/%EB%82%98%EC%9D%B4%EB%B8%8C_%EB%B2%A0%EC%9D%B4%EC%A6%88_%EB%B6%84%EB%A5%98) / [유니그램(unigram), 유니그램 혼합](https://ratsgo.github.io/from%20frequency%20to%20semantics/2017/09/16/LM/), 그리고 [확률론적 잠재 의미론 색인(probabilistic-latent-semantic-indexing; pLSI)](https://en.wikipedia.org/wiki/Probabilistic_latent_semantic_analysis)로도 알려진 호프만의 예측 모델을 포함하여 여러개의 이전 모델보다  일반화 되거나 향상되는 이산형 데이터의 텍스트 및 기타 집합에 대한 생성 모델을 제안한다. 텍스트 모델링의 맥락에서, 우리의 모델은 각 문서가 주제(topics)들이 혼합되어 생성된다는 것을 가정하며, 여기서 연속 값을 갖는 혼합 비율은 잠재 디리클레 확률 변수로 분포된다. 추론과 학습은 변분 알고리즘들(variational-algorithms)을 통해 효율적으로 수행된다. 본 연구는 텍스트 모델링, 협업 필터링 및 텍스트 분류 문제에 이 모델을 적용해본 경험적 결과를 제시한다.


#### Comment
> 이 방법론에서 중요한 포인트는 텍스트 데이터 각각이 명확하게 알려지지는 않았으나 존재하는 어떤 주제들로 구성되어 있다는 것을 가정하여 학습을 통해 이를 분류해 낼 수 있다는 것이다. 

## 1. 서론

최근 몇년간 이산형 데이터를 위한 몇몇 잠재 요인 모델의 개발과 성공적인 적용이 있어왔다. 한가지 주목할만한 예시는 **Hofmann's** pLSI/예측모델로, 많은 연구자들의 주목을 받아왔고, 텍스트 모델링(text-modeling)과 협업 필터링(collaborative-filtering), 그리고 연결 분석(link-analysis)에서의 응용이 부상하였다.
