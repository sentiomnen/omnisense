@def title = "Critique of Pure Reason"

# {{fill title}}
Science archived an enormously successful.



Science needs the universality and regularity( tendency or necessaraily ).\\



There is two way to get new knowledge.\\
First one is the deductive reasoning that produce new knowledges from existings.\\
If reliable the how produce and existings, then the produceds are necessarily reliable.\\
Second one is the inductive reasoning that produce new knowledges from data.\\
If reliable the data and how produce, then the produceds are also necessarily reliable.\\
There is two way, But we only can use inductive reasoning for produce scientific knowledges.\\
Although the science predicts phenomena with deduction.\\
For the reliable science, we must asure the reliable of how the produce knowledges and proconditions.

\link{/science/logic/propositional/}{## Propositional Logic
Propositional logic is the studies of the how we produce new knowledges.}

\link{/science/logic/predicate/}{## Prodicated Logic
Prodicated logic is the studies of the what we said about and what we said.}



연구 대상에 변화가 발생하면 주위 환경과의 상호작용에도 변화가 발생한다.
연구 대상이 주위 환경과 상호작용하면 새로운 현상이 발생하는데, 이를 감각기관을 통해 인식하게 된다.
이를 통해 새로운 현상을 통해 연구 대상에 대한 정보를 얻을 수 있다.
즉, 주위 환경을 조성하면 연구 대상에 대한 정보를 얻을 수 있다. → 실험 experiments
가능한 모든 실험값 = experimental space, sample space.
event C :	∃C ⊂ S, outcome ∈ C.

확률은 지식이나 판단의 정도를 나타낸다.
정보는 확률(trust value)을 의미한다, 즉 정보가 많으면 확률이 높다.
사전 확률 prior probability :	실험 관측 전에 사건의 발생에 대해 이미 알고있는 확률 (믿음, 주관적 확률)
사후 확률 posterior probability :	실험 관측 후에 기대되는 확률

확률 실험 random experiment :	실험공간이 존재하고 동일한 조건하에 반복할 수 있는 실험

확률 실험을 N회 반복할 경우, 사건 C가 실제로 일어난 횟수 f
→ f / N을 N번 시행에서의 사건 C의 상대도수(relative frequency)
상대도수는 작은 N값에 대해서는 불안정하나 N의 값이 증가함에 따라 안정된다. => 근사적으로 동일한 p를 대응,
p는 실현값이 사건 C에 속하는 확률(probabilit) 혹은 C의 확률 측도(probability measure)라고 한다.

정보 이론의 핵심 아이디어 :
잘 일어나지 않는 사건(unlikely event)은 자주 발생하는 사건보다 정보량이 많다 (informative).
단위 정보 = 경우의 수의 크기. 표준 단위량으로 간주될 수 있다.
경우의 수가 2라면 밑이 2인 로그로 기술될 수 있으며, 이는 단위정보량이라 하고 이 정보량의 단위를 'bit'라고 한다.

확률변수 X의 값이 x인 사건의 정보량은 다음과 같다 :	I(x) = -log P(X).
밑이 2인 경우 정보량의 단위를 bit 혹은 shannon이라고 한다.
자연상수를 밑으로 할 경우 nat라고 한다.

Shannon entropy는 모든 사건 정보량의 기대값을 의미한다.
전체 사건의 확률붙포의 불확실한 정도를 나타낸다.
확률분포 P에 대한 섀넌 엔트로피 H(P) = H(x) = EX~P [ I(x) ] = EX~P- [ — log P(x) ].

정보이론은 주로 정보를 운반하고 있는 기호의 확률적 성질에 착안한 것이다.
k종류의 부호를 n개 늘어놓아 이뤄지는 계열의 하나가 가지는 정보량은 배합의 수 k^n종의 대수인
k = n log k에 의해 가장 합리적으로 표시된다. (엔트로피)

정보이론에서 엔트로피는 어떠한 사건event을 정의할 때,
사건이 가지는 불확실성(uncertainty)을 수치화한 것이다.
불확실성 = 정보
공리적 정의
+	양수에 한한다.
+	기하급수적이다.
+	서로 독립인 두 확률변수의 섀넌 엔트로피는 각 확률변수의 엔트로피의 합과 같다.

정보이론은 확률론과 통계학을 기반으로 하며, 여러 정보량을 통해 정보를 측정한다.
대수의 밑을 선택하는 것은 정보 엔트로피의 단위를 결정한다.
정보 엔트로피의 가장 일반적인 단위는 비트다.

정보의 측정은 메시지 m의 Self-information 혹은 "놀람의 정도 surprisal"라고 불린다.
	I(m) = log( 1/p(m) ) = - log( p(m) ).

