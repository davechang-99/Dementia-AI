# Audio Classification for Dementia Detection

## 프로젝트 소개
이 프로젝트는 오디오 데이터를 '정상(Normal)' 또는 '치매(Dementia)'로 분류하는 머신러닝 모델을 개발합니다. 음성 데이터를 멜-스펙트로그램(Mel-spectrogram) 이미지로 변환하여 딥러닝 모델에 적용하는 방식으로 진행됩니다.

## 주요 기능 및 기술 스택
- **데이터 전처리**: `.wav` 형식의 음성 파일을 `.png` 형식의 멜-스펙트로그램 이미지로 변환.
- **데이터셋**: 'Normal' 및 'Dementia' 클래스로 구성된 훈련 및 검증 데이터셋.
    - **데이터셋 링크**: [Google Drive Dataset](https://drive.google.com/drive/folders/14w2K2GedTDCQUrcLqzZk6rhBrCFX1uCD?usp=drive_link)
- **모델 아키텍처**:
    - Convolutional Neural Network (CNN)
    - Vision Transformer (ViT)
    - Random Forest (클래식 머신러닝 모델)
- **학습**: PyTorch를 사용하며, 이미지 데이터에 대한 데이터 증강(Data Augmentation) 기법 적용.
- **성능 평가**: 정확도(Accuracy), 혼동 행렬(Confusion Matrix), ROC 커브 등을 활용하여 모델 성능 분석.

## 사용법
1. GitHub 저장소를 클론(Clone)합니다.
2. 필요한 패키지를 설치합니다.
3. Jupyter Notebook 파일을 실행하여 데이터 전처리부터 모델 학습 및 평가 과정을 확인할 수 있습니다.
