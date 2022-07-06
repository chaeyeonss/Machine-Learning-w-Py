# Machine Learning w/ Python

### **ndarray**
- arrange(): 주어진 범위 내에서 배열 자동 생성
- zeros(*shape, dtype=float, order='C', \*, like=None*): 입력한 크기(shape)를 가진 모든 원소가 0인 배열 생성 
- ones(*shape, dtype=float, order='C', \*, like=None*): 입력한 크기(shape)를 가진 모든 원소가 1인 배열 생성 

### Pandas Index 개요
- R-DBMS의 Primary Key와 유사하게 DataFrame, Series의 레코드를 고유하게 식별하는 객
<br>(별도의 컬럼 값은 아님 → 연산에서 제외됨) **오직 식별용으로만 사용**
- 추출 방법<br>DataFrame.index or Series.index
- reset_index()<br>새로운 인덱스를 할당하고 기존 인덱스는 새로운 컬럼으로 추가

***

###### 2장 사이킷런
### 붓꽃 데이터
- **붓꽃 데이터 피처**
  * Sepal length, Sepal width, Petal length, Petal width

> **피처(Feature) vs 속성**
> - 피처: 데이터 세트의 일반 속성
> - (@머신러닝) 타겟값을 제외한 나머지 속성을 '피처'로 지칭

<br>

- **붓꽃 데이터 품종(레이블)**
  * Setosa, Vesicolor, Virginica
> **레이블, 클래스, 타겟(값), 결정(값)**
> - 지도학습 시 데이터의 학습을 위해 주어지는 정답 데이터
> - 지도학습 중 분류의 경우, 이 결정갑을 '레이블', 또는 '클래스'로 지칭

<br>

- **데이터 분류 예측 프로세스**
  1. 데이터 세트를 학습 데이터와 테스트 데이터로 분리합니다.
  2. [모델 학습] 학습 데이터를 기반으로 ML 알고리즘을 적용해 모델을 학습시킵니다.
  3. [예측 수행] 학습된 ML 모델을 이용해 테스트 데이터의 분류(여기서는 붓꽃 종류)를 예측합니다.
  4. [평가] 예측된 결과값과 테스트 데이터의 실제 결과값을 비교해 ML 모델의 성능을 평가합니다.

***

참고: inflearn [개정판] 파이썬 머신러닝 완벽 가이드 (권철민)
