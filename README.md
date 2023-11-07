# pytorch-hangul-recognition

# 환경설정

1. python -m venv venv #가상환경생성
2. cd ./venv/Scripts/activate.bat # 가상환경 활성화
3. pip install -r requirements.txt # txt설정 정보 읽어와서 필요 툴 다운로드

cuda버전 확인및 gpu 세팅
1. nvidia-smi 실행후 버전 확인: cuda 버전확인
2. pytorch홈페이지(https://pytorch.org/get-started/locally/)에서 해당버전 install 코드 확인: 설치 전 설치파일 삭제
3. 설치 완료 후 python 환경에서 import torch.cuda
4. torch.cuda.is_available()실행 후 가능여부 확인- True

한글 데이터 생성
1. python tools/hangul-image-generator.py --label-file labels/256-common-hangul.txt
2. image-data 디렉터리에 hangul-images, labels-map.csv 생성된 결과 확인



