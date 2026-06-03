# Machine-Learning-Course-Project

- 2026.05.08: Proposal Presentation

- 2026.05.09: Proposal 자료 일부 재구성 (발표 피드백 정리 관련)

- 2026.05.13: 기본 코드 설계(1)

- 2026.05.17: 기본 코드 설계(2) (피드백으로 마스킹 과정이 제대로 설계되지 않음. 3개의 마스킹을 수행하도록 proposal 작성을 진행했으나 code에서는 1개의 과정만 수행함. Robustness 실험에서 source marker removal, named entity masking 누락문제 발생, code가 정량 분석은 진행하였으나 정성 분석은 진행하지 않았다는 문제 발생, Learning curve analysis를 그리지 않았음.)__해당 피드백은 사전 발표에서 작성했던 Proposal 자료에 기반한 것으로 누락된 항목 위주로 체크함.

- 2026.05.19: 5.17의 피드백 반영 (피드백으로 마스킹 과정 중 punctuation_removal, lowercasing, whitespace_normalization을 통합하는게 좋아보임.), 실행 시 A100 GPU 기준으로 90분 정도 소요

- 2026.05.20: 5.19의 피드백 반영, 실행 시 A100 GPU 기준으로 90분 정도 소요 (5.19일 내용과 표현 정리 차이만 존재, 실질적인 수행 과정은 같음.), Cell 8(robustness 관련 피드백: perturbation 입력을 모델별 학습 분포에 맞추도록 수정. 기존에는 raw text를 baseline으로 써서 TextCNN이 대량 OOV로 인해 baseline이 비정상적으로 낮게 측정되고, text_normalization에서 음수 drop이 발생하던 artifact를 제거 필요), Cell 13(indexError 버그 수정, offset을 배치 루프 끝에서 1회만 누적하도록 이동 필요.)

- 2026.05.25: 5.20의 피드백 반영, 실행 시 A100 GPU 기준으로 75분 정도 소요

- 2026.05.31: 자료 정리 및 PPT 

- 2026.06.09: Final Presentation
