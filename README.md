# greedot

<img width="633" alt="image" src="https://github.com/GreeDot/greedot/assets/120752098/7f174a8b-555a-4ebc-9122-f5677ad00ab5">

## 1. skt fly ai challengers 4기 대상

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

- frontend: **flutter**
- backend: **fastapi**
- cloud: AWS RDS, Azure VM
- file: Azure Container
- CI/CD: github action, docker
- emotion ai: KoBert emotion predict
- vision ai: animated drawings
- chat ai: GPT 3.5-turbo (finetuning)
- apis: NAVER CLOVA voice, NAVER speech, midjourney api

## 4-1. 리깅