이산 신호 공간 M의 엔트로피는 한 신호가 나타날 불확실성의 정도다.
이는 이산 신호 m의 평균 self-information으로 정의된다.
	H(M) = E[ I(M) ] (expected value) = ∑_{m ∈ M} p(m) I(m) = - ∑_{m ∈ M} p(m) log p(m).


측정 : 기호화
모든 기호는 전달 형식과 전달 내용이라는 두가지 측면을 가진다.
기호 = 정보, 의미(형식과 다른 인식)를 갖는 개체
정보 = 추정 가능함

연구대상의 관계는 곧 비례관계로, 비례, 순서 관계와 양적 관계를 포함하여, 대상적 차이와 양의 차이를 알아낼 수 있다.

자연수의 본질은 비교와 비례다.

모든 측정은 불확실성을 지닌다.
따라서 실험에 대한 상대도수의 측정도 항상 불확실성을 지닌다.

관측의 이론 적재성 Theory-ladenness of observation : 관측은 이론을 수반한다
지각의 해석은 이론에 기반한다.

관측 기구는 이론에 의해 작동한다.
이론에 맞지 않는 관측 결과는 거부될 수 있다.
측정 = 수량화된 관측 수량화에 있어 중요한 것은 기준 수량의 고정점. 일관성. 정밀성.
감각이 옳다는 가정하에(기존 이론 하에) 기구를 만듦
더 정밀한 기구를 통해 감각을 수정(이론 수정) 반복
Experiments. 조작에 따른 결과 인과관계를 입증한다. 연구자가 패턴에 대한 정보를 이끌어 낼 수 있는 방법은 실험 뿐이다.


측정 measurement.
정확도 accuracy :	측정값과 참값의 차이
정밀도 precision :	측정값의 재현성, 유효숫자의 개수와 비례함.

오차 error :	측정값과 참값의 차이, E = M - T
보정값 = T - M
+	과실적 오차 gross error :	측정 과정의 실수에 의한 오차, 반복 측정으로 교정한다.
+	계통적 오차 systematic error :	측정기, 환경에 의한 오차, 개선과 교정을 통해 교정
+	우발적 오차 random error :	교정 불가, 반복측정의 평균을 얻음

측정 도구 =	연구 대상을 정량화하는 도구, 척도(scale) 등
정의에 측정을 포함하는 것 = 조작적 정의 (operational definition).

척도에 유의점 :
+	모든  예상되는 응답이 값에 반영되어야 한다.
+	각 값들 사이에는 중복되는 속성이 없어야 한다.








정밀한 정량적 관측 (측정 measurment)을 통한 수학 공식의 형태로 표현된다.

측정값과 이론의 수치 예측 (numerical predictions)의 비교를 통해
신뢰도를 얻거나 수정할 수 있다.




확률변수 X의 값이 x인 사건의 정보량은 아래와 같다 :
I(x) = - log P(x).

결정 = 비교와 선택

실제 사건은 선형적이다. (집합이 아닌 tuple로 추상화된다, waterfall model)
계획은 사건의 전체적인 양상을 예측하고 제어를 시도한다.
따라서 예측을 지속적으로 평가하고, 지속적으로 계획을 수립해야 한다.

계획을 수립하고 이행하기 전에 해야할 가장 중요한 것은 전략(패턴)을 세우는 것이다.
지속적인 계획 수정과 이행에서는 완벽한 설계로 부터의 상향식 개발이 아닌,
핵심 기능을 기본으로 하여 다양한 기능을 가진 다양한 모델을 개발하여, 가장 요구에 부합하는 모델을 선택한다.
그러나 다양한 모델을 개발하기 위해서는 핵심의 유지와 고도의 추상화가 필요하며, 이를 전략이라 한다.
즉, 전략은 판단 기준, 모델이다.

계획을 수립하는데에 중요하는 것은 예측 능력이며,
모델링은 예측 모델을 수립함으로써 예측 능력을 향상시킨다.



정보의 왜곡에도 반드시 어떠한 패턴이 있을 것이다.

백분율 오차 Percentage error : eypsilon = (M-T)/T *100%
백분율 보정 alpha = (T-M)/M * 100%
 
계측기 보증 오차 : 계측기의 정확도 (CLASS), 계기의 풀 스케일 값의 백분율 오차
CLASS 5 =  풀 스케일에서 최대 5% 오차
 
 
유효숫자 : 측정값의 신뢰할 수 있는 숫자의 범주
예> 100옴의 참값은 99~101, 100.0옴의 참값은 99.9~100.1
 
유효숫자가 서로 다른 측정값의 경우 작은 유효숫자로 제한하여 수용한다.
