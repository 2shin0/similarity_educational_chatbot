# 임베딩의 개념과 유사도 기반 학습 챗봇 구현

## ✅ 임베딩이란?
임베딩(Embedding)은 자연어 처리에서 사람이 쓰는 자연어를 기계가 이해할 수 있도록 숫자의 나열인 벡터 형태로 바꾸는 과정입니다. 고차원 데이터를 저차원 공간으로 변환하여 의미 있는 벡터 표현을 생성하는 기법으로, 데이터의 의미적 특성을 보존하면서 데이터를 보다 효율적으로 처리할 수 있게 해줍니다. 예를 들어 king과 queen은 벡터 공간에서 비슷한 위치에 있게 됩니다.

### 📌 벡터 간 거리 계산 방법
1. 코사인 유사도<br>
벡터의 방향(각도)을 기반으로 유사성을 측정합니다. 두 벡터가 동일한 방향을 가질수록 유사도가 높습니다.
![image](https://github.com/user-attachments/assets/9c75aadf-affd-4d55-96ea-4aad5d5b2149)
2. 유클리드 거리<br>
벡터 간의 실제 거리를 측정합니다. 거리가 짧을수록 유사성이 높습니다.

### 📌 임베딩 모델마다 성능이 다른 이유?
모델마다 아키텍쳐와 사전 학습시킨 훈련 데이터가 다르기 때문에 나의 목적에 따라 적합한 모델이 달라질 수 있습니다. 따라서 원하는 도메인 또는 서비스에서 좋은 성능을 보이는 모델을 선택해야 합니다.

## ✅ 실습1 : Huggingface의 사전 학습된 임베딩 모델로 유사도 기반 챗봇 만들어 보기
[실습1 코드](https://github.com/2shin0/similarity_educational_chatbot/blob/main/embedding_chat.ipynb) <br>
활동 1. 알맞은 형식으로 데이터셋 생성 <br>
활동 2. 적합한 모델을 선택하여 유사도 계산 함수 생성 <br>
활동 3. Gradio로 간단한 챗봇 구현

## ✅ 실습2 : BM25 + Embedding 앙상블 모델로 유사도 기반 챗봇 만들어 보기
[실습2 코드](https://github.com/2shin0/similarity_educational_chatbot/blob/main/BM25_Embedding_chat.ipynb) <br>
활동 1. BM25와 Embedding 모델 각각 답변 확인 <br>
활동 2. 앙상블 모델 생성 <br>
활동 3. Gradio로 간단한 챗봇 구현

## ✅ 실습3 : BM25 + Faiss 앙상블 모델로 유사도 기반 챗봇 만들어 보기
[실습3 코드](https://github.com/2shin0/similarity_educational_chatbot/blob/main/3_BM25_Faiss_chat.ipynb) <br>
활동 1. BM25와 Faiss 각각 답변 확인 <br>
활동 2. 앙상블 모델 생성 
