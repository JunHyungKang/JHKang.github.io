---
title:  "강화학습 - 기본 이론"
excerpt: "Reinforcement learniing - Basic"
toc: true
toc_sticky: true

categories:
  - tech
tags:
  - reinforcement learning

last_modified_at: 2022-08-19T00:00:00-00:00
---

# Reinforcement Learning - 기본 이론 정리

## Intro
### 강화학습?
* Agent가 환경과의 상호작용을 통해 목표를 달성하는 방법을 배우는 문제

### 특징
* 정답을 모른다 (지도학습과 다름)
* 현재의 의사결정이 미래에 영향을 미친다
* 문제의 구조를 모른다 (환경으로부터 정보를 관측 할 수 있음)

### 강화학습과 Agent의 구성요소
* 강화학습: Agent - (action, state, reward) - Enviroment
* Agent: Policy, Value function, Model

### 강화학습의 구분
Model-free, Model-based, Value-based, Policy-based, online RL, offline RL, Inverse RL

## MDP
### Markov Decision Process
* Markov Process or Markov Chain
* Markov Reward Processes: MRP
* Markov Decision Process: MDP

### Markov property
* 미래의 상태는 과거와 무관하게 현재의 상태만으로 결정된다.\
$$P(s_{t+1}|s_t) = P(s_{t+1}|s_t, s_{t-1}, ... , s_0)$$

### State Transition Matrix
상태 천이 행렬: 모든 현재 상태에서 다음 상태로 이동할 확률을 정의한다
* $$P_ss' = P(S_{t+1} = s'|S_t=s)$$

### Markov Reward Processes
MRP는 <$$S$$, $$P$$, $$R$$, $$gamma$$> 인 튜플
* $$S$$은 (유한한) 상태의 집합
* $$P$$는 상태 천이 행렬
* $$R$$는 보상 함수
* $$gamma$$는 감소율

### Return
강화학습 agent가 현재 상태로부터 미래의 일을 고려할 수 있게 해주는 장치





