# 1 통계학과 연구설계 입문

현대통계학의 두 가지 기본 갈래는 다음과 같다.

1. **descriptive statistic**(기술 통계)

descriptive statistic은 많은 data를 하나 또는 소수의 수치로 기술한다. 

예를 들어 '백상아리의 평균 길이는 4.6미터이다.'라고 나타낸 자료가 이 descriptive statistic에 해당한다.

2. **inferential statistic**(추론 통계)

inferential statistic은 sample data를 사용하여 보다 큰 **population**(전집)을 추정한다. 

예를 들어 백상아리의 길이를 조사한 연구자들은, 모든 백상아리 집합(population)을 조사하지 않고도, 백상아리 길이를 inference(추론)하였다.

- **sample**(표본)

sample은 관심 대상인 population에서 추출한 일련의 data set이다. 연구자들은 sample을 연구하지만 실제로는 population에 관심을 가진 것이다.

다시 말해, sample은 population을 대표하려는 의도를 갖는다.

---

## 1.1 variable(변인)

**variable**(변인)이란 상이한 값을 가질 수 있는 물리, 태도, 행동 특성(**attribute**) 등의 logical set을 뜻한다. 

variable이 취할 수 있는 discrete한 값이나 조건을 **level**(수준)이라고 한다.

variable은 discrete observation, continuous observation 관찰치 중 어느 것으로도 수량화할 수 있다.

**discrete** observation(불연속 관찰)은 오직 discrete한 값만 취할 수 있다.(예를 들어 정수) 예컨대 요일마다 담배를 핀 횟수를 측정했다면 가능한 값은 오직 정수다. 담배를 1.6회처럼 필 수는 없다.

- **nominal variable**(명목변인): no numerical value, 즉 수와 관련되지 않은 variable을 뜻한다.(예를 들어 성별) 

>주의할 점은 숫자로 남녀를 1,2로 encode할 수 있지만, 이 숫자는 어떤 의미도 함축하지 않는다.

- **ordinal variable**(서열변인): 순위와 관련된 variable.(예를 들어 1등, 2등, 3등)

**continuous** observation(연속 관찰)은 continuous한 모든 값을 취할 수 있다. 예를 들어 시간이나 길이는 discrete하지 않다.(연구자가 설정한 소숫점 제한은 있을 수 있다.)

- **interval variable**(등간변인): continuous한 수치이며, 값 간의 거리(차이)가 모두 동일하다고 가정한다.(예를 들어 1도, 2도와의 간격, 5도와 6도와의 간격은 동일하다.)

> 정확히 말하면 interval variable은 요일과 같이 discrete한 variable이 있고, 온도와 같이 continuous한 variable이 있다.

- **ratio variable**(비율변인): interval variable을 만족하면서, 동시에 의미 있는 origin(영점)을 가진 variable을 의미한다.(예를 들어, 사람이 정보를 파악하는 데 걸리는 시간에서 0초는 의미 있는 영점이 된다.)

> interval variable, ratio variable은 모두 **scale variable**(척도변인)이라고 부르기도 한다.

---

### 1.1.1 independent, dependent, confounding variable

modeling에서 고려하는 세 가지 타입의 variable로 다음이 있다.

1. **independent variable**(독립변인)

dependent에 끼치는 영향을 결정하기 위해 연구자가 설계하는 적어도 두 개 수준의 level을 갖는 variable을 뜻한다.

예를 들어, 성별이 정치 성향에 어떤 영향을 미치는지를 연구할 때, independent variable은 성별이다. 

2. **dependent variable**(종속변인)

independent variable의 변화에 의해 바뀌거나, 바뀔 것이라 가정하는 variable이다.

3. **confounding variable**(혼입변인)

independent variable이 변할 때 마찬가지로 특정 체계에 따라 변하면서, 어느 variable이 independent variable인지 결정하기 어렵게 만드는 variable을 뜻한다.

예를 들어, 체중 감량을 위해 약물과 운동을 병행하고 있다고 하자. 실험자가 약물이 체중 감량을 이끌어 간다고 가정하면, independent variable은 약물 사용 여부가 되며, 운동은 confounding variable이 된다.

