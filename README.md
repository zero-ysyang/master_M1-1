# 삼성전자 주가 시계열 분석

2023~2024년 삼성전자(005930.KS) 주가의 추세·변동성·
계절성을 분석한 프로젝트입니다.

## 📁 프로젝트 구조

```
project
├── README.md # 실행 방법 (이 파일)
├── REPORT.md # 분석 리포트
├── analysis.ipynb # 분석 노트북
├── requirements.txt # 의존성 목록
├── data/ # 데이터
|     └── samsung_2023_2024.csv
└── images/ # 시각화 결과
      ├── ma_trend.png
      ├── daily_return.png
      └── monthly_pattern.png
```


## ⚙️ 설치 방법
```bash
# 1. 라이브러리 설치
pip install -r requirements.txt
```

```
# Jupyter 노트북 실행
jupyter notebook analysis.ipynb
```
그 후 위에서 아래로 셀을 순서대로 실행하세요.

```
실행 순서
라이브러리 import
데이터 수집 (yfinance)
데이터 전처리 (결측치·수익률 계산)
분석 1: 추세 (이동평균)
분석 2: 급등락 (일간 수익률)
분석 3: 월별 패턴
시각화 저장
```

📊 데이터 출처
```
출처: Yahoo Finance (yfinance 라이브러리)
종목: 삼성전자 (005930.KS)
기간: 2023-01-01 ~ 2024-12-31
수집 방법: yf.download("005930.KS", start=..., end=...)
```

⚠️ 라이선스 및 주의사항
```
본 데이터는 Yahoo Finance에서 제공하며, 개인 학습·연구 목적으로만 사용합니다.
yfinance는 비공식 라이브러리로, 상업적 사용 시 Yahoo의 이용약관을 확인해야 합니다.
본 분석은 투자 조언이 아니며, 투자 판단의 책임은 본인에게 있습니다.
```
