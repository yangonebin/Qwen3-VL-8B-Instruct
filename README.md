🏆 SSAFY AI 챌린지: VQA 모델 성능 혁신 보고서

💡 프로젝트 개요 (Visual Question Answering)

본 프로젝트는 $\text{SSAFY}$ $\text{AI}$ 챌린지에서 제시된 Visual Question Answering ($\text{VQA}$) 모델 개발 미션을 수행한 결과물입니다. 이미지와 자연어 질문을 동시에 처리하는 멀티모달 $\text{AI}$ 모델을 개발하고, 제공된 베이스라인의 성능을 분석 및 최적화하여 리더보드 순위를 상위권으로 향상시키는 것을 목표로 하였습니다.

미션 주제: 이미지 기반 질의응답 ($\text{VQA}$) 모델 개발

핵심 모델: $\text{Qwen3-VL-8B-Instruct}$ ($\text{Fine-tuning}$ 적용)

주요 기술: $\text{PEFT}$ ($\text{LoRA}$), $\text{4-bit Quantization}$, $\text{Hyperparameter}$ $\text{Optimization}$

🚀 최종 성과 (Public Score $17.64\%p$ 향상)

제공된 베이스라인 대비 $\mathbf{17.64%p}$의 유의미한 성능 향상을 달성하였으며, 이는 $\text{AI}$ 엔지니어링 역량을 통해 모델의 잠재력을 극한으로 끌어올린 결과를 입증합니다.

지표

베이스라인 점수

최종 Public Score

개선 폭

Public Score

$0.76028$

$\mathbf{0.93672}$

$\mathbf{17.64\%p}$

순위

-

캠퍼스 $\mathbf{3}$위 달성

(경쟁 환경에서의 문제 해결 능력 입증)

🛠️ 베이스라인 진단 및 최적화 전략

초기 베이스라인 코드의 기술적 한계를 식별하고, 다음과 같은 세 가지 핵심 전략을 적용하여 성능 혁신을 추진하였습니다.

전략 구분

베이스라인 한계 진단

적용된 개선 전략

기술적 효과

1. 모델 아키텍처

Qwen2.5-VL-3B의 VQA 복잡성 처리 능력 부족

Qwen3-VL-8B로 모델 교체 및 AutoModelForImageTextToText 로딩

모델의 표현력 및 추론 정확도 확장

2. 데이터 활용

학습 데이터 200개 샘플로 제한적인 학습 진행

전체 학습 데이터셋 $\mathbf{100\%}$ 활용

모델 일반화 능력 강화 및 데이터 편향 최소화

3. 학습 안정화

기본적인 Fine-tuning 설정

Warmup 및 Weight Decay 재설정을 통한 학습 파이프라인 안정화

초기 Loss 수렴 가속화 및 과적합 제어

⚙️ 기술 스택 (Technical Stack)

구분

주요 기술 스택

설명

핵심 모델

$\text{Qwen3-VL-8B-Instruct}$

80억 파라미터 기반의 $\text{Instruction-tuned}$ $\text{Multimodal}$ $\text{LLM}$

프레임워크

$\text{PyTorch}$, $\text{Hugging Face}$ $\text{Transformers}$

딥러닝 모델 구현 및 $\text{Model/Tokenizer}$ 운영 환경

최적화

$\text{PEFT}$ ($\text{LoRA}$), $\text{4-bit Quantization}$

$\text{GPU}$ 메모리 효율화 및 경량 $\text{Fine-tuning}$ 기법 적용

학습 전략

$\text{Cosine Annealing with Warmup}$, $\text{Weight Decay}$

최적의 모델 수렴을 위한 $\text{Learning Rate}$ 스케줄링 및 정규화