---

## 1.2 reliability(신뢰도)와 validity(타당도)

두 기준은 측정의 가치를 평가할 때 사용한다.

**reliability**는 측정한 data의 <U>일관성, 즉 재현의 가능 여부</U>(replicable)에 따라 평가한다. **validity**는 측정한 data가 <U>실험자의 의도와 제대로 연관이 있는가</U> 여부에 따라 평가된다.

가령 집에 있는 체중계로 얻은 몸무게가 한 시간 뒤 다시 잰 몸무게랑 크게 다르다면, 이 측정치는 reliability가 떨어지는 것이다.

반면 몸무게를 측정하기 위해 줄자를 사용했다고 치자. 얻은 측정치는 일관성을 갖기 때문에 reliability는 높겠지만, valid(타당)하지는 않다. 즉 validity는 떨어진다.

> reliability가 떨어지면, 에초에 valid(타당)할 수도 없다. 즉, validity가 높기 위한 필요조건처럼 보기도 한다.

> 예를 들어 로르샤흐 잉크반점 검사는 reliability가 떨어지는 검사이며, 따라서 validity를 해석하기도 어렵다.

---

## 1.3 hypothesis testing(가설 검증) 방법

hypothesis testing이란 증거가 variable들이 맺는 특정한 관계를 support하는지 여부를 도출하는 과정이다. 

이를 수행하기 위해서 **operational definition**(조작적 정의), variable에 처치를 가하거나, 그 variable을 측정하는 데 사용하는 절차를 규정한다.  이를 정하고 나면 hypothesis testing은 여러 방법으로 접근할 수 있다.

예컨대 가설을 검증하기 위해 여러 variable 간의 관계성을 연구할 수 있다. 이를 **correlation**(상관) 연구라고 한다.

> 그러나 일반적으로 correlation은 명확한 결과 해석이 어렵다. 따라서 실험연구를 더 선호한다.

**experiment**(실험)은 참가자를 하나 이상의 independent variable의 각 조건이나 level에 random으로 assign하는 연구이다.

실험연구를 위해서는 **random assignment**(무선 할당)을 수행해야 한다. random assignment는 모든 참가자가 <U>어떤 집단 또는 실험 조건에 assign될 기회를 동등하게 갖는다.</U>

이런 random assignment가 근사하게나마 다양한 level이나 조건을 대등하게 만들면서, 여러 잠재적 confounding variable을 제거할 수 있게 해준다.

> 하지만 random assignment가 비현실적이거나 어렵기 때문에 실험을 수행할 수 없는 경우가 흔히 있다. 이럴 때 주로 correlation 연구를 수행한다.

---

### 1.3.1 집단간 설계와 집단내 설계

실험에서는 비교집단을 여러 방식으로 만들 수 있다. 하지만 대체로 집단간 설계 또는 집단내 설계(반복측정설계) 중 하나를 사용한다.

1. 집단간 연구설계(between-groups research design)

어느 집단의 참가자가 오직 independent variable의 한 가지 level만을 경험하는 실험이다.

예를 들어 유년기 피아노가 뇌 발달에 영향을 주는지 여부를 실험한다면 다음과 같이 통제집단과 실험집단(control group and experimental group)을 설계할 수 있다.

- 통제집단(control group): 유년기 피아노 경험이 없는 level에 random assignment된 group

- 실험집단(experimental group): 유년기 피아노 경험이 있는 level에 random assignment된 group

2. 집단내 연구설계(within-groups research design)

모든 참가자가 independent variable의 모든 level을 경험하는 실험이다.

예를 들어 비디오 게임이 사람에게 미치는 영향을 비교하는 실험이 있다면, 비디오 게임을 플레이하기 전에 해당하는 level과, 플레이한 후에 해당하는 level을 동일한 참가자 집단에서 비교하게 된다.

> within이라는 표현이 한 level을 경험하더라도, 다른 모든 level을 경험할 때까지 연구를 진행한다는 의미를 담고 있다.

---