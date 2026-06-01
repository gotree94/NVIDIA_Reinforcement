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
