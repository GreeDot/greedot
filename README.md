# 🚀 greedot

<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/7f174a8b-555a-4ebc-9122-f5677ad00ab5">

## 1. skt fly ai challengers 4기 대상 🏆

<img width="633" alt="스크린샷 2024-03-02 144058" src="https://github.com/GreeDot/greedot/assets/120752098/72021669-84c8-4c75-9a2f-b73ec5564f47">

## 2. 시연 영상

[<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/ea200ca6-653b-4622-b2f3-43fc222ba332">](https://www.youtube.com/watch?v=_1cBe-LdLRE)

- <https://www.youtube.com/watch?v=_1cBe-LdLRE>


## 3. 프로젝트 개요
### 3-1. 제안 배경
- 아이가 직접 그린 그림이 말하고 움직이는 나만의 AI친구 생성 서비스
- 아이의 스마트폰 사용 연령은 점점 낮아지고 있는데, 맞벌이 가정은 늘어나면서 아이의 친구를 만들어주는 서비스를 기획하게 되었다.

### 3-2. 목표
- 엔터테인먼트: 흥미 유발을 통하여 사용자에게 즐거움을 선사
- 사회성 향상: 의사소통과 정서 교류가 가능한 AI 단짝 친구 역할
- 정서 모니터링: 대화 기반 분석 리포트를 통한 자녀의 관심사 및 고민 파악 가능

## 4. 시스템 아키텍쳐

<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/1ab2ad98-6712-439f-aa92-e35f5b6b56e8">

### 4-1. 구현 툴
- frontend: **flutter**
- backend: **fastapi**
- cloud: AWS RDS(MySQL), Azure VM, Azure Container(Blob Storage)
- CI/CD: github action, docker

### 4-2. AI, API
- emotion ai: **KoBert emotion predict**
- vision ai: **animated drawings**: <https://github.com/facebookresearch/AnimatedDrawings>
- chat ai: **GPT 3.5-turbo** (finetuning)
- apis: NAVER CLOVA voice, NAVER speech, midjourney api

## 5. 기술
### 5-1. 리깅

<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/4fd6044f-5e6f-4485-9b8e-779469cfde1e">

<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/6509452b-9020-4c76-8498-53e1c72f274d">


- 동영상에서 인간 관절 좌표 추출 후 캐릭터에 적용


### 5-2. 감정 분류
- 6가지 감정 상황에 따른 대화 데이터 약 8만개 문장으로 KoBERT 학습
- fine tuning, 데이터 이상치 제거, 모델 앙상블을 통한 정확도 향상(test val: 77%)

### 5-3. GPT 파인튜닝
- gpt 3.5 모델을 활용, 약 70개 대화 파인튜닝 및 페르소나 적용
- 성격, 성별에 따라 다양한 스타일의 목소리 제공

## 6. 팀원 소개

| 이름   | 역할                                       | 구현                                       |
| ------ | ------------------------------------------ | ------------------------------------------ |
| [변지협](https://github.com/rimgosu) 🤨 | **팀장**, 백엔드, 클라우드    | CI/CD 파이프라인 구축 |
| [이성원](https://github.com/2Swon) 😊 | 백엔드, 프론트엔드 | 그림 업그레이드 기능 구현 |
| [김동욱](https://github.com/donguk071) 😁 | Vision AI                     | 캐릭터 리깅 기능 구현 |
| [김동재](https://github.com/dongjaee) 😘 | 프론트엔드, 감정 AI               | STT, GPT 파인튜닝 |
| [문지우](https://github.com/Moonjiwoojdjeiwnwh) 😯 | 프론트엔드, 언어 AI             | 감정분석 기능 구현 |


## 7. Link
- **아보카도 노션**: <https://cuddly-spinach-1a9.notion.site/90bdc1a12dcd4e79a551be74e0b76196?pvs=25>
- **최종 발표 자료**: [https://github.com/GreeDot/greedot/blob/main/assets/greedot_ppt.pdf](https://github.com/GreeDot/greedot/blob/main/assets/%EC%B5%9C%EC%A2%85PPT_%EA%B7%B8%EB%A6%AC%EB%8B%B7.pdf)
- **Backend Server(Dockerhub)**: <https://hub.docker.com/repository/docker/newnyup319/greedot-backend/general>
- **AI Server(Dockerhub)**: <https://hub.docker.com/repository/docker/newnyup319/greedot-ai/general>
