# NVIDIA Reinforcement Learning

---

## 🤖 Robotics RL (Isaac Lab 중심)

### 1. Getting Started With Isaac Lab (공식 NVIDIA 학습 과정)
👉 https://docs.nvidia.com/learning/physical-ai/getting-started-with-isaac-lab/latest/

**공식 커리큘럼으로 구성이 잘 되어 있으며, 다음 모듈로 구성됩니다:**
   * An Introduction to Robot Learning and Isaac Lab — RL 개념, Isaac Gym → Isaac Sim → Isaac Lab 역사
   * Train Your First Robot in Isaac Lab — Cartpole 환경으로 첫 RL 학습
   * Train Your Second Robot in Isaac Lab — 커스텀 Reward 함수 설계
   * Transferring Robot Learning Policies from Simulation to Reality — Sim-to-Real 전략 

### 2. Isaac Lab 공식 문서 & GitHub
👉 https://developer.nvidia.com/isaac-lab
   * Isaac Lab은 GPU 가속 기반의 모듈식 로봇 학습 프레임워크로, PhysX, Newton, Warp, MuJoCo 등
   * 다양한 물리 엔진을 지원하며 모방 학습과 강화 학습을 모두 커버합니다.
   * Isaac GR00T 플랫폼의 기반 프레임워크이기도 합니다.

---

## 🧠 LLM/Post-Training RL (NeMo RL 중심)

### 3. NeMo RL 공식 문서
👉 https://docs.nvidia.com/nemo/rl/latest/index.html
   * NeMo RL은 멀티모달 모델(LLM, VLM)을 위한 오픈소스 post-training 라이브러리로,
   * DTensor/Megatron Core 백엔드 Quick Start, 새 모델 아키텍처 추가 방법,
   * YaRN Long-Context Training 등 심화 내용을 포함합니다. 

### 4. NeMo-RL GitHub + 블로그 튜토리얼
👉 https://developer.nvidia.com/blog/reinforcement-learning-with-nvidia-nemo-rl-reproducing-a-deepscaler-recipe-using-grpo/

   * GRPO 알고리즘을 활용해 Qwen-1.5B 모델을 학습하여 AIME 2024 수학 벤치마크에서 OpenAI O1에 근접한 성능을 달성한 사례를 다룹니다.
   * GitHub에서 예제 스크립트와 설정 파일을 직접 확인할 수 있습니다. 

### 5. NeMo Gym (환경 라이브러리)
👉 https://github.com/NVIDIA-NeMo/Gym

   * NeMo Gym은 REST API 기반의 확장 가능한 학습 환경과 Model/Resources/Agents 추상화를 제공하며,
   * NeMo RL과 함께 GRPO, on-policy distillation, asyncRL, FP8 RL 학습을 지원합니다. 

---

## 🚀 Jetson 기반 로봇 RL (임베디드 환경)

### 6. jetson-reinforcement (GitHub)
👉 https://github.com/dusty-nv/jetson-reinforcement

   * Jetson TX1/TX2용 Deep RL 라이브러리로, PyTorch, OpenAI Gym, Gazebo 시뮬레이터를 사용해 가상 시뮬레이션에서
   * RL 에이전트를 훈련하고 실제 로봇으로 transfer하는 것을 목표로 합니다. DQN 알고리즘 노트북도 포함되어 있습니다.

## 📌 추천 학습 순서 (교수님 상황 기준)

| 단계 | 리소스 | 목적 | 
|:-------:|:-------:|:-------:|
| 1 | Getting Started with Isaac Lab | RL 개념 + Isaac Lab 실습 기초 | 
| 2 | Isaac Lab GitHub Docs | TurtleBot | 
| 3 | 환경 커스텀3NeMo RL 공식 문서 | GRPO/RLHF 이론 심화 | 
| 4 | NeMo Gym | 에이전트 환경 설계 | 

---

## ✅ NVIDIA DLI 무료 RL 관련 과정

### 🆓 완전 무료 — Robotics Fundamentals Learning Path
👉 https://nvidia.com/en-us/learn/learning-path/robotics

