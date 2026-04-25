# Paper Reading Guide

## Selected Paper
- **Title**: Foundational Models Defining a New Era in Vision: A Survey and Outlook
- **Year**: 2023
- **Venue**: arXiv.org
- **Authors**: Muhammad Awais, Muzammal Naseer, Salman Siddique Khan 외 5명
- **URL**: https://www.semanticscholar.org/paper/584ca135b61482fd89247113da87d784f738dbfa
- **PDF**: https://arxiv.org/pdf/2307.13721
- **Estimated Difficulty**: beginner
- **Citations**: 161
- **Influential Citations**: 8

## Summary
이 논문은 컴퓨터 비전에서 ‘파운데이셔널 모델’이 왜 중요한지, 그리고 이들이 비전·텍스트·오디오·깊이 같은 다양한 모달리티를 어떻게 연결하는지 한 번에 훑어볼 수 있는 서베이입니다. 특히 트랜스포머 관심이 있는 학습자에게는, 단순한 구조 이해를 넘어 멀티모달 결합, 학습 목적함수, 프리트레이닝, 프롬프팅까지 연결해서 보는 데 도움이 됩니다.

## Why Read This Paper
- 비전 분야의 파운데이셔널 모델을 ‘전체 그림’으로 정리한 서베이이므로, 개별 모델보다 큰 흐름을 먼저 잡기에 좋습니다.
- 트랜스포머 관심과 잘 맞는 이유는, 다양한 모달리티를 결합하는 아키텍처 설계를 다루기 때문입니다.
- 학습 목적(contrastive, generative), 데이터셋, 파인튜닝, 프롬프팅 패턴까지 함께 다뤄서 연구 주제를 찾는 데 유용합니다.
- open challenges와 research directions가 포함되어 있어, 다음에 무엇을 읽어야 할지 방향을 잡기 좋습니다.

## Recommended Prerequisites
- 컴퓨터 비전의 기본 개념: 이미지, 객체, 시맨틱/장면 이해 정도
- 트랜스포머의 기본 개념: attention, encoder-decoder, 멀티모달 입력의 직관
- 지도학습과 사전학습(pre-training), 미세조정(fine-tuning)의 차이
- 대조학습(contrastive)과 생성학습(generative)의 아주 기본적인 의미
- 모달리티라는 용어에 대한 이해: 텍스트, 시각, 오디오, 깊이 등

## Suggested Reading Order
- 1) 제목과 초록을 먼저 읽고, 이 서베이가 ‘비전 파운데이셔널 모델의 범위와 쟁점’을 정리하는 글임을 확인합니다.
- 2) 서베이의 목차를 빠르게 훑어, 아키텍처 / 학습 목적 / 데이터셋 / 파인튜닝 / 프롬프팅 / 오픈 챌린지의 구조를 파악합니다.
- 3) 멀티모달 아키텍처 부분에서 ‘어떤 모달리티를 어떻게 결합하는가’만 먼저 잡습니다. 세부 모델명보다 결합 방식에 집중하세요.
- 4) 학습 목적과 프리트레이닝 데이터셋 부분을 읽으며, 모델 성능이 구조만이 아니라 데이터와 목적함수에 의해 좌우된다는 점을 체크합니다.
- 5) 파인튜닝과 프롬프팅 섹션을 읽고, ‘재학습 없이 출력이 어떻게 바뀌는가’라는 관점을 정리합니다.
- 6) 마지막으로 open challenges와 research directions를 읽어, 이 분야의 한계와 연구 공백을 메모합니다.

## What To Focus On
- ‘foundational model’이 일반적인 비전 모델과 무엇이 다른지 한 문장으로 정리해 보세요.
- 아키텍처보다 먼저, 왜 멀티모달 결합이 필요한지를 이해하는 데 집중하세요.
- contrastive vs generative 목적의 차이를 ‘무엇을 배우게 하려는가’ 관점에서 비교해 보세요.
- 프롬프팅 패턴을 읽을 때는, 입력 형식이 어떻게 출력 행동을 바꾸는지에 집중하세요.
- 평가와 벤치마킹의 어려움, 실제 세계 이해의 한계, 편향, adversarial vulnerability, interpretability를 별도로 메모해 두세요.
- 서베이이므로 세부 실험 재현보다 ‘분류 체계와 개념 지도’를 얻는 것이 목표입니다.

## Caution Points
- 초록과 메타데이터만으로는 각 섹션의 구체적 모델 이름, 비교 실험, 정량 성능은 알 수 없습니다.
- 이 논문은 서베이이므로 새로운 단일 방법의 성능을 주장하는 글로 읽으면 안 됩니다.
- ‘포괄적’이라는 표현이 있지만, 실제 포함 범위는 논문 본문과 목차를 확인해야 합니다.
- 벤치마킹, 실제 세계 이해, 편향, adversarial 공격, 해석가능성은 문제 제기 수준일 수 있으니 구체적 해결책이 있는지 본문에서 확인해야 합니다.
- 오디오·깊이 등 여러 모달리티가 언급되지만, 어떤 모달리티가 중심인지 메타데이터만으로는 확정할 수 없습니다.

## Comparison To Previously Read Papers
이전 읽은 논문이 없으므로 직접 비교는 어렵습니다. 다만, 초보자 기준에서는 개별 모델 논문보다 먼저 읽기 좋은 ‘지도(map) 역할’의 서베이입니다. 트랜스포머를 이미 알고 있다면, 이 논문은 attention 메커니즘 자체보다 그것이 멀티모달 비전 시스템에서 어떤 역할을 하는지 확장해서 보는 연습에 적합합니다.
