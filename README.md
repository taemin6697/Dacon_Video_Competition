# DACON 손동작 제어 인식 AI 경진대회 PUBLIC 4등

## 팀원
### 한성대학교_김태민, 3o3

## 사용 모델 및 GPU
### Timesformer(https://arxiv.org/abs/2102.05095)
(https://huggingface.co/facebook/timesformer-base-finetuned-k400)

RTX4090

### python=3.7 Windows anaconda
## 주요 설치 라이브러리(주의! jupyter notebook으로 실행 시 ipykernel과 jupyter notebook에 가상환경 등록 후 사용하시길 바랍니다!)
주피터 노트북으로 실행시 링크 = (https://python-an.tistory.com/5) + pip install jupyter
```
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113
pip install pandas
pip install opencv-python
pip install tqdm
pip install scikit-learn
pip install transformers
pip install evaluate
```

## DACON 손동작 제어 인식 AI 경진대회 코드 사용법
### 위 라이브러리 설치 후 ipynb를 열어서 그대로 실행시키면 됩니다.
```
-훈련 데이터 경로./train
-테스트 데이터 경로./test
-Submission 경로 ./sample_submission.csv
```
```
처음부터 훈련 시 그대로 따라가시면 됩니다.
가중치 파일로부터 추론 시 ipynb의 안에 있는 추론 코드를 바꾸면 됩니다.
```

## 파일 구조
```bash
├── git
│   ├── Timesformer.ipynb
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
│   ├── times (가중치파일) (https://drive.google.com/drive/folders/1lByJZrsdGp2rn8zmvQmt7SJoat3w9HgE?usp=share_link)
│   ├── train (데이터)
│   └── test (데이터)

``` 
