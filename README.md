# Dementia Pre-detection AI: Mel-Spectrogram Voice Classification

본 프로젝트는 음성 데이터를 Mel-Spectrogram 이미지로 변환한 후,  
딥러닝 및 기계학습 기반의 분류 모델(CNN, ViT, RandomForest 등)을 활용하여  
치매 환자와 정상 노인을 구분하는 인공지능 모델 개발 및 실험을 목표로 합니다.

## 📚 주요 특징
- 음성 파일을 Mel-Spectrogram 이미지로 자동 변환
- PyTorch, Transformers(Huggingface), scikit-learn 기반 다양한 분류기 지원
- 성능 비교: CNN, ViT(Vision Transformer), RandomForest
- 실험 결과 표, 시각화, 혼동행렬, ROC 곡선 등 자동 생성
- Colab/Jupyter 환경에서 즉시 재현 가능

---

## 🔥 실행 방법

1. **Google Colab에서 실행 권장**  
   (또는 Jupyter 환경)
2. 필요한 라이브러리 설치  
   (Colab의 경우 ipynb 첫 셀에서 자동 설치)
3. Google Drive에 데이터셋 업로드  
   ## 📂 Google Drive

- [프로젝트 데이터 및 파일 폴더 바로가기](https://drive.google.com/drive/folders/1WHmpintD0IiBifRBx2IPOTMS5_rPo8bH?usp=drive_link)
4. 각 셀을 순서대로 실행


---

## 💾 데이터셋 안내

- 본 프로젝트는 공개 영어권 치매 음성 데이터셋(예: DementiaBank, Pitt Corpus 등)을 예시로 사용하였습니다.
- 실제 한국어 음성 데이터셋은 공개 DB 부족으로 분석에 활용하지 못하였으며,  
  연구 확장 시 별도 구축 필요
- 각 폴더별 `.wav` 파일 형식(정상: `Normal/`, 치매: `Dementia/`)

---

## 🏆 실험 결과 예시

| Model         | Accuracy | Precision | Recall   | F1-Score |   AUC    |
|---------------|----------|-----------|----------|----------|----------|
| ViT           | 0.610    | 0.628     | 0.610    | 0.603    | 0.721    |
| RandomForest  | 0.616    | 0.615     | 0.616    | 0.614    | 0.692    |
| CNN           | 0.610    | 0.617     | 0.610    | 0.598    | 0.642    |

- ViT가 AUC(0.72)에서 가장 높은 값을 기록
- 전체적으로 정밀도/재현율/정확도는 유사  
- 모델별 혼동행렬, ROC 곡선 등 추가 시각화 가능

---

## 📝 주요 파일 구성

- `pre_dectaction_dementia_.ipynb` : 전체 파이프라인 Colab 노트북 (음성→Mel→분류→분석)
- `README.md` : Github 프로젝트 안내 및 설명

---

## 📈 참고문헌 (APA)

- Breiman, L. (2001). Random forests. *Machine Learning*, 45(1), 5-32.
- Dosovitskiy, A., Beyer, L., Kolesnikov, A., et al. (2021). An image is worth 16x16 words: Transformers for image recognition at scale. *International Conference on Learning Representations*.
- Saito, T., & Rehmsmeier, M. (2015). The precision-recall plot is more informative than the ROC plot when evaluating binary classifiers on imbalanced datasets. *PLoS One, 10*(3), e0118432.

---

## 👨‍🔬 Contact

- 연구 및 협업 문의: [이메일 또는 Github 아이디]

---

## ❗️ 참고사항

- 본 코드는 공개 음성 데이터셋에 한해 연구 및 교육용으로 제공되며,  
  상업적/임상적 진단 목적 사용 시 데이터 및 법적 책임은 사용자에게 있음  
- 한국어 데이터셋 추가 연구 및 적용을 환영합니다.
