# LG Aimers 6기 해커톤 - 난임 예측 모델

## 1. 프로젝트 개요

본 프로젝트는 LG Aimers 6기 해커톤의 과제로, 제공된 난임 시술 관련 데이터를 바탕으로 **임신 성공 여부**를 예측하는 모델을 개발하는 것을 목표로 합니다. 다양한 머신러닝 및 딥러닝 모델을 실험하고, 최종적으로 성능이 우수한 앙상블 모델을 구축하였습니다.

## 2. 주제

난임 환자 대상 임신 성공 여부 예측 AI모델 개발

## 3. 데이터셋

- `data/train.csv`: 모델 학습을 위한 데이터
- `data/test.csv`: 예측을 위한 테스트 데이터
- `data/sample_submission.csv`: 제출 양식 파일
- `data/데이터 명세.xlsx`: 데이터셋 명세서

## 4. 파일 설명

- **Baseline(ExtraTrees).ipynb**: ExtraTreesClassifier를 사용한 간단한 베이스라인 모델, 기본적인 pre-processing 및 feature importance 포함
- **Ensemble(xgb+lgbm+catboost)\_Best.ipynb**: **메인 모델**, Multiple Imputation과 Feature Engineering 및 XGBoost, LightGBM, CatBoost를 ensemble한 모델
- **Ensemble(xgb+lgbm+catboost+tabnet).ipynb**: 기본 ensemble 모델에 TabNet을 추가하여 성능 확인
- **Ensemble(xgb+lgbm+catboost+tabpfn).ipynb**: 기본 ensemble 모델에 TabPFN을 추가하여 성능 확인
