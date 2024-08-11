# OCR Image Processing Tool

이 프로젝트는 이미지 폴더 내의 이미지에 대해 OCR(Optical Character Recognition)을 수행하고, 결과를 CSV, JSON 또는 TXT 파일로 저장하는 도구입니다. 이 도구는 PaddleOCR을 사용하여 한국어 텍스트를 인식합니다.


## 설치
      
1. **필수 패키지 설치**
```
pip install numpy paddleocr paddlepaddle paddlepaddle-gpu pandas Pillow argparse
```

## 사용법
```
python run.py --image_folder <이미지 폴더 경로> --output_folder <결과 저장 폴더 경로> --savefile_type <저장 파일 형식> [--draw_ocr]
```

- --image_folder: 이미지 파일들이 있는 폴더의 경로입니다. (필수)
- --output_folder: OCR 결과를 저장할 폴더의 경로입니다. 기본값은 './output'
- --savefile_type: 결과 파일 저장 형식입니다. csv, txt, json 중 하나를 선택할 수 있습니다. 기본값은 csv입니다.
- --draw_ocr: 이 플래그를 지정하면, OCR 결과를 이미지에 그려서 저장합니다. (선택)

