# Intro AI

상명대학교 인공지능개론 수업 실습·과제 모음. 주제별로 폴더를 나눠 정리한다.

## 목차

| 폴더 | 주제 | 내용 |
|---|---|---|
| [`knn-matlab/`](knn-matlab) | KNN | MATLAB으로 KNN을 단계별로 구현·비교한 실습 5개 |
| [`naive-bayes/`](naive-bayes) | 가우시안 나이브 베이즈 | 꽃받침 길이 하나로 Setosa / Versicolor 판별 |
| [`data/`](data) | — | 실습용 데이터셋 |

## knn-matlab

| 파일 | 내용 |
|---|---|
| `ex1_dataload_visualization.m` | 데이터 적재와 시각화 |
| `ex2_knn_using_matlab.m` | MATLAB 내장 함수로 KNN |
| `ex3_knn_my_style.m` | KNN 직접 구현 |
| `ex4_knn_generalization.m` | 일반화 성능 확인 |
| `ex5_knn_space.m` | 결정 공간 시각화 |

## naive-bayes

`iris_nb.ipynb` — 꽃받침 길이(sepal.length) 하나만 보고 길이 7.2cm인 붓꽃의 품종을 판별한다.

품종별 평균·표준편차로 정규분포를 그리고(확률분포를 구한다 = 평균과 표준편차를 구한다), 두 곡선이 만나는 결정경계를 계산한 뒤, 우도 → 사후확률 → 판정 순서로 분류한다. 사전확률을 바꾸면 경계가 어떻게 움직이는지도 확인한다.

실행 결과와 그래프가 노트북에 저장돼 있어 따로 돌리지 않아도 볼 수 있다.

## data

| 파일 | 내용 |
|---|---|
| `iris.csv` | Iris 데이터셋 150행 (sepal/petal length·width, variety) |

## 실행

MATLAB 실습은 MATLAB에서 각 `.m` 파일을 연다.

노트북은 저장소 루트를 기준으로 실행한다.

```bash
pip install numpy pandas matplotlib jupyter
jupyter notebook naive-bayes/iris_nb.ipynb
```
