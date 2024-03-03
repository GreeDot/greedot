# 🚀 GreeDot

![GreeDot Project Image](https://github.com/GreeDot/greedot/assets/120752098/7f174a8b-555a-4ebc-9122-f5677ad00ab5)

GreeDot is a project brings life to children's drawings by creating "Meta Characters".
Enjoy various interaction with your characters!!

## 1. SKT Fly AI Challengers 4th Generation Grand Prize 🏆

![SKT Fly AI Challengers Award](https://github.com/GreeDot/greedot/assets/120752098/72021669-84c8-4c75-9a2f-b73ec5564f47)

## 2. Demonstration Video

[![Demonstration Video](https://github.com/GreeDot/greedot/assets/120752098/ea200ca6-653b-4622-b2f3-43fc222ba332)](https://www.youtube.com/watch?v=_1cBe-LdLRE)

- [Video Link](https://www.youtube.com/watch?v=_1cBe-LdLRE)

## 3. Project Overview
### 3-1. Background
- A service that creates a personal AI friend that talks and moves, based on drawings made by children themselves.
- With the age of smartphone use by children getting lower and the increase in dual-income families, we planned a service that creates friends for children.

### 3-2. Goals
- Entertainment: Provide joy through engaging user experiences.
- Social Skills Improvement: Serve as an AI buddy capable of communication and emotional exchange.
- Emotional Monitoring: Identify the child's interests and concerns through conversation-based analysis reports.

## 4. System Architecture

![System Architecture](https://github.com/GreeDot/greedot/assets/120752098/1ab2ad98-6712-439f-aa92-e35f5b6b56e8)

### 4-1. Implementation Tools

| Category  | Technologies                                        |
|-----------|-----------------------------------------------------|
| Frontend  | Flutter                                             |
| Backend   | FastAPI                                             |
| Cloud     | AWS RDS (MySQL), Azure VM, Azure Container (Blob Storage) |
| CI/CD     | GitHub Actions, Docker                              |

### 4-2. AI, API

| Category                 | Technologies/Services                              |
|--------------------------|----------------------------------------------------|
| Emotion AI               | KoBert emotion predict                             |
| Vision AI & Rendering    | Animated drawings                                  |
| Chat AI                  | GPT 3.5-turbo + finetuning                         |
| APIs                     | NAVER CLOVA voice, NAVER speech, Midjourney API    |

## 5. Technologies
### 5-1. Rendering (rigging + retargeting)

- Tech flow
  - Animation (.bvh) creation algorithm using MediaPipe
  - Rigging + Retargeting
  - Applying animations to characters through Animated Drawings Renderer

### 5-2. Emotion Classification
- Trained KoBERT on about 80,000 sentences for six emotional situations
- Improved accuracy through fine-tuning, outlier data removal, and model ensembling (test validation: 77%)

### 5-3. GPT Fine Tuning
- Utilized GPT 3.5 model for fine-tuning about 70 conversations and applying personas
- Provides various styles of voices based on personality and gender

## 6. Team Members

| Name   | Role                                       | Implementation                                       |
| ------ | ------------------------------------------ | ---------------------------------------------------- |
| [Byeon Ji-hyeop](https://github.com/rimgosu) 🤨 | **Team Leader**, Backend, Cloud    | CI/CD Pipeline Construction |
| [Lee Seong-won](https://github.com/2Swon) 😊 | Backend, Frontend | Drawing Upgrade Feature Implementation |
| [Kim Dong-wook](https://github.com/donguk071) 😁 | Vision AI                     | Character Rigging Feature Implementation |
| [Kim Dong-jae](https://github.com/dongjaee) 😘 | Frontend, Emotion AI               | STT, GPT Fine-tuning |
| [Moon Ji-woo](https://github.com/Moonjiwoojdjeiwnwh) 😯 | Frontend, Language AI             | Emotion Analysis Feature Implementation |

## 7. Links

- [**Avocado Notion**](https://cuddly-spinach-1a9.notion.site/90bdc1a12dcd4e79a551be74e0b76196?pvs=25)
- [**Final Presentation Material**](https://github.com/GreeDot/greedot/blob/main/assets/%EC%B5%9C%EC%A2%85PPT_%EA%B7%B8%EB%A6%AC%EB%8B%B7.pdf)
- [**Backend Server (Dockerhub)**](https://hub.docker.com/repository/docker/newnyup319/greedot-backend/general)
- [**AI Server (Dockerhub)**](https://hub.docker.com/repository/docker/newnyup319/greedot-ai/general)