* "Start Your Free Learning Path" 버튼이 있는 완전 무료 경로로, 다음 섹션으로 구성됩니다:
   * Robotics Foundations — 로보틱스 핵심 개념 강의
   * Getting Started With Isaac Sim — Isaac Sim 기초, ROS 2 연동, 합성 데이터 생성
   * Getting Started With Isaac Lab — 로봇 학습(RL/Imitation Learning) 고급 개념 실습
   * Getting Started With Isaac ROS — NVIDIA Isaac ROS 프레임워크
   * Getting Started With Isaac for Healthcare — 의료 로봇 워크플로우 nvidia

* 이 중 "Getting Started With Isaac Lab" 섹션이 바로 RL을 다루는 핵심 파트입니다.

### 📋 무료 과정 직접 링크

| 과정명 | URL | 가격 | 
|:---------:|:---------:|:---------:|
| An Introduction to Robot Learning and Isaac Lab | learn.nvidia.com → DLI+S-OV-36+V1 | 🆓 Free | 
| Train Your First Robot in Isaac Lab | learn.nvidia.com → DLI+S-OV-46+V1 | 🆓 Free | 
| Simulating Your First Robot in Isaac Sim | learn.nvidia.com → DLI+S-OV-27+V1 | 🆓 Free | 
| A Beginner's Guide to Autonomous Robots | learn.nvidia.com → DLI+S-OV-35+V1 | 🆓 Free | 

## 💡 추가 팁 — 교수님 입장에서 활용 가능한 것
* NVIDIA DLI는 Teaching Kit를 제공하는데, 교수자가 신청하면 최대 200명 학생에게 무료 DLI 과정 접근 코드를 발급받을 수 있습니다.
* 강의 슬라이드, 영상, 퀴즈/시험 문제 세트와 정답까지 포함된 학기 단위 커리큘럼 자료도 함께 제공됩니다.

* 광주 인재개발원 강의에 학생들과 함께 활용하기 딱 좋은 루트입니다!
* Teaching Kit 신청은 https://www.nvidia.com/en-us/deep-learning-ai/education/ 에서 할 수 있어요.

## ✅ DLI 무료 과정 = 로컬 GPU 불필요
   * NVIDIA DLI 자기 주도 학습 과정에 등록하면 클라우드 기반 GPU 실습 환경에 대한 접근 권한이 제공됩니다.
   * 필요한 것은 컴퓨터와 인터넷 연결뿐입니다.

   * NVIDIA가 직접 완전히 구성된 GPU 가속 클라우드 서버를 실습용으로 제공하며,
   * 해당 환경은 NVIDIA NGC 카탈로그에서 제공되는 DLI 기본 환경 컨테이너와 동일합니다.

   * 각 과정에는 클라우드의 GPU 가속 워크스테이션에 접근할 수 있는 자기 주도 학습 환경이 포함되어 있으며,
   * 수강생은 웹 브라우저와 인터넷 연결만 있으면 시작할 수 있습니다. NVIDIA Developer

## ⚠️ 단, 로보틱스 RL 과정은 예외 가능성 있음

   * 일반 딥러닝/데이터사이언스 과정과 달리, Isaac Sim 기반 RL 과정은 상황이 다릅니다.

   * Isaac Sim 자체가 RTX GPU + 대용량 RAM을 요구하는 렌더링 시뮬레이터라서,
   * DLI "Getting Started with Isaac Lab" 시리즈는 이론 강의 + 문서 기반으로 구성되어 있고,
   * 실제 Isaac Sim 실행은 로컬 환경(교수님의 ROG SCAR 16 같은)에서 하도록 안내하는 구조입니다.

   * 즉:
| 과정 유형 | 클라우드 GPU 제공 | 로컬 GPU 필요 |
|:---------------:|:---------------:|:---------------:|
| 일반 DL/ML 과정 (Fundamentals of DL 등) | ✅ | ❌ | 
| CUDA / 가속 컴퓨팅 과정 | ✅ | ❌ | 
| Isaac Sim / Isaac Lab RL 과정 | ⚠️ 이론 위주 | 실습은 로컬 권장 | 


