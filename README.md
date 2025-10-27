🏆 SSAFY AI 챌린지: VQA 모델 성능 혁신 보고서
💡 프로젝트 개요 (Visual Question Answering)
본 프로젝트는 SSAFY AI 챌린지에서 제시된 Visual Question Answering (VQA) 모델 개발 미션을 수행한 결과물입니다.

미션 주제: 이미지 기반 질의응답 (VQA) 모델 개발

핵심 모델: Qwen3-VL-8B-Instruct (Fine-tuning 적용)

주요 기술: PEFT (LoRA), 4-bit Quantization, Hyperparameter Optimization

🚀 최종 성과 (Public Score 17.64%p 향상)
제공된 베이스라인 대비 17.64%p의 유의미한 성능 향상을 달성하였으며, 이는 모델의 잠재력을 극한으로 끌어올린 결과를 입증합니다.

Public Score 개선: 베이스라인 0.76028 → 최종 0.93672

개선 폭: 17.64%p 성능 향상 달성

🛠️ 베이스라인 진단 및 최적화 전략
초기 베이스라인 코드의 기술적 한계를 식별하고, 다음과 같은 세 가지 핵심 전략을 적용하여 성능 혁신을 추진하였습니다.

1. 모델 아키텍처 혁신
진단: Qwen2.5-VL-3B의 VQA 복잡성 처리 능력 부족

개선: Qwen3-VL-8B로 모델 교체 및 AutoModelForImageTextToText 로딩

효과: 모델의 표현력 및 추론 정확도 대폭 확장

2. 프롬프트 및 명령어 템플릿 정교화
진단: 베이스라인의 단순한 명령어 구조로 인해 모델의 추론 과정이 불명확

개선: Chain-of-Thought (CoT) 유도 및 명확한 출력 형식 지정 프롬프트 설계

효과: 모델의 상황 인지 및 답변 형식 안정화로 최종 정확도 개선

3. 학습 안정화 및 파이프라인 최적화
진단: 기본적인 Fine-tuning 설정만 적용되어 학습 안정성이 낮음

개선: Warmup 및 Weight Decay 재설정을 통한 학습 파이프라인 안정화

효과: 초기 Loss 수렴 가속화 및 과적합 제어

⚙️ 기술 스택 (Technical Stack)
핵심 모델: Qwen3-VL-8B-Instruct (80억 파라미터 기반의 Instruction-tuned Multimodal LLM)

프레임워크: PyTorch, Hugging Face Transformers (딥러닝 모델 구현 및 환경 운영)

최적화 기법: PEFT (LoRA), 4-bit Quantization (GPU 메모리 효율화 및 경량 Fine-tuning 적용)

학습 전략: Cosine Annealing with Warmup, Weight Decay (최적의 모델 수렴을 위한 스케줄링 및 정규화)
