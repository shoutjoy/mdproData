# 4장_공간디스플레이_research
# STEP 1: 지식의 지도 그리기 (Preview)
본 챕터(제4장 공간 디스플레이)는 인간이 공간적 정보를 지각하고 처리하는 과정과 이를 지원하는 디스플레이 인터페이스 설계의 원리를 다룬다. 본문의 전체 내용을 논리적 흐름에 따라 핵심 요약 및 도식화하고, 반드시 기억해야 할 주요 전문 용어를 학술적 인용 정보와 함께 정리하였다.


![image](https://i.ibb.co/tTP6S8C6/image.png)
<span class="fig-caption">[그림 1] 그래프의 설계 원칙 </span>


### 1. 단원 핵심 요약 및 논리적 흐름 (Logical Flow)

**섹션 1: 그래프 지각 (Graph Perception)**
그래프는 데이터를 시각적인 공간 배열로 표상하여 인간이 신속한 공간적 판단을 내리게 돕는다. 효과적인 그래프 설계를 위해서는 시각적 탐색과 정보 통합에 필요한 정신적 연산을 최소화해야 한다. 이를 위해 과제의 성격과 디스플레이 배열을 일치시키는 근접성 호환성 원리(PCP)[^1]가 적용되며, 불필요한 시각적 잉크를 제거하는 데이터-잉크 비율 원칙[^2]을 준수해야 한다. 다중 그래프에서는 변수 매핑과 형태의 일관성을 유지하여 시각적 운동성(visual momentum)을 확보하는 것이 핵심이다.

**섹션 2: 다이얼, 미터 및 지시기: 디스플레이 호환성 (Display Compatibility)**
동적 통제 시스템에서 디스플레이는 물리적 시스템과 운영자의 멘탈 모델 사이를 매개한다. 아날로그 시스템 표상 시에는 변수 형태와 방향의 직관성을 보장하는 그림 사실주의 원리(PPR)[^3]와, 제어 조작에 따른 표시기의 움직임 방향을 멘탈 모델과 일치시키는 이동 부품의 원리(PMP)[^4]가 요구된다. 때로는 두 원리가 충돌하므로 주파수 분리(frequency-separated)와 같은 하이브리드 설계가 도입된다. 또한, 시스템의 목적과 물리적 제약 등 작업 도메인을 깊이 분석하여 시각적 창발 자질(emergent feature)로 형상화하는 생태학적 인터페이스 설계(EID)[^5]는 작업의 효율성을 극대화한다.

**섹션 3: 3차원: 자아 운동, 깊이 그리고 거리 (The Third Dimension)**
인간의 3차원 공간 지각은 무의식적으로 환경을 탐색하는 직접 지각 체계(자아 운동 등)와 의식적 추론이 수반되는 간접 지각 체계로 이중화되어 있다[^6]. 직접 지각은 시야 주변부에서 발생하며, 광학적 흐름이나 전개성 등 불변하는 환경 단서(광학 불변량)[^7]를 통해 진행 방향과 속도를 조절하게 한다. 간접 지각에서는 대상의 크기, 교차(occlusion) 등 대상 중심 단서와 생리적 요인 등 관찰자 중심 단서가 활용되며, 뇌는 이를 가중 선형 단서 모델(WLCM)[^8]에 따라 확률적으로 통합하여 깊이와 거리를 추론한다. 

**섹션 4: 공간 청각 및 촉각 디스플레이 (Spatial Audio and Tactile Displays)**
공간 정보는 시각에만 국한되지 않는다. 3D 공간 음향과 촉각 디스플레이는 시각 채널에 과부하가 걸렸을 때 정위 반사(orientation reflex)를 이용하여 공간적 주의력을 빠르고 직관적으로 환기시키는 보완적 역할을 수행한다.

---

### 2. 반드시 기억해야 할 가장 중요한 전문 용어 (Key Technical Terms)

| 전문 용어 (학술 개념) | 관련 학자 및 연도 | 주요 내용 및 학술적 의의 | 출처(Source) 참조 |
| :--- | :--- | :--- | :--- |
| **근접성 호환성 원리 (PCP)** | Wickens & Carswell (1995) | 다중 정보 출처의 배열과 통합 과제 요구 간의 호환성을 정의. 통합 과제에는 통합된 객체 디스플레이가 적합함. | Source, |
| **데이터-잉크 비율 (Data-Ink Ratio)** | Tufte (2001) | 디스플레이에 사용된 전체 잉크 중 불필요한 비데이터 잉크를 배제하고 실제 데이터 묘사에 사용된 비율을 극대화해야 함. | Source, |
| **그림 사실주의 원리 (PPR)** | Roscoe (1968) | 변수가 본질적으로 아날로그라면 디스플레이 역시 방향, 형태를 물리적 멘탈 모델과 일치하는 아날로그로 표상해야 함. | Source,, |
| **이동 부품의 원리 (PMP)** | Roscoe (1968); Roscoe, Corl, & Jensen (1981) | 디스플레이 상의 지시기 이동 방향은 조작자가 변수의 움직임에 대해 가지는 멘탈 모델의 방향과 반드시 호환되어야 함. | Source, |
| **생태학적 인터페이스 설계 (EID)** | Vicente & Rasmussen (1992); Vicente (2002) | 대상 시스템의 물리적, 기능적 제약을 시각 디스플레이의 창발적 구조(기하학적 형태 등)에 반영하여 생태학적 호환성을 달성하는 설계. | Source, |
| **광학 불변량 (Optical Invariants)** | Gibson (1979) | 자아 운동을 통제하기 위해 관찰자의 시각 시스템이 자동 감지하는 환경적 특성(예: 질감 기울기, 전개성, 광학 흐름). | Source, |
| **충돌 시간 (Tau)** | Lee (1976); DeLucia (2007) | 망막에 맺히는 물체상 크기의 팽창률 역수. 관찰자가 대상과 물리적으로 접촉하기까지 남은 시간을 산출하는 시각적 변수[^9]. | Source, |
| **가중 선형 단서 모델 (WLCM)** | Bruno & Cutting (1988); Young, Landy, & Maloney (1993) | 인간의 뇌가 여러 깊이 단서를 통합할 때 단서의 신뢰성에 따라 가중치를 부여하며, 이 과정에서 교차(occlusion) 등 특정 단서가 우위를 점함. | Source, |

---

### 3. 지식 구조 도식화 (Flow Chart / Mind Map)

```mermaid
treeView-beta

[제4장 공간 디스플레이 (Spatial Displays) 지식 구조도]

(Root) 공간 디스플레이 인터페이스 최적화
 ├── 1. 정적/아날로그 정보 표상 (Graphs)
 │    ├── 정보 접근 비용 축소 (Search, Encode, Compare)
 │    ├── 디스플레이-인지 호환성: 근접성 호환성 원리 (PCP)
 │    ├── 시각적 노이즈 제거: 데이터-잉크 비율 원칙
 │    └── 지각 편향(Bias) 완화: 스티븐스 법칙 고려
 │
 ├── 2. 동적 제어/계기반 설계 (Dials, Meters, Indicators)
 │    ├── 호환성의 3계층: 물리적 시스템 ↔ 멘탈 모델 ↔ 디스플레이 표면
 │    ├── 인지적 매핑 원리: 그림 사실주의 원리 (PPR) vs 이동 부품 원리 (PMP)
 │    │    └── 해결책: 주파수 분리 하이브리드 디스플레이
 │    └── 시스템 목적의 시각화: 생태학적 인터페이스 설계 (EID)
 │
 ├── 3. 3차원 공간 지각 (The Third Dimension)
 │    ├── 직접 지각 시스템 (Egomotion 통제)
 │    │    └── 광학 불변량 인식 (Optical flow, Splay, Tau 등)
 │    ├── 간접 지각 시스템 (물체 및 깊이 인식)
 │    │    └── 가중 선형 단서 모델 (WLCM) 기반 깊이 단서 통합
 │    └── 3D 디스플레이 적용: 모호성(LOS) 및 압축 한계 돌파 방안
 │
 └── 4. 감각 확장을 통한 보완 (Spatial Audio & Tactile)
      ├── 3D 공간 음향: HRTF 기반 정위 반사 유도
      └── 공간 촉각: 시각 정보 부하(Clutter) 시 즉각적 주의 분산 방지
```

위 구조도에서 볼 수 있듯, 이 단원은 기초적인 정적 그래프의 '인지적 경제성(Data-ink, PCP)' 논의에서 출발하여 동적 기기(PPR, PMP)를 거쳐, 인간이 3차원 물리 환경과 상호작용하는 근원적 지각 모델(Direct vs Indirect perception, EID, 광학 불변량)까지 이론적 스케일을 논리적으로 확장하고 있다.




[^1]: "In Chapter 3 we introduced the notion of compatibility between the arrangement of multiple information sources on a display, and the task requirements. We saw that this display-cognitive compatibility could be defined in part by the proximity compatibility principle (PCP; Wickens & Carswell, 1995)."
[^2]: "He argued for a data-ink ratio principle, which states that the amount of ink that does not depict data points should be kept to a minimum (Tufte, 2001)."
[^3]: "The principle of pictorial realism (PPR; Roscoe, 1968) has two parts. The first part can be defined as follows: if a variable’s physical representation is analog, then its display representation should also be analog (Roscoe, 1968)."

[^4]: "Roscoe (1968) and Roscoe, Corl, and Jensen (1981) proposed the principle of the moving part (PMP)—that the direction of movement of an indicator on a display is compatible with the direction of movement of an operator’s mental model of the variable."

[^5]: "When this configuration is done in a way to reflect the constraints of the natural physical system being represented, the resulting displays are called ecological interfaces (Vicente & Rasmussen, 1992; Vicente, 2002), conforming to ecological compatibility."

[^6]: "Psychologists have reached broad consensus that there are two qualitatively different systems for perceiving 3D space (DeLucia, 2008)."

[^7]: "Gibson (1979) identified a set of environmental properties that the visual system can detect to assist in control of egomotion. These properties have sometimes been referred to as optical invariants..."

[^8]: "To understand when depth judgments succeed and fail, it is important to consider how the cues are integrated in the brain, an integration that is well explained by the weighted linear cue model (WLCM; Bruno & Cutting, 1988; Ichikawa & Saida, 1996; Knill, 2007; Young, Landy, & Maloney, 1993)."

[^9]: "4. Time-to-contact (tau). Tau specifies the time remaining until an observer makes contact with an object, assuming that the speed of the observer or the object is constant (DeLucia, 2007; Grosz, Rysdyk, et al., 1995; Lee, 1976)."


<div class="page-break"></div>


# STEP 2: 핵심 개념 딥다이바이빙 (Concept Mastery)

본 교재(제4장 공간 디스플레이)는 인간의 인지적 한계를 극복하고 복잡한 시스템과의 상호작용을 최적화하기 위해 다양한 심리학적 이론과 공학적 모델을 망라하고 있다. 교재 전체에 걸쳐 등장하는 모든 핵심 이론과 모델을 심층 분석하고, 이들의 유기적 연결 관계를 도식화한다.

### 1. 전체 핵심 이론 및 모델 딥다이브 (Concept Mastery)

**1) SEEV 모델 (시각적 정보 표집 모델)**
*   **연구자 및 연도**: 제3장 개념으로 본 장의 그래프 지각에 응용됨[^10].
*   **탄생 배경**: 수많은 시각 정보 중 인간이 어디에 주의를 기울이는지 예측하고, 비효율적인 디스플레이 설계로 인해 불필요한 인지 연산이 길어지는 것을 방지하기 위해 고안되었다.
*   **세부 요소**: 상향식(Bottom-up) 요소인 현저성(Salience)과 노력(Effort), 하향식(Top-down) 요소인 기대치(Expectancy)와 가치(Value)로 구성된다.
*   **쉬운 비유**: **'마트에서의 장보기'**와 같다. 화려한 네온사인(현저성)과 입구에서 가까운 매대(노력)는 무의식적으로 눈길을 끈다. 하지만 소비자는 자신이 평소 우유를 어디서 샀는지(기대치)와 오늘 요리에 우유가 얼마나 중요한지(가치)를 종합하여 최종 시선을 결정한다.

![image](https://i.ibb.co/Z69xdFVY/image.png)
<span class="fig-caption">[그림 2] SEEV모델의 영향</span>


**2) 그래프 지각 모델 (탐색, 부호화, 비교)**
*   **연구자 및 연도**: Casner (1991); Gillan (1995, 2009); Peebles & Cheng (2003) 등[^11].
*   **탄생 배경**: 사용자가 그래프를 읽을 때 비효율적인 스캐닝이나 정보 망각을 겪는 이유를 인지적 단계로 쪼개어 분석하기 위해 탄생했다.
*   **세부 요소**: 시각적 탐색(Search), 변수 부호화(Encoding), 작업 기억 내 비교(Comparison)라는 순차적 정신적 연산(Mental operations)으로 이루어진다.
*   **쉬운 비유**: **'도서관에서 논문 쓰기'**와 같다. 수많은 책장 중 필요한 책을 찾고(탐색), 책의 내용을 읽어 머릿속에 넣은 뒤(부호화), 내가 원래 알고 있던 지식이나 다른 책의 내용과 대조하는(비교) 과정이다. 이 단계가 꼬이면 책을 여러 번 다시 들춰봐야 하는 비효율이 발생한다.

**3) 스티븐스의 법칙 (Stevens' Law)**
*   **연구자 및 연도**: Stevens (1957, 1975)[^12].
*   **탄생 배경**: 인간이 물리적인 연속체(부피, 면적 등)의 크기를 추정할 때, 실제 크기와 뇌에서 지각된 크기 사이에 체계적이고 수학적인 편향이 발생함을 설명하기 위해 만들어졌다. 스티븐스는 기존 페히너 법칙(Fechner's Law)이 모든 감각 차원에서 로그 함수적 관계를 가진다고 가정한 한계를 비판하며, 자극의 종류에 따라 지각의 양상이 근본적으로 다름을 **거듭제곱 함수(Power Function)**로 증명하였다.

스티븐스의 법칙은 물리적 자극의 강도와 주관적 지각 크기 사이의 관계를 다음과 같이 정의한다.
$$S = kI^n$$
$S$ (Subjective Magnitude): 피험자가 느끼는 주관적인 감각의 크기.
$I$ (Physical Intensity): 실제 물리적인 자극의 강도.
$k$ (Constant): 측정 단위에 따라 결정되는 비례 상수.
$n$ (Exponent): 자극의 특성을 결정짓는 거듭제곱 지수. 
이 지수값에 따라 감각의 왜곡 방향과 강도가 결정된다.

*   **세부 요소**: 물리적 크기와 지각된 크기의 관계를 결정하는 거듭제곱 지수로, 반응 압축(지수<1.0, 부피/면적 과소평가)과 반응 팽창(지수>1.0, 채도 과대평가)으로 나뉜다.
<span class="tbl-caption"><표1> 스티븐슨 법칙의 반응 </span>
| 분류 | 지수 조건 | 지각적 특징 | 대표적 예시 |
| --- | --- | --- | --- |
| 반응 압축 (Response Compression) | n<1.0 | 물리적 자극이 커질수록 감각의 증가 폭이 점차 둔화됨. | "밝기(0.33) /소리 크기(0.67)/ 면적/ 부피" |
| 선형 반응 (Linear Response) | n=1.0 | 물리적 자극의 변화와 지각된 크기가 정확히 일치함. | 선의 길이 (인간이 가장 정확하게 인지) |
| 반응 팽창 (Response Expansion) | n>1.0 | 물리적 자극이 조금만 증가해도 감각이 폭발적으로 증폭됨. | "전기 충격(3.5)/온도/무거운 무게" |


 **학술적 보완 및 시사점**
1 ) 진화심리학적 해석: 왜 지수가 다른가?
- 반응 팽창(위험 감지): 전기 충격이나 강한 통증은 생명과 직결된다. 따라서 뇌는 미세한 자극 변화에도 민감하게 반응하여 신속한 회피 행동을 유도하도록 설계되었다.
- 반응 압축(범위 적응): 빛의 밝기나 소리의 크기는 자연계에서 변화의 폭이 매우 크다. 만약 이를 선형적으로 지각한다면 우리의 감각 수용기는 금방 포화 상태(Saturation)에 이를 것이다. 뇌는 이를 압축함으로써 넓은 범위의 정보를 효율적으로 수용한다.


2) 데이터 시각화 및 설계에서의 응용
- 면적의 오류: 지도에서 원의 크기로 데이터를 표현할 때, 사용자는 실제 면적보다 작게 인지하는 경향(반응 압축)이 있다. 따라서 숙련된 설계자는 스티븐스의 지수를 역산하여 원의 크기를 실제 데이터보다 조금 더 크게 키워 그려주는 방식을 취하기도 한다(Flannery's Compensation).
- 길이의 신뢰성: $n=1$에 가까운 '막대그래프'나 '직선'이 원형 그래프나 3D 입체 그래프보다 정보 전달의 정확도가 압도적으로 높은 이유를 이 법칙이 설명해준다.

*   **쉬운 비유**: **'놀이공원의 요술 거울'**과 같다. 채도 같은 자극은 한 걸음 다가가면 거울 속 모습이 훌쩍 커 보이지만(반응 팽창), 부피 같은 자극은 세 걸음을 다가가도 겨우 한 걸음 커진 것처럼 답답하게 느껴진다(반응 압축).
    
** 스티븐스의 법칙(Stevens' Power Law)을 시각적으로 가장 잘 나타내는 그래프**

![스티븐슨](https://www.appstate.edu/~steelekm/classes/psy3215/Measure/StevensFig1.gif) 

위 그래프는 물리적 자극의 강도(Horizontal Axis)와 주관적인 지각 강도(Vertical Axis) 사이의 관계를 지수($n$)에 따라 명확하게 보여준다.


  - Stevens, S. S. (1957). On the psychophysical law. Psychological Review, 64(3), 153–181.
  - Stevens, S. S. (1975). Psychophysics: Introduction to its perceptual, neural, and social prospects. Wiley.
  - Cleveland, W. S., & McGill, R. (1984). Graphical Perception. Journal of the American Statistical Association (스티븐스 법칙의 시각화 적용 사례).
    



**4) 데이터-잉크 비율 원칙 (Data-Ink Ratio Principle)**
*   **연구자 및 연도**: Tufte (2001)[^13].
*   **탄생 배경**: 정보 그래픽에 불필요한 시각적 장식이 많아지면 시각적 혼란(Clutter)이 발생하여 데이터 판독 시간이 지연되는 문제를 해결하기 위함이다. 에드워드 터프티(Edward Tufte)가 제안한 이 원칙은 UI 디자인에서 **'시각적 노이즈 제거를 통한 인지 부하(Cognitive Load)의 최소화'**로 직결된다. UI 구성 요소 중 실제 정보를 전달하지 않는 장식적 요소를 제거함으로써 사용자의 작업 효율성을 높이는 것이 핵심이다.
*   **세부 요소**: 그래프에 사용된 전체 잉크 중에서, 실제 데이터를 나타내는 데 쓰인 '데이터 잉크'의 비율을 극대화하고 장식용 '비데이터 잉크'는 최소화해야 한다.
*   **쉬운 비유**: **'과일 주스 원액과 물'**의 관계다. 정보라는 과즙(데이터 잉크)에 불필요한 물(비데이터 잉크, 예: 3D 장식)을 너무 많이 섞으면 맛이 흐려져 무슨 주스인지 단번에 알아맞히기 힘들어진다.


<span class="tbl-caption"><표 2> 데이터 잉크 비율법칙</span>
| 구분 | 낮은 데이터-잉크 (장식 과잉) | 높은 데이터-잉크(최적화) |
| --- | --- | --- |
| 차트/그래프 | "3D 막대 그래프/ 그림자 효과/ 배경 그리드" | "2D 평면 그래프/ 그리드 제거 또는 점선 처리" |
| 버튼(Button) | "과도한 입체감(Bevel)/ 복잡한 아이콘과 텍스트 병행" | 고스트 버튼(Ghost Button) 또는 플랫 디자인 |
| 내비게이션 | "화려한 질감의 메뉴 바/ 구분선 남발" | "여백을 활용한 그룹화/ 타이포그래피 중심 설계" |

**핵심결론 **
Tufte는 "설계의 핵심은 데이터-잉크 비율을 1.0에 가깝게 만드는 것"이라고 주장하였다(Tufte, 2001). 이는 디자인이 단순히 심미적인 영역에 머무는 것이 아니라, 정보 전달의 정확성을 담보하는 공학적 접근임을 시사한다. UI 디자인에서 비데이터 잉크(Non-data-ink)를 제거하는 행위는 사용자가 정보를 처리할 때 소비하는 **작업 기억(Working Memory)**의 낭비를 막아준다. 즉, 불필요한 장식을 걷어낼수록 사용자는 인터페이스 자체가 아닌 '콘텐츠' 그 자체에 온전히 집중할 수 있게 된다.


**5) 근접성 호환성 원리 (PCP; Proximity Compatibility Principle)**
*   **연구자 및 연도**: Wickens & Carswell (1995)[^14].
*   **탄생 배경**: 화면상의 정보 출처 배열 방식과 사용자가 수행해야 할 과제의 인지적 요구 사항 사이의 불일치를 막고 통합 처리 효율을 높이기 위해 정립되었다.
*   **세부 요소**: 과제 근접성(여러 정보를 통합해야 하는지 vs 개별 점만 읽는지)과 디스플레이 근접성(정보가 선이나 도형처럼 하나의 객체로 묶였는지 vs 분리되었는지)의 일치를 요구한다.
*   **쉬운 비유**: **'요리 과제에 따른 식기 선택'**이다. 여러 재료를 섞어야 하는 비빔밥(통합 과제)은 넓은 하나의 양푼(통합된 객체 디스플레이)이 호환성이 높고, 개별 반찬의 맛을 따로 봐야 하는 뷔페(초점 과제)는 칸이 나뉜 식판(분리된 디스플레이)이 호환된다.

**6) 멘탈 모델 이론 (Mental Models Theory)**
*   **연구자 및 연도**: Gentner & Stevens (1983); Moray (1998) 등[^15].
*   **탄생 배경**: 시스템 사용자가 눈에 보이지 않는 복잡한 내부 동작 원리를 어떻게 추론하고 시스템을 통제하는지 설명하기 위한 인지 구조 이론이다.
*   **세부 요소**: 물리적 시스템(기계 자체), 디스플레이 표면, 그리고 조작자의 뇌 속에 형성된 예측과 이해의 기반인 내부 표상(멘탈 모델)으로 구성된다.
*   **쉬운 비유**: **'스마트폰 백그라운드 앱 상상하기'**와 같다. 스마트폰 내부의 반도체 회로(물리적 시스템)를 직접 볼 수는 없지만, 아이콘(디스플레이)을 쓸어 올리면서 '아, 뒤에서 돌아가던 앱이 꺼졌구나'라고 머릿속으로 메커니즘을 그리는 과정(멘탈 모델)이다.

**7) 그림 사실주의 원리 (PPR) 및 이동 부품의 원리 (PMP)**
*   **연구자 및 연도**: Roscoe (1968); Roscoe, Corl, & Jensen (1981)[^16][^17].
*   **탄생 배경**: 동적 계기판(고도계, 자세지시계)이 인간의 직관(멘탈 모델)과 반대로 설계되어 발생하는 치명적 비행 및 제어 사고를 예방하기 위해 제안되었다.
*   **세부 요소**: PPR은 물리적 변수가 아날로그라면 디스플레이도 형태와 방향(높은 곳은 위로)을 아날로그로 일치시켜야 한다는 원리다. PMP는 조작자가 상상하는 지시기 이동 방향과 실제 화면상 이동 방향이 같아야 한다는 원리다.
*   **쉬운 비유**: **'자동차 핸들과 창밖 풍경'**이다. 핸들을 왼쪽으로 돌리면 바퀴 기호도 왼쪽으로 돌아가야 직관적이다(PMP). 동시에 차가 언덕을 오르면 화면 속 고도선도 땅으로 꺼지는 대신 하늘로 올라가야 한다(PPR).

**8) 순진한 사실주의 (Naïve Realism)**
*   **연구자 및 연도**: Smallman & St John (2005); Hegarty, Smallman, & Stull (2012)[^18].
*   **탄생 배경**: 무조건 사진처럼 극사실적으로 3D 렌더링을 하면 사용자의 성과가 좋아질 것이라는 대중과 설계자들의 맹신과 착각을 비판하기 위해 탄생했다.
*   **세부 요소**: 불필요한 질감, 과도한 사실적 지형 묘사 등 과제와 무관한 시각적 노이즈가 과제 관련 핵심 데이터를 가려 인지적 과부하를 유발하는 현상.
*   **쉬운 비유**: **'TMI (Too Much Information) 친구'**와 같다. "도서관 가는 길 좀 알려줘"라고 물었는데, 길의 방향(핵심 정보)뿐만 아니라 바닥의 보도블록 색깔, 길가에 핀 꽃의 종류까지 사진처럼 다 설명해서 오히려 길을 더 헷갈리게 만드는 것이다.

**9) 생태학적 인터페이스 설계 (EID; Ecological Interface Design)**
*   **연구자 및 연도**: Vicente & Rasmussen (1992); Vicente (2002)[^19].
*   **탄생 배경**: 원자력 발전소처럼 극도로 복잡한 자동화 시스템에서, 수백 개의 숫자를 암산하다가 발생하는 돌발 실패를 막기 위해 시스템의 물리적/추상적 제약을 직관적인 시각 기하학으로 치환하기 위해 도입되었다.
*   **세부 요소**: 작업 도메인의 기능적/추상적 분석, 물리적 질량 보존 법칙과 같은 한계치, 그리고 이를 단일 도형의 기울기나 형태로 묶어낸 '창발 자질(Emergent features)'로 구성된다.
*   **쉬운 비유**: **'목수 수준기(Carpenter's level)'**와 같다. 복잡한 중력 가속도와 벽의 기울기를 머리 아프게 수학으로 계산하지 않고, 물방울 기포가 선 중앙에 있는지(창발 자질)만 쓱 보고 즉각적으로 균형(시스템 상태)을 판단하는 직관적 설계다.

**10) 이중 지각 체계 (직접 지각 및 간접 지각)와 생태학적 심리학**
*   **연구자 및 연도**: Gibson (1979); DeLucia (2008) 등[^20][^21].
*   **탄생 배경**: 인간이 3차원 공간을 지각할 때 단일한 과정이 아니라 무의식적인 운동 통제 체계와 의식적인 대상 식별 체계가 질적으로 분리되어 있음을 설명하기 위함이다.
*   **세부 요소**: '직접 지각'은 배측 경로를 통해 주변시로 들어오는 광학 불변량(Optical invariants; 흐름, 전개성 등)을 무의식적으로 즉각 수용하여 자아 운동을 통제한다(생태학적 심리학). '간접 지각'은 중심시와 복측 경로를 통해 과거 경험과 하향식 추론을 동원하여 대상의 거리/깊이를 판단한다.
*   **쉬운 비유**: **'자전거 타며 동네 구경하기'**와 같다. 몸의 중심을 잡고 넘어지지 않기 위해 땅바닥과 주변이 스쳐 지나가는 흐름을 몸이 자동으로 느끼는 것은 '직접 지각'이다. 반면, 저 멀리 보이는 표지판 글씨를 찡그리며 집중해서 읽어 거리를 가늠하는 것은 '간접 지각'이다.

**11) 가중 선형 단서 모델 (WLCM; Weighted Linear Cue Model)**
*   **연구자 및 연도**: Bruno & Cutting (1988); Young, Landy, & Maloney (1993)[^22].
*   **탄생 배경**: 뇌가 2D 망막에 맺힌 상을 3D 깊이로 추론할 때, 수많은 대상 중심 및 관찰자 중심 깊이 단서들이 충돌할 경우 뇌가 어떻게 확률적으로 결론을 내리는지 수학적으로 규명하기 위해 고안되었다.
*   **세부 요소**: 선형 원근법, 입체시, 교차 등 다양한 깊이 단서들과, 각 단서가 뇌에서 차지하는 신뢰성과 경험 기반의 '가중치(Weight)'. 특히 교차(Occlusion)와 입체시가 우위를 점한다.
*   **쉬운 비유**: **'재판정의 배심원단'**이다. 판사(뇌)에게 여러 목격자(깊이 단서들)가 진술을 한다. 어두운 골목에서 봤다는 목격자(상대적 크기 단서)의 말보다, 또렷한 CCTV와 지문 증거를 제시한 목격자(교차 단서)의 말에 훨씬 무거운 가중치를 두어 "피의자는 유죄(대상은 가까이 있다)"라는 최종 판결을 내리는 구조다.

---

### 2. 이론 및 모델 간 연결 관계 (Interconnectivity)

**(1) 이론 간 연결관계 (Theories)**
근본적으로 **인간 정보 처리 이론(Human Information Processing)**이 인지의 유한함(지각, 주의, 기억의 한계)을 정의하면서 모든 논의가 시작된다. 이 인지적 한계로 인해 발생하는 시각 정보 선택 메커니즘을 **SEEV 모델**이 설명하고, 정보 처리 과정에서 발생하는 수학적 지각 왜곡을 **스티븐스의 법칙**이 규명한다. 이를 극복하고자 인간이 기계를 통제하기 위해 내면에 그리는 표상을 연구한 **멘탈 모델 이론**이 등장한다. 한편, 내부 인지 연산에 의존하는 정보 처리 이론의 대척점(보완점)으로서, 환경 자체가 제공하는 불변량을 무의식적으로 받아들이는 **생태학적 심리학(이중 지각 체계 중 직접 지각)** 이론이 병존한다. 이러한 이론적 토대를 오해하여 3차원 극사실주의 묘사가 무조건 좋다고 믿는 인지적 착각을 비판하는 것이 **순진한 사실주의** 관점이다.

**(2) 모델 간 연결관계 (Models)**
정적 표상(그래프)에서는 **그래프 지각 모델(탐색-부호화-비교)**의 연산 부하를 줄이기 위해 노이즈를 제거하는 **데이터-잉크 비율 원칙**과, 과제 형식에 디스플레이 형태를 맞추는 **근접성 호환성 원리(PCP)**가 상호보완적으로 작동한다. 동적 통제 표상(다이얼, 미터)에서는 멘탈 모델과 일치시키기 위해 **그림 사실주의 원리(PPR)**와 **이동 부품의 원리(PMP)**가 결합한다. 그러나 둘이 충돌할 경우, 단기 조작에는 PMP를, 장기 조작에는 PPR을 적용하는 **주파수 분리 하이브리드 디스플레이 모델**로 모순을 해결한다. 복잡한 시스템에서는 이 모든 호환성(PCP, 디스플레이 호환성, 생태학적 호환성)을 총망라하여 물리적 제약을 시각적 도형으로 승화시키는 **생태학적 인터페이스 설계(EID)** 모델이 최상위 아키텍처로 기능하며, 3차원 디스플레이의 모호성을 해결하기 위해서는 **가중 선형 단서 모델(WLCM)**을 활용해 고신뢰성 단서를 적절히 융합한다.

**(3) 이론과 모델의 연결 구조도 (Flow Chart & Mind Map)**

```text
[공간 디스플레이 이론 및 모델 지식 지도 (Concept Map)]

(Root) 인간-시스템 인지 및 지각의 한계 극복
  │
  ├── [1. 기초 심리/지각 이론]
  │     ├── 인간 정보 처리 & SEEV 모델 (주의 할당/탐색의 메커니즘)
  │     ├── 스티븐스의 법칙 (부피/면적 지각의 반응 압축 편향)
  │     ├── 멘탈 모델 이론 (보이지 않는 내부 시스템 작동에 대한 추론)
  │     └── 생태학적 심리학 (직접 지각 시스템을 통한 자동적 환경 반응)
  │
  ├── [2. 정적/2D 표상 최적화 모델 (Graphs)]
  │     ├── 그래프 지각 모델 (탐색 -> 부호화 -> 비교 연산 단계 최적화)
  │     ├── 데이터-잉크 비율 원칙 (비데이터 잉크 제거로 시각적 부하 최소화)
  │     └── 근접성 호환성 원리 (PCP) (통합 과제 ↔ 객체 디스플레이 결합)
  │
  ├── [3. 동적/3D 시스템 통제 모델 (Dials, 3D Navigation)]
  │     ├── 그림 사실주의 원리 (PPR) (변수의 아날로그 형태/방향 일치)
  │     ├── 이동 부품의 원리 (PMP) (조작자 멘탈 이동 방향과 지시기 일치)
  │     │    └── [해결 모델]: 주파수 분리 디스플레이 (PPR-PMP 충돌 해결)
  │     ├── 가중 선형 단서 모델 (WLCM) (3D 깊이 모호성 해결을 위한 단서 융합)
  │     └── 순진한 사실주의 비판 (과도한 3D 렌더링에 따른 인지 과부하 경계)
  │
  └── [4. 궁극의 통합 아키텍처]
        └── 생태학적 인터페이스 설계 (EID)
              (물리적/기능적 제약을 창발 자질로 시각화하여 PCP, PPR, PMP를 모두 포괄)
```

위 구조도에서 볼 수 있듯, 인간의 근본적인 '한계(정보 처리, 스티븐스 법칙)'를 정의하는 이론에서 출발하여, 이를 보완하기 위해 '노이즈 제거(데이터-잉크)' 및 '인지적 매핑(PCP, PPR, PMP)' 모델이 수립되며, 궁극적으로 환경 자체의 물리적 특성을 무의식적/직관적으로 묘사하는 EID와 생태학적 심리학으로 귀결되는 완전한 논리적 흐름을 갖추고 있다.

---


[^10]: "These are essentially the same as the bottom-up and top-down influences on visual information sampling described in the SEEV model in Chapter 3."

> [^11]: "Various graphical perception models postulate a general process of search... followed by the encoding of variables, and ultimately comparison of perceived elements with values stored in working memory (e.g., Casner, 1991; Gillan, 1995...)"

[^12]: "Stevens (1957, 1975) found that the relation between physical and perceived magnitude can be expressed by the power function called Stevens’ law, with the exponent representing the amount of response compression or expansion."

[^13]: "He argued for a data-ink ratio principle, which states that the amount of ink that does not depict data points should be kept to a minimum (Tufte, 2001)."

[^14]: "We saw that this display-cognitive compatibility could be defined in part by the proximity compatibility principle (PCP; Wickens & Carswell, 1995)."

[^15]: "It is important that dials and meters be compatible with the operator’s mental model of the system. The mental model... forms the basis for understanding the system, predicting its future behavior, and controlling its actions (Gentner & Stevens, 1983...)"

[^16]: "The principle of pictorial realism (PPR; Roscoe, 1968) has two parts... if a variable’s physical representation is analog, then its display representation should also be analog..."

[^17]: "Roscoe (1968) and Roscoe, Corl, and Jensen (1981) proposed the principle of the moving part (PMP)—that the direction of movement of an indicator on a display is compatible with the direction of movement of an operator’s mental model of the variable."

[^18]: "Smallman and St John (2005; Hegarty, Smallman, & Stull, 2012) labeled this misplaced faith in realistic information display as naïve realism."

[^19]: "When this configuration is done in a way to reflect the constraints of the natural physical system being represented, the resulting displays are called ecological interfaces (Vicente & Rasmussen, 1992; Vicente, 2002)..."

[^20]: "Psychologists have reached broad consensus that there are two qualitatively different systems for perceiving 3D space (DeLucia, 2008)."

[^21]: "Because of this anchoring of direct perception in the environment, it is closely associated with ecological psychology (Gibson, 1979; Warren, 2004)."

[^22]: "...an integration that is well explained by the weighted linear cue model (WLCM; Bruno & Cutting, 1988; Ichikawa & Saida, 1996; Knill, 2007; Young, Landy, & Maloney, 1993)."






# 실제 환경(교재 사례)에서 어떻게 문제와 해결책
본 교재(제4장 공간 디스플레이)는 인간의 인지적, 지각적 한계를 극복하기 위해 설계된 다양한 인터페이스 이론을 실제 산업 및 운송 사례를 통해 증명하고 있다. 제시된 이론들이 실제 환경(교재 사례)에서 어떻게 문제와 해결책을 도출했는지 체계적으로 정리하고, 이를 우리의 일상생활(새로운 사례)에 어떻게 적용할 수 있는지 교차 검증하여 제시한다. (*참고: 사용자가 언급한 '고릴라 실험' 등은 주의(Attention) 챕터의 내용으로 본 출처의 공간 디스플레이 범위에는 포함되지 않아 제외하였다.*)

---

### 1. 교재 속 현실 세계 적용 사례 (Real-world Case Studies from Text)

**1) 디스플레이 호환성(PMP와 PPR)의 충돌과 해결: 항공기 계기판 디자인**
*   **이론 적용:** 디스플레이 조작 직관성을 나타내는 이동 부품의 원리(PMP)와 물리적 현실성을 나타내는 그림 사실주의 원리(PPR)는 종종 충돌한다.
*   **기존 문제:** 항공기 자세 지시계에서 비행기가 기울 때 지평선이 도는 방식(Inside-out)은 PPR을 만족하나 PMP에 위배되고, 비행기 기호가 도는 방식(Outside-in)은 PMP를 만족하나 PPR을 위반하여 조종사 혼란을 야기했다.
*   **해결책:** Lintern, Roscoe, & Sivier (1990)는 초기 빠른 조작에는 비행기가 돌고(PMP 충족), 시간이 지나면 지평선이 서서히 회전하여 원상 복귀하는(PPR 충족) '주파수 분리 디스플레이(Frequency-separated display)'를 개발하여 이 인지적 모순을 해결하였다[^33].

**2) 광학 불변량(Optical Invariants)을 활용한 속도 지각 오류 해결: 항공 및 주행**
*   **이론 적용:** 직접 지각 시스템은 주변부 시야로 들어오는 전역 광학 흐름(Global optical flow)과 에지 율(Edge rate)을 통해 자아 운동 속도를 파악한다.
*   **기존 문제 1:** 보잉 747 항공기 도입 초기, 조종석이 기존 비행기보다 두 배 높아지면서 활주로 패턴이 망막을 지나는 광학 흐름 속도가 반으로 줄었다. 이로 인해 조종사들이 자신의 속도가 느리다고 착각하여 과속 택싱(Taxiing)을 하다 랜딩 기어를 파손하는 사고가 빈번했다 (Owen & Warren, 1987)[^34].
*   **기존 문제 2:** 영국의 교차로(Roundabout) 진입 시 운전자들이 속도를 충분히 줄이지 않아 사망 사고가 빈발했다.
*   **해결책:** Denton (1980)은 교차로에 진입할수록 도로에 칠해진 횡단 선(마커)의 간격을 점진적으로 좁게 배치했다. 물리적 속도가 같아도 시야를 통과하는 에지 율(Edge rate)이 급증하게 하여 운전자가 자신이 '가속'하고 있다고 착각하게 만들었고, 결과적으로 자발적인 급감속을 유도해 사고를 크게 줄였다[^35].

**3) 3D 깊이 단서(WLCM)의 오판: 소형차 후방 추돌 현상**
*   **이론 적용:** 뇌는 경험에 기반한 깊이 단서(친숙한 크기, 상대적 크기 등)를 통합하여 거리를 판단한다 (가중 선형 단서 모델).
*   **기존 문제:** 고속도로에서 소형차가 대형차보다 더 자주 후방 추돌을 당하는 현상이 발생했다.
*   **원인 규명:** Eberts & MacMillan (1985)은 뒤따르는 운전자가 일반적인 표준 차량의 크기(기대치)를 기준으로 앞차의 거리를 판단하기 때문임을 밝혀냈다. 소형차는 크기가 작으므로 뇌는 이를 '충분히 멀리 떨어져 있다'고 오판(상대적 크기 단서 왜곡)하게 만들었고, 결국 제동 타이밍을 놓치게 만든 것이다[^36].

**4) 생태학적 인터페이스 설계(EID): 스마트 크루즈 컨트롤(ACC)**
*   **이론 적용:** 물리적 시스템의 목적과 제약을 직관적인 창발 자질(도형, 기울기 등)로 치환하여 인지 부하를 줄인다.
*   **기존 문제:** 적응형 크루즈 컨트롤 사용 시, 운전자는 앞차와의 속도 차이, 거리, 충돌 시간(TTC) 등 복잡한 숫자를 머릿속으로 계산하여 브레이크 개입 여부를 결정해야 했다.
*   **해결책:** Seppelt & Lee (2007)는 시스템 상태를 숫자가 아닌 도형으로 시각화했다. 위험 상황에서는 정지 표지판 같은 삼각형(Yield) 모양으로, 안전한 거리에서는 빈 도로를 나타내는 사다리꼴 모양으로 화면이 변하게 하여 운전자가 악천후 속에서도 즉각적으로 제동을 판단할 수 있게 했다[^37].

**5) 3D 공간 음향의 정위 반사(Orientation Reflex) 활용**
*   **기존 문제:** 조종사나 통제관의 시각 정보가 포화(과부하) 상태일 때, 시각 알람만으로는 즉각적인 위험 인지가 어렵다.
*   **해결책:** Simpson, Brungart 등 (2004)은 교통 경고 시스템에 3D 공간 음향을 도입하여 소리가 실제 표적이 있는 3D 위치에서 들리도록 했다. 인간의 본능적인 정위 반사를 유도하여 표적 탐색 시간을 25% 단축시켰다[^38]. 추가로 최신 전투기인 F-35는 조종사에게 HMD를 통해 바닥을 투시하는 듯한 시야를 제공하며 시각적/청각적 상황 인식을 극대화한다[^39].

---

### 2. 일상생활로의 이론 확장 및 적용 (Everyday Life Verification)

내가 이해한 이론이 우리의 일상생활에 어떻게 적용될 수 있는지 다음의 3가지 새로운 사례를 통해 확인한다.

**사례 A: 스마트폰 내비게이션 (디스플레이 호환성 PPR vs PMP)**
*   **상황:** 초행길을 걸어가며 스마트폰 지도(카카오맵, 구글맵)를 볼 때.
*   **문제:** 지도가 항상 북쪽을 향해 고정(North-up)되어 있으면 실제 물리적 세계와 동일한 형태(PPR)를 유지하지만, 내가 우회전할 때 화면 속 내 아바타는 오른쪽으로 움직이는데 지도는 그대로 있어 내 직관(PMP)과 충돌하여 길을 잃기 쉽다.
*   **해결:** 최근 지도 앱의 **헤딩업(Heading-up / 나침반 연동) 모드**는 내가 몸을 돌리는 즉시 지도가 함께 회전하여 시야의 전방을 지도 위쪽에 맞춘다. 즉, PMP를 완벽히 만족시켜 직관적 길 찾기를 돕는 하이브리드 설계로 이론이 성공적으로 안착한 훌륭한 사례다.

**사례 B: 스마트폰/태블릿의 인강 시청 및 공부 (에지 율과 상대적 크기 편향)**
*   **상황:** 스마트폰으로 끝없이 스크롤되는 PDF 문서나 SNS 피드를 읽을 때.
*   **문제:** '무한 스크롤' 환경은 페이지 경계라는 에지(Edge)가 없어 에지 율(Edge rate)이 발생하지 않는다. 이로 인해 뇌는 자신이 얼마나 많은 정보를 얼마나 빠르게 소비했는지(속도감) 지각하지 못해 시간 가는 줄 모르고 스크롤하게 된다. 또한 스마트폰의 작은 화면은 글씨 크기(상대적 크기 단서)를 작게 만들어, 뇌가 이를 '대상과 멀다'고 착각하게 하고 나도 모르게 얼굴을 화면에 바짝 붙이는 거북목 원인이 된다.
*   **해결:** 무한 스크롤 대신 **페이지 단위 분할(Pagination)**을 도입하거나 진행 상태 바(Progress bar)를 두어 명확한 시각적 에지(Edge rate)를 제공하면, 독서량과 속도를 체감하여 집중력을 통제할 수 있다.

**사례 C: 뽀모도로(Pomodoro) 집중력 타이머 (생태학적 인터페이스 EID)**
*   **상황:** 공부할 때 남은 시간을 확인하기 위해 스마트폰 타이머를 켜둔 상황.
*   **문제:** "15:27"이라는 숫자로 표시된 타이머는 현재 시각과 내 목표 시각을 비교하는 정신적 연산(Mental operation)을 요구한다.
*   **해결:** '타임타이머(Time Timer)' 처럼 남은 시간이 직관적인 붉은색 원반 면적으로 표시되어 점차 줄어드는 앱을 사용하면, '붉은 면적의 크기 = 남은 시간'이라는 창발 자질(Emergent feature)을 제공한다. 인지적 암산 없이 곁눈질만으로 남은 자원을 즉각 통제할 수 있으므로 EID 이론이 학습 환경에 완벽히 구현된 예시다.

---

### 3. APA Reference List (연구 인용 정보)

*   Denton, G. G. (1980). *The influence of visual pattern on perceived speed*. (※ 교재 내에서 라운드어바웃 사고율 감소 실증 연구로 인용됨).
*   Eberts, R., & MacMillan, N. A. (1985). *Misperception of small cars*. (※ 교재 내에서 소형차 후방 추돌의 상대적 크기 왜곡 연구로 인용됨).
*   Lintern, G., Roscoe, S. N., & Sivier, J. E. (1990). *Display principles, control dynamics, and environmental factors in pilot training and transfer*. (※ 주파수 분리 하이브리드 디스플레이 연구).
*   Owen, D. H., & Warren, R. (1987). *Perception and control of self-motion*. (※ 보잉 747 택싱 속도 착각 현상 분석 연구).
*   Seppelt, B. D., & Lee, J. D. (2007). *Making adaptive cruise control (ACC) limits visible*. (※ EID 기반 사다리꼴/삼각형 인터페이스 평가).
*   Simpson, B. D., Brungart, D. S., et al. (2004). *3D audio system for traffic advisory warnings*. (※ 3D 오디오의 반응 시간 단축 연구).
*   Wikipedia. (2011). *Lockheed Martin F-35 Lightning II*. Retrieved from http://en.wikipedia.org/wiki/Lockheed_Martin_F-35_Lightning_II

---

[^33]: "A hybrid display called the frequency separated display (Figure 4.9(c); Lintern, Roscoe, & Sivier, 1990)... captures the best of both worlds, conforming in different ways to both principles."

[^34]: "When the Boeing 747 was first introduced, pilots often taxied the aircraft too fast... The 747 cockpit was about twice as far above the runway as the cockpits in other jets... As a result they achieved a true velocity that was unsafe (Owen & Warren, 1987)."

[^35]: "His solution was to decrease the spacing between road markers gradually and continuously as the distance to the roundabout decreased. A driver not slowing down appropriately would see the edge rate as increasing... Denton’s solution was imposed on the approach to a particularly dangerous roundabout in Scotland."

[^36]: "The driver behind judges separation, in part on the relative size of the vehicle in front... A smaller car will thus be perceived to be farther away relative to the expected norm; the following car will then inappropriately correct, by pulling too close... (Eberts & MacMillan, 1985)"

[^37]: "The display developed by Seppelt and Lee mapped the physical variables that the driver must monitor and control to certain characteristics of the display... If the driver’s vehicle was approaching the vehicle in front too quickly, a triangular shape (like a yield sign) was produced; if the vehicle in front was traveling more quickly... the display looked like a trapezoid..."

[^38]: "For example, response times to Traffic Advisory Warning alerts are reduced by 25 percent when 3D audio cues are available (Simpson Brungart et al., 2004)."

[^39]: "In fact, the cockpits of fifth-generation fighter aircraft (such as the F-35 joint strike fighter) make use of such cues and allow the pilot to see sensor imagery “through the floor” using a head-mounted display (http://en.wikipedia.org/wiki/Lockheed_Martin_F-35_Lightning_II, 2011)."
---

# 그림 설명 

그림 4.1부터 4.11까지는 정적 그래프에서부터 동적 시스템 통제에 이르기까지, 인간의 지각적 편향을 완화하고 시스템과 인지 구조 간의 호환성을 극대화하기 위한 공간 디스플레이 설계의 핵심 이론과 실제 사례들을 도식화하여 보여준다. 논리적 흐름에 따라 각 그림이 시사하는 개념과 인용 정보를 정리한다.

**1. 그림 4.1: 그래프의 종류와 과제 유형 (Graph Types and Task Dependency)**
그림 4.1은 동일한 데이터(공장 A와 B의 생산량)를 표상하는 세 가지 그래픽 형태인 막대그래프, 선 그래프, 파이 차트를 나열한다[^1]. 이 그림은 각 그래프 형태가 과제의 성격에 따라 유불리가 다름을 설명하기 위한 기초 자료다. 그래프 읽기 과제는 개별 값을 추출하는 점 읽기(Point reading), 두 값을 직접 비교하는 국소 비교(Local comparisons), 파생된 추세를 파악하는 전역 비교(Global comparisons), 그리고 전체 데이터를 아우르는 종합(Synthesis)으로 분류되며, 설계자는 과제 요구 사항에 맞는 그래픽 형태를 선택해야 함을 강조한다[^2].

![image](https://i.ibb.co/DHtSH55v/image.png)
<span class="fig-caption">[그림 3] 그래프의 예: 막대그래프 선, 파이 차트 </span>




**2. 그림 4.2: 근접성 호환성 원리 (Proximity Compatibility Principle, PCP)**
그림 4.2는 다양한 디스플레이 설계 연구들을 메타 분석한 결과 그래프로, 근접성 호환성 원리(PCP)의 타당성을 입증한다[^3]. 그래프의 x축은 과제의 유형(좌측: 초점적 과제, 우측: 통합적 과제)을 나타내며, y축은 통합된 객체 디스플레이(Object-display)의 이점 여부를 나타낸다. 과제가 고도의 통합(Information synthesis)을 요구할수록 분리된 형식보다 통합된 객체 디스플레이가 압도적으로 더 큰 성과 향상(Benefit)을 제공함을 증명하고 있다[^4].
![image](https://i.ibb.co/gqndJjM/image.png)
<span class="fig-caption">[그림 4] 근접 양립성 원리 </span>
분리된 형식보다 통합된 그래프들 사이에서 더 좋은 수행을 보인 연구들... 


**3. 그림 4.3: 포겐도르프 착시와 편향 완화 (Poggendorf Illusion and Debiasing)**
그림 4.3은 선 그래프를 읽을 때 발생할 수 있는 시각적 편향(Bias)을 설명한다. (a)는 사선이 끊겨 보이는 포겐도르프 착시를 보여주며, (b)는 이 착시로 인해 선 그래프 상의 값이 실제보다 과소평가되는 왜곡 현상을 나타낸다. (c)는 그래프 양쪽에 눈금이 있는 테두리 축을 명확히 제공(Marked edges)함으로써 이러한 착시 편향을 크게 줄일 수 있음(Debiasing)을 보여주는 실질적인 설계 팁이다[^5].

![image](https://i.ibb.co/kLVVQQ6/image.png)
<span class="fig-caption">[그림 5] 포켄도르프 착시 </span>
**<span style="color:#ff4444">포겐도르프 착시(Poggendorff Illusion)</span>**는 

1860년 독일의 물리학자 요한 크리스찬 포겐도르프(Johann Christian Poggendorff)에 의해 발견된 기하학적 착시 현상이다. 두꺼운 수직 띠나 직사각형에 의해 하나의 사선이 가려졌을 때, 차단된 양 끝의 사선이 서로 일직선상에 있음에도 불구하고 위치가 어긋나 보이는 현상을 의미한다(그림 4.3a 참조).

2. 인지적 원인
이 현상의 주요 원인에 대해서는 여러 인지 심리학적 가설이 존재한다.
- 각도 왜곡(Angle Misestimation): 뇌가 예각(Acute angle)을 실제보다 크게, 둔각(Obtuse angle)을 실제보다 작게 지각하려는 경향 때문에 발생한다는 이론이 지배적이다.
- 공간 지각의 오류: 시각 시스템이 평면상의 이미지를 3차원 공간으로 해석하는 과정에서 수직 막대를 사선보다 앞선 물체로 인식하며 발생하는 위치 편향으로 해석되기도 한다.

1) 그래프 상의 수치 왜곡 (Figure 4.3b)
선 그래프(Line graph)에서 데이터 포인트가 급격히 변하거나 특정 시각적 요소에 의해 가려질 때, 관찰자는 데이터의 연속성을 정확히 파악하지 못할 수 있다. Poulton(1985)의 연구에 따르면, 이러한 착시는 그래프 우측의 사선 위치를 실제보다 **과소평가(Underestimation)**하게 만드는 경향이 있다. 즉, **실제 데이터 값보다 낮은 위치에 선이 있다고 오인하게 되는 '굽어짐(Bending)' 현상**이 발생한다.

2) 편향 완화 전략 (Debiasing, Figure 4.3c)
공학 심리학 및 인간-컴퓨터 상호작용(HCI) 분야에서는 이러한 시각적 편향을 제거하기 위한 설계 지침을 다음과 같이 제시한다.
- ** 이중 축 프레임(Marked Edges):** 그래프의 좌측뿐만 아니라 우측에도 눈금이 있는 축(Graduated axis)을 배치함으로써 시각적 기준점을 강화한다. 이는 사선의 끝점 위치를 즉각적으로 비교할 수 있게 하여 착시를 억제한다.
- **그리드라인(Gridlines) 활용**: Amer(2005)는 그래프 내부에 격자선을 배치하는 것이 기준 프레임을 명확히 제공하여 위치 지각의 정확도를 높이고 편향을 감소시키는 데 효과적임을 입증하였다.



**4. 그림 4.4: 기울기 차이 지각의 편향 (Biases in Perceiving Differences)**
그림 4.4는 두 곡선 사이의 수직적 차이(Vertical separation)를 판단할 때 뇌가 겪는 오류를 보여준다[^7]. 기울기가 가팔라질수록 인간은 두 선 사이의 '수직 거리'가 아닌 눈에 띄는 '최단 유클리드 거리(시각적 분리)'를 기준으로 차이를 판단하기 때문에, 우측에서 두 선의 차이가 오히려 좁아진 것처럼 착각하게 된다. 이를 해결하기 위해 하단의 그래프처럼 '두 선의 차이값(Difference)' 자체를 직접 플롯하는 방식이 권장된다[^8].

![image](https://i.ibb.co/M4t43cF/image.png)
<span class="fig-caption">[그림 6] 그래프 쌍사이의 지각 </span>


**5. 그림 4.5: 정량적 판단을 위한 그래픽 형식의 위계 (Ranking of Graphical Methods)**
그림 4.5는 클리블랜드와 맥길(Cleveland & McGill)이 제안한 것으로, 두 양(Quantity)을 비교할 때 인간이 가장 정확하게 지각하는 그래픽 방법부터 가장 부정확한 방법까지 7단계의 위계를 나타낸다[^9]. '정렬된 길이(Aligned lengths, 예: 막대그래프)'가 비교 판단에 가장 효과적이며, 아래로 갈수록 면적(Area), 부피(Volume), 그리고 색상의 채도나 색상(Hue)이 위치하여 이들이 정량 비교에 매우 비효과적임을 경고한다. 이는 스티븐스의 법칙(Stevens' Law)과 관련된 지각적 압축/팽창 편향과 직결된다[^10].
![image](https://i.ibb.co/kV29qRH9/image.png)
<span class="fig-caption">[그림 7] 수량을 비교하기 위한 일곱가지 그래프 표시 방식</span>

**추가설명 **
**1. 클리블랜드-맥길의 그래픽 방법 위계 (Cleveland-McGill Hierarchy)**
1984년 클리블랜드와 맥길은 '기초 지각 작업(Elementary Perceptual Tasks)' 이론을 통해 데이터 시각화 요소가 인간의 정보 추출 정확도에 미치는 영향을 서열화하였다.
**지각 정확도에 따른 위계 분석** 
- 상위 단계 (Position & Length): 1단계인 **'공통 축에 정렬된 위치(Position on a common scale)'와 '정렬된 길이(Aligned lengths)'**는 인간이 가장 작은 차이도 민감하게 식별할 수 있는 영역이다. 막대그래프가 데이터 전달의 표준이 되는 심리학적 근거이다.
- 중간 단계 (Angle & Slope): <span style="color:#ff4444">파이 차트에서 사용되는 각도(Angle)나 기울기(Slope)는 위치 정보보다 판단 오차율이 높다</span>. 인**간의 뇌는 각도를 실제보다 과장하거나 축소하여 인식하는 경향**이 있기 때문이다.
- 하위 단계 (Area, Volume, Hue): 면적(Area)과 부피(Volume)는 정량적 비교에 있어 매우 비효과적이다. 특히 색상(Hue)은 명확한 서열이 없는 명목 척도(Nominal scale)에 가까워 정량적 크기 비교에는 적합하지 않다.

**스티븐스의 법칙(Stevens' Power Law)**
스티븐스의 법칙(Stevens' Power Law)과의 상관성그림 4.5의 위계는 심리물리학의 스티븐스의 법칙으로 설명된다. 이 법칙은 물리적 자극의 강도($I$)와 지각된 강도($S$) 사이의 관계를 나타내는 거듭제곱 법칙이다.
$$S = k \cdot I^{\beta}$$

- 지각적 정확도와 지수( $\beta$ ):   
  - 길이(Length): $\beta \approx 1.0$. 물리적 길이의 변화와 지각된 크기의 변화가 거의 일치하여 가장 정확한 판단이 가능하다.
  - 면적(Area): $\beta \approx 0.7 \sim 0.8$. 물리적 크기가 커질수록 실제보다 작게 느껴지는 지각적 압축(Perceptual compression) 현상이 발생한다. (예: 실제 면적이 4배 커져도 인간은 약 3배 정도만 커진 것으로 지각함)
  - 부피(Volume): $\beta \approx 0.5 \sim 0.6$. 압축 현상이 더욱 심화되어 정량적 비교에서 가장 큰 오차를 범하게 된다.

** 스티븐스의 법칙과 공학 심리학적 설계 시사점**
1. 편향의 최소화: 정밀한 수치 비교가 필요한 대시보드나 보고서에서는 반드시 위계의 상단에 위치한 '정렬된 길이' 혹은 '공통 축 상의 위치'를 활용해야 한다.
2. 면적 활용의 경계: 버블 차트(Bubble chart)와 같이 면적을 사용하는 경우, 스티븐스의 법칙에 따른 지각적 편향을 인지해야 한다. 사용자가 수치를 과소평가할 가능성이 높으므로 보조적인 숫자 표기나 가이드라인 제공이 필수적이다.
3. 인지적 부하 조절: 하위 위계(부피, 색상)를 사용하여 정량 정보를 전달하려 할 경우, 사용자의 인지적 노력이 급격히 증가하며 이는 의사결정의 오류로 이어질 수 있다.

**6. 그림 4.6: 비율 판단에서의 순환적 편향과 눈금의 효과 (Cyclical Bias in Proportion)**
그림 4.6은 파이 차트처럼 전체에 대한 비율(Proportion)을 판단할 때 나타나는 순환적 편향(Cyclical bias) 패턴을 보여준다[^11]. (a)에서는 과대평가와 과소평가가 반복되는 패턴을 보이며, (b)와 같이 눈금(Tick marks)을 중간 참조점(Reference points)으로 추가하면 편향의 주기가 두 배로 짧아지면서 시각적 판단의 전체적인 오류 폭이 크게 감소하는 교정 효과를 시각화하여 보여준다[^12].

![image](https://i.ibb.co/MY99DNL/image.png)
<span class="fig-caption">[그림 8] 그래프 판단에서 주기적 편중의 패턴들 </span>


**7. 그림 4.7: 물리적 시스템과 멘탈 모델의 호환성 (Representations of a Physical System)**
그림 4.7은 복잡한 동적 시스템 제어에서 고려해야 할 세 가지 표상(물리적 시스템, 디스플레이, 사용자의 멘탈 모델) 간의 관계를 도식화한 것이다[^13]. 이 그림은 물리적 시스템의 동역학이 디스플레이에 정확히 반영되는 생태학적 호환성(Ecological Compatibility: EC)과, 디스플레이의 구조가 사용자의 머릿속 멘탈 모델과 일치해야 하는 디스플레이 호환성(Display Compatibility: DC)이라는 두 가지 핵심 아키텍처를 정의한다[^14].

![image](https://i.ibb.co/V0y3hSGJ/image.png)
<span class="fig-caption">[그림 9] 멘탈모델과 물리시스템의 표상 </span>


**8. 그림 4.8: 지시계의 이동과 설계 원리 충돌 (Display Movement Dials)**
그림 4.8은 고도계 설계를 예시로 동적 디스플레이 원리 간의 충돌을 보여준다[^15]. 바늘이 움직이는 (a) 방식은 조작 방향과 바늘 방향이 일치하는 이동 부품의 원리(PMP)와, 높은 곳이 위를 향하는 그림 사실주의 원리(PPR)를 모두 만족하지만 좁은 범위만 표시할 수 있다. 반면, 눈금이 움직이는 (b)와 (c) 방식은 시야 범위를 넓힐 수 있지만 필연적으로 PMP나 PPR 중 하나를 위반하게 되는 모순을 시각화하였다[^16].

![image](https://i.ibb.co/TxyFXMzS/image.png)
<span class="fig-caption">[그림 10] 디스플레이 운동 </span>
 - 터치스크린과 마우스 스크롤 비교 
 - 수업보조자료 pdf 참고 
![image](https://i.ibb.co/CpgQ0tZ8/image.png)
<span class="fig-caption">[그림 11] 멘탈모델과 실제모델 사례 (스크롤)</span>


**9. 그림 4.9: 항공기 자세 지시계의 하이브리드 설계 (Aircraft Attitude Display)**
그림 4.9는 비행기 롤링(좌우 기울어짐) 상황에서 PPR과 PMP가 충돌하는 문제를 어떻게 해결하는지 보여준다[^17]. 지평선이 기우는 인사이드-아웃(a)은 PPR은 충족하나 PMP를 위반하고, 비행기가 기우는 아웃사이드-인(b)은 PMP는 충족하나 PPR을 위반한다. 그림 (c)는 초기 조작 시에는 비행기가 돌고(PMP) 나중에는 지평선이 돌면서 원상 복구되는(PPR) 주파수 분리 디스플레이(Frequency-separated display)라는 궁극의 하이브리드 타협안을 제시한다[^18].


![image](https://i.ibb.co/gL7fbq2J/image.png)
<span class="fig-caption">[그림 12] 항공기 하이드리드 설계</span>



**10. 그림 4.10: 생태학적 인터페이스 설계 사례 (Ecological Displays)**
그림 4.10은 물리적 제약이나 시스템의 목적을 직관적 기하학으로 치환한 생태학적 인터페이스 설계(EID)의 두 가지 성공 사례다[^19]. (a)는 원자력/화학 공정에서 질량 균형을 목수의 수준기(Carpenter's level)처럼 물방울의 위치와 선의 기울기로 보여주어 직관성을 높였다. (b)는 스마트 크루즈 컨트롤(ACC)에서 안전한 거리일 때는 사다리꼴(빈 도로), 제동이 필요한 위험 상황일 때는 정지 표지판 모양인 삼각형으로 창발 자질(Emergent feature)이 변하게 하여 즉각적 대처를 돕는다[^20].
![image](https://i.ibb.co/SwPQXrbr/image.png)
<span class="fig-caption">[그림 13] 항공기의 비행자세 디스플레이</span>
그림 4.10은 **생태학적 인터페이스 설계(Ecological Interface Design, EID)**의 핵심 원리인 **출현 특징(Emergent Features)**을 어떻게 실제 시스템에 적용하는지 보여주는 대표적인 사례이다

1. 그림 4.10(a): 카펜터 레벨 디스플레이 (Carpenter’s Level Display)
이 디스플레이는 원자력 발전소나 석유 화학 공정 등에서 질량 균형(Mass Balance) 상태를 직관적으로 파악하기 위해 설계되었다(Lau et al., 2008).
- 구조: 두 개의 수직 막대는 각각 '총 출력 질량(Total mass output)'과 '총 펌프 질량(Total mass pumped)'을 나타낸다. 두 막대 상단을 연결하는 선과 그 위의 '버블(Bubble)'이 핵심 요소이다.
- 출현 특징 (Emergent Feature): * 두 수치가 일치해야 하는 정상 상태에서는 연결선이 수평을 유지하며, 버블은 중앙의 해치 마크(Hatch mark)에 위치한다. 
  - 두 수치에 차이가 발생하면 선이 기울어지며 버블이 한쪽으로 치우친다(그림에서는 오른쪽 질량이 더 커서 버블이 우측으로 이동함).
- 설계의 이점: 운영자는 개별 수치를 숫자로 읽고 머릿속으로 계산할 필요 없이, **'기울기'와 '버블의 위치'**라는 시각적 형태만 보고도 시스템의 불균형을 즉각적으로 감지할 수 있다.

2. 그림 4.10(b): 적응형 크루즈 컨트롤 디스플레이 (ACC Display)
Seppelt와 Lee(2007)가 개발한 이 인터페이스는 운전자가 차량 간 거리와 속도를 제어하는 과업을 돕기 위해 물리적 변수를 기하학적 형상으로 매핑한 것이다.
- 주요 변수 매핑:
  - TTC (Time to Collision): 충돌까지 남은 시간.
  - THW (Time Headway): 앞차와의 시간 간격(거리/자차 속도).
  - Range Rate: 양 차량 간의 상대 속도 차이.

- 지각적 형상 변화:
  - 역삼각형 형태 (왼쪽): 자차가 앞차에 너무 빨리 접근하여 위험한 상황을 나타낸다. 이는 도로의 '양보(Yield)' 표지판과 유사한 형태를 유도하여 운전자에게 **브레이크 작동(Braking)**이 필요함을 직관적으로 경고한다.
 - 사다리꼴 형태 (오른쪽): 앞차가 더 빠르거나 안전거리가 확보된 상태를 나타낸다. '앞으로 뻗은 빈 도로'의 소실점과 유사한 형상을 만들어 안전한 주행 상태임을 인지시킨다.
 - 설계의 이점: 추상적인 수치(TTC, THW)를 직접 모니터링하는 대신, **'도형의 모양'**이라는 단일한 출현 특징을 통해 운전자가 상황의 위험성을 즉각적으로 판단하게 한다.

3. 생태학적 인터페이스 설계(EID)의 시사점
이 예시들은 공학 심리학의 다음 원칙들을 충실히 반영하고 있다.
- 작업 영역 분석(Work Domain Analysis): 시스템의 물리적 형태(파이프, 밸브 등)가 아닌, 물리적 법칙(질량 보존, 운동 법칙)과 기능적 목적을 시각화한다.
- 근접성 양립성 원칙(Proximity Compatibility Principle): 정신적으로 통합해야 할 정보(출력량 vs 펌프량)를 시각적으로도 가깝고 연결된 형태(선과 버블)로 배치한다.
- 인지적 부하 감소: 분석적 사고(계산 및 비교)가 필요한 작업을 지각적 작업(모양 및 기울기 확인)으로 전환함으로써 인간의 오류를 줄이고 대응 속도를 높인다.

- 인용 근거
  - Vicente, K. J. (2002). Ecological interface design: Progress and challenges. Human Factors.
  - Seppelt, B. D., & Lee, J. D. (2007). Making adaptive cruise control progressive: Adding a display of upcoming operations. Human Factors.
  - Lau, N., et al. (2008). Ecological interface design in the nuclear domain. IEEE Transactions on Systems, Man, and Cybernetics.


**11. 그림 4.11: 디스플레이 호환성의 통합 아키텍처 (Integrated Compatibility Framework)**
그림 4.11은 앞선 그림 4.7의 모델에 '과제 표상(Task representation)'을 추가하여 확장한 인지 호환성의 최종 프레임워크다[^21]. 이 모델은 디스플레이가 과제의 요구 수준(통합 혹은 분리)과 일치해야 한다는 근접성 호환성 원리(PCP)를 접목시켜, 생태학적 호환성(EC), 디스플레이 호환성(DC), 그리고 근접성 호환성(PCP)이라는 세 가지 핵심 원리가 어떻게 얽혀 인간의 성과를 극대화하는지 종합적인 구조를 보여준다[^22].

![image](https://i.ibb.co/TBzrHx5q/image.png)
<span class="fig-caption">[그림 14] 과제표상 추가</span>


---
[^1]: "FIGURE 4.1 An example of a bar graph, a line graph, and a set of pie charts. Each graph type depicts the same data: the production of two factories, A and B, over four years. Four graph reading tasks that could be performed with each graph are also described."

[^2]: 과제 유형(Point reading, Local comparisons, Global comparisons, Synthesis)에 따른 4.1 그림의 세부 설계 적용 논의.

[^3]: "FIGURE 4.2 Proportion of studies showing an object-display advantage (solid line) or disadvantage (dashed line) as a function of task type (focused, left; integrated, right). The figure illustrates the proximity compatibility principle."

[^4]: PCP 통합 과제 요구 수준과 객체 디스플레이 간의 유효성 상관관계인 4.2 그림 설명.

[^5]: "FIGURE 4.3 (a) The Poggendorf illusion: the two diagonal lines actually connect. (b) A line graph susceptible to “bending” from the Poggendorf illusion. (c) Debiasing of the Poggendorf illusion by marked edges on both sides."

[^6]: 시각적 편향을 교정하는 4.3 그림의 구체적 원리 설명.

[^7]: "FIGURE 4.4 Biases in perceiving differences between pairs of lines f1(x) and f2(x) with changing slopes. The bottom curve plots the difference f1(x) – f2(x), which is larger on the right than on the left."

[^8]: 유클리드 거리에 의한 편향과 직접 플롯 해결책을 담은 4.4 그림 설명.

[^9]: "FIGURE 4.5 Seven graphical methods for presenting quantities to be compared. The graphs are arrayed from most (top) to least effective (bottom)."

[^10]: 스티븐스의 법칙에 따른 그래픽 수단 효율성 위계를 담은 4.5 그림 설명.

[^11]: "FIGURE 4.6 Patterns of cyclical bias in judging graphs. (a) Bias as a function of true proportion for pie charts. (b) Bias as a function of true proportion when tick marks are added."

[^12]: 파이 차트의 순환적 비율 편향과 눈금의 디바이어싱 효과인 4.6 그림 설명.

[^13]: "FIGURE 4.7 Representations of a physical system. Two types of compatibility are portrayed: that between the physical system and a display (ecological compatibility: EC) and that between the display and the user’s mental model (display compatibility: DC)."

[^14]: 생태학적 호환성과 멘탈 모델 간의 디스플레이 호환성인 4.7 그림 설명.

[^15]: "FIGURE 4.8 Display movement. (a) Moving-pointer altimeter; (b) and (c) are moving-scale or fixed-pointer altimeters. The dashed arrows show the direction of display movement to indicate an increase in altitude."

[^16]: 지시계 이동 방향에 대한 PMP와 PPR의 충돌을 나타낸 4.8 그림 설명.

[^17]: "FIGURE 4.9 Aircraft attitude display. (a) inside-out, (b) outside-in, and (c) frequency-separated display. All displays show an aircraft banking left."

[^18]: PPR과 PMP의 모순을 해결하는 주파수 분리 하이브리드 설계인 4.9 그림 설명.

[^19]: "FIGURE 4.10 Examples of ecological displays. (a) Carpenter’s level display (Lau et al., 2008). ... (b) Adaptive cruise control display (Seppelt & Lee, 2007)."

[^20]: 물리적/기능적 제약을 기하학적 창발 자질로 치환한 EID 성공 사례 4.10 그림 설명.

[^21]: "FIGURE 4.11 This Figure augments Figure 4.7 with a task representation. The proximity compatibility principle (PCP) states that the display representation should be compatible with the task representation."

[^22]: 과제 표상(Task representation)과 결합된 호환성 통합 아키텍처 4.11 그림 설명.





---
# 3차원 자체운동 깊이 거리를 중심으로 직접 및 간접지각에 대한 지각시스템

인간이 3차원(3D) 공간을 지각하는 메커니즘은 신체가 환경 속에서 어떻게 이동하는지(자체 운동)를 통제하는 과정과, 환경 내 객체들 간의 깊이(Depth) 및 거리(Distance)를 판단하는 과정으로 나뉜다. 심리학계의 폭넓은 합의에 따르면, 인간의 뇌는 3차원 공간을 지각하기 위해 질적으로 완전히 다른 두 가지 시스템, 즉 **직접 지각(Direct Perception)**과 **간접 지각(Indirect Perception)**을 사용한다[^40]. 
이제 3차원 공간 지각의 핵심인 두 시스템의 개념을 정리하고, 교재에 제시된 관련 그림(Figure)들의 원리와 의미를 체계적으로 설명해보려고 한다. 

---
다음은 공간을 지각하는 2가지 방식이다. 

### 1. 두 지각 시스템의 기초 개념 (Direct vs Indirect Perception)

**1) 직접 지각 시스템 (Direct Perception)**
직접 지각은 관찰자가 3D 환경을 이동하는 **자체 운동(Egomotion)**을 통제하기 위해 근처의 객체와 표면을 지각하도록 고안된 자동적이고 무의식적인 시스템이다[^41]. 
*   시야 주변부와 중심부 전체에 분포된 **주변시(Ambient vision)**를 활용하며, 뇌의 **배측 경로(Dorsal pathways)**를 거친다. 
*   높은 수준의 인지적 추론(Cognitive inference)을 거의 필요로 하지 않으며, 시각적 이미지의 역동적인 기하학적 구조를 환경으로부터 직접 수용하는 '생태학적 심리학'에 기반한다[^42].

**2) 간접 지각 시스템 (Indirect Perception)**
간접 지각은 멀리 떨어져 있는 객체들의 깊이와 거리를 명시적이고 의도적으로 판단할 때 사용되며, 하향식 인지 추론과 경험(과거 기억)에 크게 의존하는 시스템이다[^43]. 
*   주로 시야의 중심인 **중심시(Focal/Foveal vision)**를 사용하며, 대상을 식별하는 뇌의 **복측 경로(Ventral pathways)**를 거친다[^44].
*   인지적 자원(주의력)을 많이 요구하며 정보 처리(Information processing) 이론과 맞닿아 있다.


<span class="tbl-caption"><표 5> Two Perceptual Systems</span>
| Direct Perception | Indirect Perception |
| --- | --- |
| Relatively automatic | Cognitive inference |
| Egomotion (close to observer) | Object perception (all distances) |
| Ambient (peripheral) vision | Focal (foveal) vision |
| Dorsal pathways | Ventral pathways |
| Ecological | Information processing |
  - TABLE 4.1 Two Perceptual Systems

-  **직접 지각 (Direct Perception)**
    - **Relatively automatic (상대적으로 자동적):** 지각이 환경으로부터 정보를 직접적으로 자동 추출하는 과정으로 간주된다.
    -    **Egomotion (close to observer) (자기 운동 지각):** 주로 관찰자 자신의 움직임(egomotion)과 환경과의 관계를 지각하는 데 중점을 둔다. 특히 가까운 거리에서의 행동과 어포던스(affordances) 지각에 중요하게 작용한다.
    -    **Ambient (peripheral) vision (주변 시야):** 주변 시야(peripheral vision)를 통해 환경의 전반적인 구조와 자신의 위치를 파악하는 데 사용되는 지각 방식이다. 이는 의식적인 주의 없이도 방향 감각과 균형을 유지하는 데 기여한다.
    -    **Dorsal pathways (등쪽 경로):** 뇌의 등쪽 경로(dorsal stream)와 관련이 깊으며, 주로 공간 정보 처리 및 행동 지향적 지각("어디/어떻게" 경로)을 담당한다.
    -    **Ecological (생태학적):** 지각을 환경과의 상호작용 속에서 유기체가 정보를 직접적으로 추출하는 생태학적 과정으로 설명한다.

- **간접 지각 (Indirect Perception)**
    - **Cognitive inference (인지적 추론):** 지각이 감각 정보를 인지적으로 추론하고 해석하여 세계의 표상을 구성하는 과정으로 이해된다.
    -   **Object perception (all distances) (객체 지각):** 다양한 거리에서 객체를 인식하고 식별하는 데 초점을 맞춘다. 이는 인지적 처리 과정을 통해 이루어진다.
    -   **Focal (foveal) vision (중심와 시야):** 중심와(fovea)를 사용하여 세부적인 객체 인식, 식별 및 의식적인 주의를 기울이는 지각 방식이다.
    -   **Ventral pathways (배쪽 경로):** 뇌의 배쪽 경로(ventral stream)와 관련이 깊으며, 주로 객체 인식 및 식별("무엇" 경로)을 담당한다.
    -   **Information processing (정보 처리):** 지각을 감각 데이터가 인지적 조작을 통해 변형, 해석 및 풍부화되는 정보 처리 모델로 설명한다.

---



### 2. 자체 운동(Egomotion)과 직접 지각 (그림 설명 포함)

직접 지각 시스템은 인지적 계산 없이도, 환경의 빛이 눈에 들어올 때 변하지 않는 기하학적 특성인 **'광학 불변량(Optical Invariants)'**을 자동 감지하여 방향과 속도를 통제한다[^45].

#### [그림 4.12]전통적인 비행 계기판(traditional flight instrument panel)'의 형태
![image](https://i.ibb.co/D0Xbkds/image.png)

다음은 이해를 돕기 위해서 개발한 시뮬레이터이다. 
** 그림 4-12의 시뮬레이터**
https://gemini.google.com/share/cee2a6816d92 
<img src="https://i.ibb.co/3mL4cTvW/image.png" alt="image" width="439" height="243" style="width:439px;height:243px">


그림 4.12는 **'전통적인 비행 계기판(traditional flight instrument panel)'**의 형태를 보여준다[^2]. 이 그림에는 대기 속도(Air speed), 선회/미끄러짐 지시기(Turn slip indicator), 방향 지시기(Directional indicator), 수직 속도(Vertical velocity), 자세 지시기(Attitude indicator), 그리고 고도계(Altimeter) 등 6개의 원형 다이얼 계기들이 각각 물리적으로 분리되어 배열되어 있다.
이 그림은 본 교재에서 인간이 환경 내에서 이동하는 **'자체 운동(Egomotion)'**과 이를 통제하는 **'직접 지각(Direct Perception)'**을 설명하는 대목에서, 과거의 전통적인 디스플레이 시스템이 지니는 인지적, 지각적 한계를 지적하기 위한 시각적 예시로 사용되었다. 이 그림과 연결되는 구체적인 한계점과 이론적 의미는 다음과 같다.
**1. 정보의 파편화와 정신적 통합(Mental Integration)의 부하**
가장 큰 문제는 조종사가 비행 중 자신의 정확한 공간적 위치와 움직임(Location and motion)에 대한 명확한 상황 인식을 얻기 위해서는, 그림 4.12처럼 여러 개의 분리된 계기들에 담긴 필수 정보들을 일일이 확인한 뒤 머릿속에서 하나로 통합(mentally integrated)해야만 한다는 점이다[^1]. 앞선 대화에서 다룬 '근접성 호환성 원리(PCP)'에 비추어 볼 때, 3차원 공간에서의 비행은 여러 축의 정보를 동시에 종합해야 하는 '통합 과제'이다. 그러나 전통적 계기판은 정보가 파편화된 '분리형 디스플레이' 구조를 띠고 있어 조종사에게 막대한 인지적 암산과 정보 접근 비용(Information access cost)을 강제한다.
**2. 중심시(Foveal Vision)에 국한된 설계의 한계**
인간은 물리적 세계를 이동할 때 인지적 계산이나 추론을 거의 요구하지 않는 '직접 지각' 시스템을 사용하며, 이는 망막 전체, 특히 시야 주변부(Peripheral vision)로 들어오는 광학 흐름(Optical flow) 등의 환경 단서를 통해 이루어진다. 그러나 그림 4.12의 전통적인 항공 계기판은 조종사가 시선을 좁게 집중해서 읽어야만 하는 중심시(Foveal vision)에만 철저히 의존하도록 설계되었다. 즉, 자체 운동(Egomotion)을 통제하는 데 가장 효율적인 인간의 주변시 기반 직접 지각 메커니즘을 전혀 지원하지 못한다는 치명적인 단점이 있다.
**3. 도출되는 해결책**
그림 4.12가 보여주는 이러한 '통합의 문제(Integration problem)'와 '중심시 편중' 문제를 해결하기 위해, 이후의 인터페이스 설계는 **통합형 3D 디스플레이(예: HITS)**를 도입하여 분산된 3축의 정보를 하나로 묶어주거나, 조종사의 주변시를 자극하는 **생태학적 디스플레이(예: Malcolm horizon display)**를 적용하여 인간의 자연스러운 직접 지각 능력을 활용하는 방향으로 발전하게 된다.

[^1]: "A second problem with the conventional aircraft instrument panel is that the information necessary for the pilot to obtain a good sense of location and motion is contained in several separate instruments (Figure 4.12), which must then be mentally integrated."

[^2]: "FIGURE 4.12 A traditional flight instrument panel."



**[그림 4.13] 질감 압축(Compression) 및 전개성(Splay)**
*   **개념:** 그림 4.13은 관찰자의 고도와 시선 기울기에 따라 환경의 선들이 어떻게 다르게 보이는지를 보여준다. **전개성(Splay)**은 평행한 두 선(예: 도로 양옆)이 멀어질수록 모이는 각도를 의미하며, **질감 압축(Compression)**은 수평선들 사이의 간격이 멀어질수록 좁아지는 변화율을 뜻한다[^46]. 
*   **그림 해석:** 그림의 왼쪽 패널은 높은 고도에서 들판을 내려다볼 때의 시야를, 오른쪽 패널은 낮은 고도에서 앞을 바라볼 때의 시야를 나타낸다. 고도가 달라짐에 따라 전개성의 각도와 압축의 기울기가 극명하게 변하는 것을 확인할 수 있으며, 조종사나 운전자는 이를 통해 자신의 고도를 즉각적으로 지각한다[^47].


![image](https://i.ibb.co/ycbP3df9/image.png)
<span class="fig-caption">[그림 15] Splay and compression</span>





**[그림 4.14] 광학 흐름 (Optical Flow)**
*   **개념:** 세계를 이동할 때 시야(망막)를 가로지르는 질감 점들의 순간적인 상대 속도를 의미하며, 시각 장을 가로지르는 화살표로 표현된다[^48]. 
*   **그림 해석:** 그림 중앙에 흐름이 전혀 발생하지 않고 모든 화살표가 뻗어나가는 중심점인 **'팽창점(Expansion point)'**이 존재하는데, 이는 관찰자의 순간적인 진행 방향(Heading)을 나타낸다[^49]. 또한 화살표의 길이(흐름의 속도)가 팽창점 아래쪽에서 더 길게 나타나는 것을 통해 항공기가 지표면을 향해 비스듬히 하강하고 있음을 직접적으로 지각할 수 있다.

이외에도 관찰자가 대상과 충돌하기까지 남은 시간을 수학적 계산 없이 시각적 팽창률로 알려주는 **충돌 시간(Tau)**[^50], 그리고 전반적인 속도감을 형성하는 **전역 광학 흐름(Global optical flow)**과 **에지 율(Edge rate)**이 자체 운동을 통제하는 주요 불변량으로 작용한다[^51].
*   **충돌 시간(Tau)**: 관찰자가 움직이는 대상과 충돌하기까지 남은 시간을 수학적 계산 없이 시각적 정보, 즉 대상의 망막상 팽창률을 통해 직접적으로 알려주는 불변량이다. 이는 특히 회피 행동과 같은 자체 운동 통제에 중요한 역할을 한다.
*   **전역 광학 흐름(Global optical flow)**: 시각 환경 내 모든 대상의 움직임으로 인해 관찰자의 망막에 투영되는 시각 정보의 전반적인 흐름 패턴을 의미한다. 이는 관찰자의 전반적인 속도감과 이동 방향을 인지하는 데 기여하는 주요 불변량이다.
*   **에지 율(Edge rate)**: 시각 환경 내 사물의 경계선(edge)이 관찰자의 망막에 나타나거나 사라지는 속도 또는 그 변화율을 의미한다. 이는 시각적 정보의 밀도 변화와 관련되며, 전역 광학 흐름과 함께 관찰자의 속도감을 형성하고 자체 운동을 통제하는 데 중요한 불변량으로 작용한다.
![image](https://i.ibb.co/8gZC9Dts/image.png)
<span class="fig-caption">[그림 16]  Optical flow.</span>


---

### 3. 깊이(Depth) 및 거리(Distance)와 간접 지각 (그림 설명 포함)

간접 지각 시스템은 주변 환경과 객체가 제공하는 **객체 중심 단서(회화적 단서)**와 인간의 생리적 특성인 **관찰자 중심 단서**를 뇌에서 통합하여 3D 구조를 추론한다[^52].

**[그림 4.15] 객체 중심 (회화적) 깊이 단서들**
*   **개념 및 그림 해석:** 그림 4.15는 화가가 평면 캔버스에 3D 깊이감을 표현하기 위해 사용하는 다양한 회화적 단서들을 하나의 장면에 종합하여 보여준다[^53]. 
*   **세부 요소:** 평행선이 모이는 **선형 원근법**(도로), 앞 건물이 뒤 건물을 가리는 **교차(Occlusion)**, 멀리 있는 대상일수록 화면 위쪽에 위치하는 **평면상 높이**(트럭 비교), 친숙한 대상의 망막 상 크기로 거리를 가늠하는 **상대적/친숙한 크기**, 멀어질수록 경계가 흐려지는 **대기 원근법**(옥수수밭) 등이 통합되어 정지된 2D 이미지임에도 불구하고 강력한 3D 거리감을 형성한다.

![image](https://i.ibb.co/KcMkNr1w/image.png)
<span class="fig-caption">[그림 17] Contains object-centered cues for depth, as described in the text.</span>


그림[4-16] Potential stimulus for recovery of structure through motion. 
<a href="https://gemini.google.com/share/6eae2522ec9b" target="_blank" rel="noopener">시각적 깊이 단서 및 운동구조 복원 시뮬레이터</a>
https://gemini.google.com/share/6eae2522ec9b

![image](https://i.ibb.co/60PkWQjh/image.png)
<span class="fig-caption">[그림 18] 정현파 시뮬레이션</span>




**[그림 4.17] 관찰 거리에 따른 깊이 단서의 효과 (Effectiveness of Cues)**
*   **개념 및 그림 해석:** 그림 4.17은 거리에 따라 특정 깊이 단서들의 유효성이 어떻게 달라지는지를 보여주는 그래프다[^54]. 공간은 팔이 닿는 개인 공간(Personal space), 던지고 뛰는 행동 공간(Action space), 저 멀리 보이는 조망 공간(Vista space)으로 나뉜다. 
*   **핵심 원리:** 눈 근육의 조절(Accommodation)이나 두 눈의 상 차이를 이용하는 양안 시차(Binocular disparity) 같은 생리적 단서와 운동 시차는 행동 공간(~30m) 이내에서 강력한 힘을 발휘하지만 거리가 멀어질수록 효과가 급감한다. 반면 교차(Interposition/Occlusion)나 상대적 크기 같은 회화적 단서는 조망 공간에서도 깊이를 판단하는 지배적인 단서로 기능함을 알 수 있다는 논리이다. 
 **거리별 깊이 단서 효율성 분석을 분석**한 것이다. 즉,  **Cutting과 Vishton(1995)**의 연구를 바탕으로, 관찰자와 객체 사이의 거리에 따른 9가지 주요 깊이 단서의 상대적 효율성 변화를 나타내고 있다. 
1. 공간의 세 단계 분류 (Three Regions of Depth)
그래프 상단에 표시된 바와 같이, 연구자들은 깊이 지각의 범위를 세 가지 기능적 공간으로 구분하였다.
- 개인 공간 (Personal Space, 약 2m 이내): 손을 뻗어 닿을 수 있는 거리로, 수렴 및 조절과 같은 생리적 단서가 유효하게 작용하는 유일한 구간이다.
- 활동 공간 (Action Space, 약 2m ~ 30m): 타인과 상호작용하거나 이동하며 물체를 조작하는 범위로, 운동 시차와 양안 시차가 핵심적인 역할을 한다.
- 전망 공간 (Vista Space, 약 30m 이상): 직접적인 물리적 접촉이 어려운 먼 거리로, 주로 회화적 단서(Pictorial cues)에 의존하여 공간 구성을 파악한다.


![image](https://i.ibb.co/jkWc6yFC/image.png)
<span class="fig-caption">[그림 19] Effectiveness of various depth cues as a function of distance</span>

2. 주요 단서별 특성 분석

**가. 거리 불변적 단서 (Distance-Invariant Cues)**
일부 단서들은 <u>거리에 상관없이 비교적 일정한 효율성을 유지</u>한다.
- **차폐 (Interposition/Occlusion):** 그래프의 최상단 점선으로 표시되며, **모든 거리에서 가장 높은 효율성을 보이는 지배적인 단서**이다. 객체가 다른 객체를 가리는 정보는 거리와 무관하게 전 공간에서 절대적인 우선순위를 갖는다.
- 상대적 크기 (Relative size): 거리가 멀어져도 효율성이 크게 감소하지 않고 유지되는 특성을 보인다.

**나. 거리 감쇠형 단서 (Distance-Attenuating Cues)**  
<u>근거리에서 매우 강력하지만 거리가 멀어질수록 효율성이 급격히 감소하는 단서</u>들이다.
- **양안 시차 (Binocular disparity)**: 활동 공간까지는 매우 정밀한 깊이 정보를 제공하지만, 30m를 넘어서며 효율성이 급락한다. 이는** 두 눈의 간격이라는 물리적 한계** 때문이다.
- **운동 시차 (Motion parallax)**: 관찰자의 이동에 따른 상대적 속도 차이는 근거리에서 매우 효과적이며, 양안 시차보다 조금 더 먼 거리까지 유효성을 유지한다.
- **수렴 및 조절 (Convergence and accommodation)**: 2m 이내의 개인 공간에서만 작동하며 그 이후에는 효율성이 0에 수렴한다.

**다. 거리 비례형 단서 (Distance-Increasing Cues)**
 <u>거리가 멀어질수록 지각적 중요도가 상승하는 단서</u>이다.
- 공중 원근법 (Aerial perspective): 대기의 산란 현상으로 인해 멀리 있는 물체가 흐릿해 보이는 현상으로, 전망 공간(100m 이상)에서 그 효율성이 유의미하게 상승한다.
- 질감 구배 (Textural gradient): 표면 밀도의 변화를 통해 깊이를 지각하며, 원거리로 갈수록 단위 면적당 밀도가 높아지므로 정보 가치가 유지되거나 소폭 상승한다.

Cutting과 Vishton(1995)의 모델은 인간의 깊이 지각이 특정 단서 하나에 의존하는 것이 아니라, **가용 가능한 여러 단서의 가중치 합산(Weighted integration)**을 통해 이루어지고 있음을 주장하였다. 특히, **Allison et al.(2009)**은 현대의 VR/AR 디스플레이 환경에서 이러한 자연적 한계를 넘어 인위적으로 단서의 효율성을 조절할 수 있음을 지적하였다. 예를 들어, **입체 디스플레이 기술을 통해 전망 공간에 위치한 물체에 대해서도 인위적인 양안 시차를 부여함으로써 인간의 자연적 시각 한계를 보완하는 성능 향상이 가능**하다.
  - Cutting, J. E., & Vishton, P. M. (1995). Perceiving layout and knowing distances: The integration, relative potency, and contextual use of different information about depth.
  - Allison, R. S., Gillam, B. J., & Vecellio, E. (2009). Binocular depth discrimination and estimation beyond interaction space.

 ### 실제 사례 
**제미나이 시뮬레이터 **
 https://gemini.google.com/share/359de991973e
<p><img src="https://i.ibb.co/qLdNxNSp/image.png" alt="image" width=500></p>


**가. 거리 불변적 단서 (Distance-Invariant Cues)**
*   **차폐 (Interposition/Occlusion):**
- **현실 사례:** 숲에서 나무들이 겹쳐 보이는 경우, 앞쪽 나무가 뒤쪽 나무를 가리면 앞쪽 나무가 더 가깝다는 것을 명확히 인지한다. 이는 나무들이 수 미터 떨어져 있든 수십 미터 떨어져 있든 동일하게 적용되는 절대적인 단서이다.
*   **상대적 크기 (Relative size):**
- **현실 사례:** 도로 위에 동일한 규격의 가로등이 일렬로 서 있는 경우, 시야에서 더 작게 보이는 가로등을 더 멀리 있다고 지각한다. 이 지각은 가로등이 가까이 있든 멀리 있든 그 효율성이 크게 변하지 않는다.

**나. 거리 감쇠형 단서 (Distance-Attenuating Cues)**
*   **양안 시차 (Binocular disparity):**
- **현실 사례:** 바늘에 실을 꿰는 것과 같이 매우 정밀한 근거리 작업을 할 때, 양안 시차는 두 눈에 맺히는 상의 미세한 차이를 통해 정확한 깊이 정보를 제공한다. 그러나 30미터 이상 떨어진 산봉우리의 상대적 깊이를 판단할 때는 양안 시차가 거의 무의미해진다.
*   **운동 시차 (Motion parallax):**
- **현실 사례:** 자동차를 타고 이동할 때, 창밖의 가까운 가로수나 건물은 빠르게 스쳐 지나가지만, 멀리 있는 산이나 구름은 느리게 움직이거나 거의 움직이지 않는 것처럼 보인다. 이러한 상대적 속도 차이는 근거리에서 매우 효과적인 깊이 단서이다.
*   **수렴 및 조절 (Convergence and accommodation):**
- **현실 사례:** 스마트폰 화면을 보거나 책을 읽을 때, 눈동자가 안쪽으로 모이고(수렴) 수정체의 두께가 조절되어(조절) 화면이나 책의 거리를 정확히 인지한다. 그러나 2미터 이상 떨어진 벽을 볼 때는 이러한 안구 운동이나 수정체 조절이 깊이 지각에 거의 기여하지 않는다.

**다. 거리 비례형 단서 (Distance-Increasing Cues)**
*   **공중 원근법 (Aerial perspective):**
- **현실 사례:** 멀리 떨어진 산맥을 바라볼 때, 가까운 산은 선명하고 색이 뚜렷하게 보이지만, 멀리 있는 산은 대기 중의 먼지와 수증기로 인해 푸르스름하고 흐릿하게 보인다. 이러한 흐릿함의 정도는 거리가 멀어질수록 더욱 명확한 깊이 단서가 된다.
*   **질감 구배 (Textural gradient):**
- **현실 사례:** 자갈밭이나 잔디밭을 바라볼 때, 가까운 곳의 자갈이나 잔디는 개별적인 질감이 뚜렷하게 보이지만, 멀리 있는 부분은 질감의 밀도가 높아져 점차 촘촘하고 부드러운 평면처럼 보인다. 이러한 질감의 변화는 원거리에서 깊이를 지각하는 데 중요한 역할을 한다.



**[그림 4.18] 가중 선형 단서 모델 (WLCM)과 단서 우위성**
*   **개념:** 뇌는 깊이를 판단할 때 여러 단서의 신뢰성에 따라 가중치를 부여하여 통합하는데, 이를 가중 선형 단서 모델(WLCM)이라 한다[^55].
*   **그림 해석:** 그림 4.18은 단서들이 중첩될 때 깊이감이 어떻게 강력해지는지, 그리고 특정 단서가 어떻게 다른 단서를 압도(우위성)하는지를 명확히 보여준다[^56]. 
    - 상단 좌측: 상대적 크기 단서만 존재하여 B가 뒤에 있다는 약한 느낌을 준다.
    - 하단 좌측: 평면상 높이 단서가 추가되어 깊이감이 더 명확해진다.
    - 하단 우측: 상단 좌측과 똑같은 위치/크기 배열이지만, B가 A의 윤곽선을 가리는 **교차(Occlusion)** 단서를 추가했다. 그 결과 뇌는 크기나 높이 단서를 무시하고 단번에 B가 A보다 '앞에' 있다고 판단한다. 이는 교차 단서가 WLCM 통합 과정에서 매우 높은 가중치를 지니는 지배적 단서(Dominant cue)임을 증명한다.

![image](https://i.ibb.co/bgfw82LF/image.png)
<span class="fig-caption">[그림 20] 가중 선형 단서 모델 (WLCM)</span>

 깊이 통합 수식 (Mathematical Framework)뇌의 최종 깊이 판단 $D$는 다음과 같은 선형 결합 모델로 시뮬레이션할 수 있다. 
$$D = \sum_{i=1}^{n} w_i C_i = w_{size}C_{size} + w_{height}C_{height} + w_{occlusion}C_{occlusion}$$
단, $\sum w_i = 1$ 이며, 차폐(Occlusion) 단서가 활성화될 경우 $w_{occlusion}$의 값이 급격히 상승하여 타 단서의 영향을 압도(Dominance)하도록 알고리즘을 구성할 수있다.


---
**[주석 및 원문 인용]**

[^40]: "Psychologists have reached broad consensus that there are two qualitatively different systems for perceiving 3D space (DeLucia, 2008)."

[^41]: "We describe first a system for direct perception, which functions somewhat automatically and is designed for perceiving nearby objects and surfaces as we move through the 3D world, a process called egomotion."

[^42]: "It employs dorsal visual pathways leading to the cortex... Because of this anchoring of direct perception in the environment, it is closely associated with ecological psychology"

[^43]: "In contrast, a system for indirect perception is much more dependent on inference and higher-level cognition. This system is useful for more explicit, deliberate judgments of depth and distance of objects"

[^44]: "It makes use of focal (usually foveal) vision, using ventral visual pathways, as opposed to ambient (or peripheral) vision"

[^45]: "Gibson (1979) identified a set of environmental properties that the visual system can detect to assist in control of egomotion. These properties have sometimes been referred to as optical invariants"

[^46]: "Splay and compression. Splay is defined by the angle of the two receding lines. Compression is defined by the gradient of separation between the horizontal lines from the front (bottom) to the back (top)."

[^47]: "On the left, the perception is of being high above the field looking down. On the right, the observer is at low altitude, looking forward. Note how both splay and compression change with altitude."

[^48]: "Optical flow. The arrows indicate the momentary velocity of texture across the visual field that the pilot would perceive on approach to landing."

[^49]: "The expansion point is that place where there is no flow but from which all flow radiates, and it indicates the direction of momentary heading (Warren, 2004)."

[^50]: "Time-to-contact (tau). Tau specifies the time remaining until an observer makes contact with an object, assuming that the speed of the observer or the object is constant"

[^51]: "Our subjective perception of speed is heavily determined by global optical flow... Edge rate can be defined as the number of edges or discontinuities that pass across the observer’s visual field per unit time."

[^52]: "Some cues are characteristics of the object or world we perceive, and others are properties of our own visual system. We refer to these as object-centered and observer-centered cues respectively."

[^53]: "FIGURE 4.15 Contains object-centered cues for depth, as described in the text... Object-centered cues are sometimes called pictorial cues because they are the kinds of cues that an artist could use in a picture to convey a sense of depth."

[^54]: "The various cues are not all equally effective, and their effectiveness depends on the viewing distance, as shown in Figure 4.17... The figure separates the continuum of depth into three regions: personal, action, and vista space."

[^55]: "an integration that is well explained by the weighted linear cue model (WLCM... The model essentially describes the cues as varying in the reliability and precision with which they convey depth information"

[^56]: "FIGURE 4.18 Illustrating the weighted linear cue model (WLCM). The Figure illustrates the added sense of depth by added cues, and the role of cue dominance by occlusion."


## 추가 그림 설명 
교재의 그림 4.19부터 4.23까지는 3차원(3D) 공간을 2차원 평면 디스플레이에 표상할 때 발생하는 인지적 이점과 지각적 한계, 그리고 이를 극복하기 위한 설계적 해결책을 체계적으로 보여준다. 각 그림의 세부 내용과 연결되는 핵심 개념 및 인용 정보를 논리적 흐름에 따라 정리하면 다음과 같다.

**1. 그림 4.19: 3D HITS 디스플레이와 근접성 호환성 원리 (PCP)**
*   **개념 설명:** 그림 4.19는 조종사에게 지시된 비행 경로를 안내하는 3D 'Highway in the sky (HITS)' 디스플레이(a, c)와 이를 3개의 평면으로 나눈 분할 표상(b)을 비교한다. 3D 화면은 상대적 크기(Relative size)와 선형 원근법(Linear perspective)이라는 깊이 단서를 활용하여 비행 경로의 3차원적 깊이감을 명확히 제시한다[^1]. 
*   **이론적 연결:** 항공기를 통제하는 과제는 본질적으로 3차원 공간 전체의 움직임을 하나로 통합(Integration)해야 하는 과제이다. 따라서 근접성 호환성 원리(PCP)에 입각했을 때, 분할된 평면 디스플레이보다는 요소들이 통합된 3D 디스플레이가 인지적으로 훨씬 효과적이다[^2].
*   **연구 인용:** Haskell & Wickens (1993); Prinzel & Wickens (2008).

![image](https://i.ibb.co/0y7R4JpV/image.png)

시뮬레이터 
https://gemini.google.com/share/1fa90121e26e






**2. 그림 4.20: 3D 지형 디스플레이와 전역적 형태 이해 (Shape Understanding)**
*   **개념 설명:** 동일한 지형을 2D 등고선 지도(좌측)와 명암이 들어간 3D 원근 뷰(우측)로 비교한 그림이다.
*   **이론적 연결:** "A 지점에서 B 지점이 보이는가?"와 같은 가시성 판단이나 지형의 전반적인 형태(Layout)를 파악해야 하는 형상 이해(Shape understanding) 과제, 즉 전역 상황 인식(Global situation awareness)을 수행할 때는 사실적인 3D 원근 디스플레이가 2D 평면도보다 압도적으로 우수함을 증명한다[^3].
*   **연구 인용:** Hollands et al. (2008); St John et al. (2001).

![image](https://i.ibb.co/Z1ztMFPJ/image.png)
<span class="fig-caption">[그림 21] 2D topographic map and a 3D perspective representation </span>



### 그림 4-19와 4-20의 차이점은?
그림 4.19와 4.20은 모두 3차원(3D) 디스플레이가 평면(2D) 디스플레이보다 우수한 인지적 이점을 제공하는 사례를 보여주지만, 적용되는 과제의 성격, 비교 대상, 그리고 이를 뒷받침하는 이론적 개념에서 명확한 차이점을 가진다.

**1. 과제의 목적과 내용 (Task Purpose)**
*   **그림 4.19:** 항공기 조종사에게 지시된 비행 경로(Commanded route)와 실제 위치를 안내하기 위한 '3D 하늘의 고속도로(HITS; Highway in the sky)' 디스플레이를 다룬다[^1]. 즉, 3차원 공간에서 궤적을 제어하고 항로를 추적하는 비행 조종 과제에 맞추어져 있다.
*   **그림 4.20:** 정적인 지형의 전반적인 형태(Layout)를 파악하거나 3D 객체의 형상을 이해하는 과제를 다룬다[^2]. 예를 들어, 특정 지형의 "A 지점에서 B 지점이 보이는가?"와 같은 가시성 판단이나 전역 상황 인식(Global situation awareness)이 필요한 과제에 해당한다[^3].

**2. 비교 대상의 차이 (Comparison Target)**
*   **그림 4.19:** 비행 경로 정보를 하나의 3D 통합 화면으로 보여주는 것과, 동일한 정보를 세 개의 평면(Tri-planar)으로 분할하여 표상한 것을 비교한다[^4]. 
*   **그림 4.20:** 동일한 산악 지형을 2D 등고선 지도(Topographic map)로 나타낸 것과, 사실적인 음영이 들어간 3D 원근 뷰(Perspective view)로 나타낸 것을 비교한다[^3].

**3. 기반하는 인지적 원리 (Cognitive Principles)**
*   **그림 4.19 (통합 과제와 PCP):** 항공기를 비행하는 것은 본질적으로 공간의 세 축(가로, 세로, 높이)에 걸친 움직임을 머릿속에서 하나로 통합(Integration)해야 하는 과제이다. 따라서 다중 정보의 호환성을 강조하는 근접성 호환성 원리(PCP; Proximity Compatibility Principle)에 입각했을 때, 분할된 평면 디스플레이보다는 요소들이 합쳐진 3D 디스플레이가 인지적으로 훨씬 유리하다[^5]. 이 디스플레이는 선형 원근법과 상대적 크기 같은 깊이 단서를 통해 3차원 경로를 직관적으로 전달한다[^4].
*   **그림 4.20 (형상 이해):** 특정 공간의 전체 지형이나 3D 객체의 형태를 총체적으로 이해(Shape understanding)해야 하는 상황에서는, 등고선을 해독하기 위한 복잡한 정신적 연산 없이 즉각적인 깊이감을 제공하는 사실적인 3D 원근 디스플레이가 평면도보다 압도적인 우위를 점함을 보여준다[^2].

결론적으로, 그림 4.19는 **근접성 호환성 원리(PCP)**에 기반하여 비행과 같은 능동적 '통합 과제'에서 3D 디스플레이가 주는 이점을 설명하며, 그림 4.20은 정적 지형이나 환경의 **'형상 이해(Shape understanding)' 및 전역 상황 인식**을 돕는 데 있어 3D 표상의 이점을 강조한다는 점에서 핵심적인 차이가 있다.




---

[^1]: "One example of such a 3D display is the so called 3D highway in the sky (HITS) display that shows a pilot’s commanded route through and actual position within the sky (Figure 4.19..."

[^2]: "Tasks requiring shape understanding, such as judging the layout of terrain, or the general shape of 3D objects, are best performed with realistic 3D perspective displays."

[^3]: "In Figure 4.20, if you were asked whether you could see point A from point B, you can generally do this better with the realistically shaded, 3D perspective view display (right) than with the plan view topographic map (left)."

[^4]: "The role of relative size and linear perspective in signaling the depth component of the command path is clearly evident in Figure 4.19a, in a way that is missing in the “tri-planar” presentation of the same information in 4.19b."

[^5]: "Within the context of the proximity compatibility principle, the advantage can be seen because flying an aircraft clearly requires integration of motion across all three axes. Hence such an integration task is best supported by the integrated display"



**3. 그림 4.21: 항공 관제 디스플레이의 3D 한계와 평면 분할 (Co-planar) 해결책**
*   **개념 설명:** 충돌 위험이 있는 두 항공기의 공간적 위치를 3D(a), 평면 분할(b: 상단 X-Y 지도, 하단 Z-Y 고도), 인공적 참조 프레임이 추가된 3D(c)로 구분하여 보여준다.
*   **이론적 연결:** 비행 조종(통합 과제)과 달리, 항공 관제사들이 충돌 분리도를 판단할 때는 3D 표상이 오히려 성과를 저하시킨다[^4]. 이는 3차원의 공간이 2D 화면으로 압축되면서 발생하는 위치의 근본적인 모호성 때문이다[^5]. 관제사의 과제는 X-Y 지도 상의 거리와 고도(Z) 분리를 각각 독립적으로 판단해야 하는 '초점적 주의(Focused attention)' 과제이므로 평면 분할(Co-planar) 디스플레이가 더 적합하다[^6]. 3D를 고수해야 한다면 그림 (c)처럼 기둥(Posts)과 격자(Gridlines)를 제공해야 한다.
*   **연구 인용:** May, Campbell, & Wickens (1996); Ellis, McGreevy, & Hitchcock (1987).


![image](https://i.ibb.co/7tzDFK4X/image.png)
<span class="fig-caption">[그림 22] Three representations of a traffic conflict display</span>




**4. 그림 4.22: 시선 모호성(LOS Ambiguity)과 깊이 압축(Compression)**
*   **개념 설명:** 그림 4.21(a)에서 관찰된 3D 디스플레이의 한계가 왜 발생하는지 그 근본 원인을 도식화한 그림이다. 
*   **이론적 연결:** 상단의 물리적 현실에서는 A가 가장 멀리 있지만, 하단의 2D 투영 화면에서는 A와 B가 인접한 것처럼 보인다. 관찰자의 2D 시야(망막) 상에서 동일한 상을 맺게 하는 3D 깊이 축 상의 객체 위치는 무한하므로, 정확한 상대적 거리를 판별할 수 없는 **시선 모호성(Line of Sight Ambiguity)**이 발생한다[^7]. 이 모호성은 모니터 테두리나 빛 반사와 같은 평면성 단서(Flatness cues)로 인해 화면이 2D라는 사실이 뇌에 각인될 때 더욱 심해진다[^8]. 또한, 시선 방향(깊이 축)으로의 거리 정보는 화면에서 시각적으로 심하게 압축되므로, 객체 간 미세한 차이를 구분하는 해상도(Resolution)를 심각하게 떨어뜨린다[^9].
*   **연구 인용:** McGreevy & Ellis (1986); Young et al. (1993); Stelzer & Wickens (2006).

![image](https://i.ibb.co/gbhZ74tH/image.png)
<span class="fig-caption">[그림 23] 상대적 깊이(상대적 깊이)</span>



**5. 그림 4.23: 3D 개념적 그래프의 지각 왜곡과 인공적 프레임워크**
*   **개념 설명:** 실제 3차원 물리 공간이 아닌 정량적 데이터(예: 막대그래프)를 3D 그래픽으로 렌더링했을 때 발생하는 부작용과 그 해결책을 보여준다.
*   **이론적 연결:** 그림 (a)의 좌측 막대들은 실제 데이터 높이가 같지만 깊이 렌더링으로 인해 뒤쪽 막대가 더 커 보이고, 우측 막대들은 실제로는 뒤쪽이 더 작음에도 원근법 왜곡으로 인해 같아 보이는 치명적인 지각 오류를 유발한다[^10]. 이를 바로잡기 위해 그림 (b)와 같이 막대에 눈금(Tick marks)이라는 인공적 프레임워크(Artificial frameworks)를 추가하면, 관찰자가 깊이 왜곡에 속지 않고 데이터의 연장 정도(크기)를 정확히 판독할 수 있게 된다[^11].
*   **연구 인용:** Hollands et al. (2002).



![image](https://i.ibb.co/B5374rxm/image.png)
<span class="fig-caption">[그림 24] 깊이지각을 통한 크기 </span>

---

[^1]: "The role of relative size and linear perspective in signaling the depth component of the command path is clearly evident in Figure 4.19a..."

[^2]: "...flying an aircraft clearly requires integration of motion across all three axes. Hence such an integration task is best supported by the integrated display (Haskell & Wickens, 1993)."

[^3]: "Tasks requiring shape understanding, such as judging the layout of terrain, or the general shape of 3D objects, are best performed with realistic 3D perspective displays."

[^4]: "Here research has shown that the 3D representation of the airspace is inferior for air traffic controllers (May, Campbell, & Wickens, 1996; Wickens, Miller, & Tham, 1996)..."

[^5]: "The position of the two aircraft is inherently ambiguous given that the three spatial dimensions have been collapsed onto a 2D viewing surface (McGreevy & Ellis, 1986)."

[^6]: "...the strength of the co-planar advantage for air traffic controllers is related to the fact that controllers do not really perform an integration task as they judge separation. Rather, they approach separation more as a two-stage judgment: XY (map) separation, and altitude separation are judged separately."

[^7]: "It is impossible to judge, since there are many (indeed, an infinite number of) locations of A along the depth axis and the vertical axis that could produce the same relative position of A and B from the viewer’s perspective."

[^8]: "Here certain features of the viewing environment (e.g., the display frame, reflectance from the screen) signal loud and clear to the observer that this is indeed a 2D image."

[^9]: "There is also a second cost to 3D displays, closely related, but not identical to LOS ambiguity, and this is compression along the depth axis... its compression will still degrade the resolution with which differences can be judged"

[^10]: "For example, if asked to judge the relative heights of two bars in the 3D graph shown in Figure 4.23(a) it is difficult to do this accurately, and the error increases with the distance between the bars in the simulated depth plane (Hollands et al., 2002)."

[^11]: "The tickmarks placed on the bars of Figure 4.23(b) provide a framework that helps judgments of extent (height, in this case)."


<div class="page-break"></div>



# discussion 

## 스티븐스의 법칙(Stevens' Law)이 그래프 설계에 주는 실질적 팁은?
스티븐스의 법칙(Stevens' Law)은 그래프 설계에 있어 인간의 지각적 편향(Bias)을 최소화하기 위한 두 가지 핵심적인 실질적 지침을 제공한다. 이 법칙은 물리적 크기와 인간이 지각하는 크기 사이의 관계가 거듭제곱 함수(Power function)로 표현되며, 그 지수(Exponent)에 따라 반응 압축(Response compression) 또는 반응 팽창(Response expansion)이 발생함을 설명한다[^23]. 이로 인해 발생하는 정보 왜곡을 막기 위한 실질적 팁은 다음과 같다.

첫째, **스티븐스의 지수가 1.0과 다른 지각적 연속체의 사용을 배제해야 한다**[^24]. 면적이나 부피와 같은 시각적 차원은 지수가 1.0보다 작아, 물리적 크기가 커질수록 지각된 크기의 증가폭이 점점 줄어드는 반응 압축을 유발한다[^25]. 따라서 그래프에서 거대한 면적이나 3D 부피를 사용하여 양을 표현하면 독자는 실제 데이터보다 이를 심하게 과소평가하게 된다[^26]. 반대로 색상의 채도(Color saturation)는 반응 팽창을 일으켜 실제 값을 과대평가하게 만든다[^27]. 결과적으로 그래프 설계자는 지각적 오류를 방지하기 위해 지수가 1.0에서 벗어나는 면적, 부피, 채도 등의 사용을 피하고, 왜곡이 적은 '정렬된 길이'와 같은 차원을 우선적으로 선택해야 한다[^28].

둘째, **눈금(Tick marks)과 같은 중간 참조 지점을 명확히 제공해야 한다**[^29]. 원형 차트나 누적 막대그래프에서 비율(Proportion)과 같이 복잡한 양을 판단할 때, 스티븐스의 법칙에 기인하여 과대/과소평가가 반복되는 순환적 편향(Cyclical bias) 패턴이 발생한다[^30]. 이때 그래프에 중간 참조 지점인 눈금을 명확히 추가하면, 관찰자가 이를 기준 삼아 그래프를 여러 구성 요소로 세분화하여 분석하게 된다. 그 결과 편향의 주파수(Frequency)는 증가하지만, 시각적 판단의 전체적인 오류(Error) 폭은 대폭 감소하는 긍정적인 보정 효과를 얻을 수 있다[^31].

결론적으로, 스티븐스의 법칙을 통해 도출할 수 있는 상대적 판단의 편향 완화 전략은, 왜곡을 유발하는 부피나 면적 그래픽을 지양하고 눈금 등의 기준점을 제공하여 인지적 판단을 돕는 것으로 요약할 수 있다[^32].

[^23]: "Stevens (1957, 1975) found that the relation between physical and perceived magnitude can be expressed by the power function called Stevens’ law, with the exponent representing the amount of response compression or expansion."

[^24]: "avoiding continua whose Stevens exponents differ from 1.0"

[^25]: "Some continua, like area and volume, produce response compression: each unit increase in physical magnitude causes less and less increase in perceived magnitude."

[^26]: "Estimates of the areas and volumes shown in graphs are thus subject to response compression so that large areas and particularly volumes will tend to be underestimated."

[^27]: "Other stimuli, such as color saturation, tend to show response expansion: each increase in physical magnitude causes incrementally greater increases in perceived magnitude."

[^28]: "In general, the use of areas, volumes, color saturation, and other perceptual continua whose Stevens’ exponent differ from unity should be avoided in graphs."

[^29]: "making reference points available (e.g., adding tick marks)."

[^30]: "Moreover, the bias described by Stevens’ law affects more complex judgments where multiple quantities are involved, such as judgments of proportion... people tend to show cyclical bias patterns"

[^31]: "When tick marks are added to the graph... the bias frequency doubles, reducing error. Intermediate reference points (the tick marks) are used by observers to subdivide the graph into components, which has the beneficial side effect that error is reduced"

[^32]: "In summary, bias in making relative judgments with graphs can be reduced by: 1) avoiding continua whose Stevens exponents differ from 1.0; and/or 2) making reference points available (e.g., adding tick marks)."

## 데이터-잉크 비율을 높이면서 창발 자질을 유지하는 방법은?

데이터-잉크 비율(Data-ink ratio)을 극대화하려는 시도는 불필요한 시각적 장식을 제거하여 시각적 혼란(Clutter)을 줄이지만, 때로는 그래프 전체의 의미를 즉각적으로 전달하는 창발 자질(Emergent feature)을 훼손할 위험이 있습니다. 이 두 가지 원칙을 조화롭게 유지하고 인지적 효율성을 극대화하기 위해서는 다음과 같은 설계 방법론이 요구됩니다.

첫째, **극단적인 비데이터 잉크(Non-data ink) 삭제를 지양해야 합니다**. 데이터-잉크 비율 원칙을 지나치게 엄격하게 적용하여, 선 그래프에서 데이터 포인트를 연결하는 선을 비데이터 잉크로 간주해 모두 지워버리는 것은 매우 위험한 설계입니다. 비록 점 자체가 데이터를 완벽히 표상하더라도, 점들을 잇는 **'선의 기울기(Slope)'는 데이터의 변화율이나 추세를 직관적으로 보여주는 강력한 창발 자질로 기능**하여 사용자의 정보 해석을 결정적으로 돕기 때문입니다. 

둘째, **그래프의 본질적 내용과 개념적으로 연결된 비데이터 잉크를 제한적이고 신중하게 활용해야 합니다**. 모든 비데이터 잉크가 해로운 것은 아닙니다. графи적인 비데이터 이미지가 그래프가 전달하고자 하는 핵심 내용과 유기적으로 연결되어 있다면, 이를 적절히 허용하는 것이 그래프를 시각적으로 더 돋보이게 하고 독자의 뇌리에 오래 기억되도록 만드는 긍정적 효과를 창출할 수 있습니다. 즉, 단순한 장식용 잉크(예: 무의미한 3D 효과나 배경 그림)는 철저히 제거하되, 인지와 기억을 보조하는 구조적 형태는 의도적으로 보존하는 타협이 필요합니다.

셋째, **축(Axis)의 전략적 배치를 통해 데이터 자체가 자연스럽게 창발 자질을 형성하도록 유도해야 합니다**. 다중 변수를 그래프로 구성할 때, 정량적(Quantitative) 변수를 반드시 x축에 배치하는 구조를 설계해야 합니다. 이렇게 하면 x축을 따라 전개되는 데이터 지점 간의 차이가 자연스럽게 선으로 연결되며, **결과적으로 선의 기울기 및 두 선 사이의 각도라는 창발 자질을 통해 변수의 효과가 가장 직접적이고 직관적으로 표상**될 수 있습니다.

결론적으로, 데이터-잉크 비율을 높이면서 창발 자질을 유지하는 핵심은 **무분별한 잉크 제거가 아니라, 시각적 주의를 분산시키는 노이즈만을 선별적으로 제거하면서 정보의 전체적 추세를 보여주는 구조적 뼈대(기울기 등)를 보존하는 '선택적 최적화'**에 있습니다.



## 스티븐스의 법칙이 그래프 설계에 주는 실질적 팁은?

스티븐스의 법칙(Stevens' Law)은 그래프 설계에 있어 인간의 지각적 편향(Bias)을 최소화하기 위한 두 가지 핵심적인 실질적 지침을 제공한다. 이 법칙은 물리적 크기와 인간이 지각하는 크기 사이의 관계가 거듭제곱 함수(Power function)로 표현되며, 그 지수(Exponent)에 따라 반응 압축(Response compression) 또는 반응 팽창(Response expansion)이 발생함을 설명한다[^57]. 이로 인해 발생하는 정보 왜곡을 막기 위한 실질적 팁은 다음과 같다.

첫째, **스티븐스의 지수가 1.0과 다른 지각적 연속체의 사용을 배제해야 한다**[^58]. 면적이나 부피와 같은 시각적 차원은 지수가 1.0보다 작아, 물리적 크기가 커질수록 지각된 크기의 증가폭이 점점 줄어드는 반응 압축을 유발한다[^59]. 따라서 그래프에서 거대한 면적이나 3D 부피를 사용하여 양을 표현하면 독자는 실제 데이터보다 이를 심하게 과소평가하게 된다[^60]. 반대로 색상의 채도(Color saturation)는 반응 팽창을 일으켜 실제 값을 과대평가하게 만든다[^61]. 결과적으로 그래프 설계자는 지각적 오류를 방지하기 위해 지수가 1.0에서 벗어나는 면적, 부피, 채도 등의 사용을 피하고, 왜곡이 적은 '정렬된 길이'와 같은 차원을 우선적으로 선택해야 한다[^62].

둘째, **눈금(Tick marks)과 같은 중간 참조 지점을 명확히 제공해야 한다**[^63]. 원형 차트나 누적 막대그래프에서 비율(Proportion)과 같이 복잡한 양을 판단할 때, 스티븐스의 법칙에 기인하여 과대/과소평가가 반복되는 순환적 편향(Cyclical bias) 패턴이 발생한다[^64]. 이때 그래프에 중간 참조 지점인 눈금을 명확히 추가하면, 관찰자가 이를 기준 삼아 그래프를 여러 구성 요소로 세분화하여 분석하게 된다. 그 결과 편향의 주파수(Frequency)는 증가하지만, 시각적 판단의 전체적인 오류(Error) 폭은 대폭 감소하는 긍정적인 보정 효과를 얻을 수 있다[^65].

결론적으로, 스티븐스의 법칙을 통해 도출할 수 있는 상대적 판단의 편향 완화 전략은, 왜곡을 유발하는 부피나 면적 그래픽을 지양하고 눈금 등의 기준점을 제공하여 인지적 판단을 돕는 것으로 요약할 수 있다[^66].

[^57]: "Stevens (1957, 1975) found that the relation between physical and perceived magnitude can be expressed by the power function called Stevens’ law, with the exponent representing the amount of response compression or expansion."

[^58]: "avoiding continua whose Stevens exponents differ from 1.0"

[^59]: "Some continua, like area and volume, produce response compression: each unit increase in physical magnitude causes less and less increase in perceived magnitude."

[^60]: "Estimates of the areas and volumes shown in graphs are thus subject to response compression so that large areas and particularly volumes will tend to be underestimated."

[^61]: "Other stimuli, such as color saturation, tend to show response expansion: each increase in physical magnitude causes incrementally greater increases in perceived magnitude."

[^62]: "In general, the use of areas, volumes, color saturation, and other perceptual continua whose Stevens’ exponent differ from unity should be avoided in graphs."

[^63]: "making reference points available (e.g., adding tick marks)."

[^64]: "Moreover, the bias described by Stevens’ law affects more complex judgments where multiple quantities are involved, such as judgments of proportion... people tend to show cyclical bias patterns"

[^65]: "When tick marks are added to the graph... the bias frequency doubles, reducing error. Intermediate reference points (the tick marks) are used by observers to subdivide the graph into components, which has the beneficial side effect that error is reduced"

[^66]: "In summary, bias in making relative judgments with graphs can be reduced by: 1) avoiding continua whose Stevens exponents differ from 1.0; and/or 2) making reference points available (e.g., adding tick marks)."



## PPR과 PMP가 충돌할 때 해결하는 하이브리드 설계가 뭔가?

PPR(그림 사실주의 원리)과 PMP(이동 부품의 원리)가 충돌할 때 이를 해결하기 위해 고안된 대표적인 하이브리드 설계는 **'주파수 분리 디스플레이(Frequency-Separated Display)'**이다[^67]. 

이 설계는 조작에 따른 시스템의 시각적 변화를 시간 주파수(단기적 빠른 변화 vs 장기적 느린 변화)에 따라 분리하여 두 원리를 상황에 맞게 모두 충족시키는 혁신적인 방식이다. 구체적인 작동 원리와 적용 사례는 다음과 같다.

**1. 주파수 분리 디스플레이의 작동 메커니즘**
*   **고주파(단기) 영역 - PMP 적용:** 조작자의 즉각적이고 빠른 제어 입력(고주파 변화)이 발생할 때, 화면의 지시기(바늘이나 비행기 기호 등)는 조작자가 의도한 멘탈 모델의 이동 방향과 똑같이 즉시 움직여 **PMP 원리를 확실히 충족**시킨다[^68]. 
*   **저주파(장기) 영역 - PPR 적용:** 초기 조작 이후의 안정된 정상 상태(Steady state)나 느리게 원상태로 돌아가는 저주파 영역에서는, 움직였던 지시기가 천천히 중앙으로 돌아오고 대신 배경 눈금이나 지평선이 회전 및 이동한다. 이를 통해 실제 창밖으로 보이는 물리적 시야 및 형태와 방향을 일치시키며 **장기적으로 PPR을 완벽히 수용**하게 된다[^69].

**2. 대표적인 적용 사례**
*   **고도계 (Altimeter):** 전체 눈금 중 제한된 창(Window) 부분만 보여주는 방식을 취한다. 고도가 변할 때 바늘이 창 안에서 위아래로 빠르게 움직여 직관적인 조작 방향(PMP)을 맞춘다. 바늘이 창의 끝에 도달하려 하면, 배경에 있는 전체 눈금 척도가 반대 방향으로 아주 천천히(저주파로) 스크롤된다. 결과적으로 바늘은 다시 중앙으로 돌아오고, 높은 고도는 계속 위쪽에 표시되도록 하여 공간적 사실성(PPR)을 유지한다[^70].
*   **항공기 자세 지시계 (Attitude Indicator):** 조종사가 조종간을 꺾어 비행기를 빠르게 기울일 때, 중앙의 비행기 기호가 즉각적으로 조작 방향을 따라 좌우로 기운다(PMP). 하지만 선회 동작이 지속되면 비행기 기호는 서서히 수평으로 되돌아오고, 대신 배경의 인공 지평선이 기울어진 상태로 회전 고정된다. 이는 조종사가 실제 밖을 내다보는 시야(기울어진 지평선)와 일치하므로 모순 없이 PPR을 달성하게 된다[^69]. 

결론적으로 주파수 분리 디스플레이는 **단기적인 조작 직관성(PMP)과 장기적인 상황 인식의 사실성(PPR)을 시간의 흐름에 따라 교차 적용**함으로써 두 원리 간의 치명적인 설계 모순을 해결한다.

***

[^67]: "자세 지시계의 극단적 모순을 극복하기 위해 Lintern, Roscoe, & Sivier (1990)가 제안한 궁극의 혁신적 하이브리드 형태가 바로 주파수 분리 디스플레이(Frequency-Separated Display; Figure 4.9c)이다"

[^68]: "조종사가 조종간(에일러론)을 빠르게 꺾을 때 초기 고주파(High frequency) 단계에서는 중앙의 항공기 기호가 조작 방향과 똑같이 좌우로 움직여 PMP 원리를 확실히 충족시킨다"

[^69]: "선회가 지속되는 정상 상태(Steady state)나 느린 롤백 복귀 단계인 저주파(Low frequency) 영역으로 넘어가면, 비행기 기호는 천천히 원래 수평 위치로 돌아가고 배경의 지평선이 새롭게 기울어진 상태로 회전 고정되어 창밖의 실제 시야와 정확히 일치하는 형태를 회복하며 PPR을 완벽히 수용한다"

[^70]: "제한된 부분의 눈금만 보이는 창(Window)을 두고 그 안에서 바늘이 위아래로 빠르게 움직이게 하여 고주파(High frequency) 변화에 대응해 PMP를 만족시킨다. 동시에, 바늘이 창의 끝에 도달하려 할 때 배경 눈금 전체가 반대 방향으로 아주 천천히(저주파로) 이동하여 바늘을 중앙으로 되돌리면서 지속적으로 넓은 척도를 표시함으로써 장기적으로 PPR을 충족시킨다"


## 간접 지각 시스템이 직접 지각보다 주의력을 더 많이 소모하는 이유는?

간접 지각 시스템(Indirect perception system)이 직접 지각 시스템(Direct perception system)보다 주의력을 더 많이 소모하는 근본적인 이유는, 두 시스템이 3차원 공간을 지각하기 위해 사용하는 정보 처리의 메커니즘과 인지적 추론(Cognitive inference)의 의존도가 질적으로 다르기 때문이다[^71]. 

구체적으로 간접 지각 시스템이 주의 자원을 더 많이 요구하는 이유는 다음과 같은 핵심적 차이에서 비롯된다.

첫째, **고차원적 인지 추론과 하향식 처리(Top-down processing)의 차이**이다. 간접 지각 시스템은 관찰자로부터 비교적 멀리 떨어져 있는 대상들의 깊이나 거리를 명시적이고 의도적으로 판단할 때 주로 사용된다[^72]. 이 과정에서 뇌는 망막에 맺힌 불완전한 단서들을 해석하기 위해 과거의 경험, 지식, 기대치에 기반한 고차원적인 인지 추론(Higher-level cognition)에 크게 의존해야만 한다[^73]. 즉, 대상을 식별하고 거리를 가늠하기 위해 하향식 처리(Top-down processing)와 기대치에 큰 인지적 부담을 지우게 되며, 뇌가 단서들을 능동적으로 통합하고 계산해야 하므로 필연적으로 더 많은 주의력이 소모된다[^74].

둘째, **지각 과정의 자동화 수준 차이**이다. 반면 직접 지각 시스템은 관찰자가 3차원 공간을 이동하는 자아 운동(Egomotion)을 통제하고 가까운 표면을 지각하기 위해 진화된 시스템으로, 인지적 계산 없이 시각적 이미지의 역동적인 기하학적 구조(예: 광학 흐름 등)를 환경으로부터 직접 수용한다[^75]. 따라서 고차원적인 인지적 추론이 거의 필요하지 않아 그 작동이 무의식적이고 다소 자동적(Relatively automatic)으로 이루어진다[^76]. 

셋째, **해부학적 시각 경로와 시야 사용의 차이**이다. 간접 지각 시스템은 주의력이 집중되는 중심시(Focal/Foveal vision)를 활용하여 대상을 식별하는 데 특화된 뇌의 복측 경로(Ventral visual pathways)를 거친다[^77]. 중심시를 통해 특정 대상을 초점화하고 식별하는 작업은 본질적으로 의식적인 자원을 요구한다. 이와 대조적으로 직접 지각 시스템은 시야 전체에 분포한 주변시(Ambient/Peripheral vision)를 통해 빛의 정보를 받아들이고 배측 경로(Dorsal visual pathways)를 거쳐 자동적인 운동 통제에 기여한다[^78].

결론적으로, 직접 지각 시스템은 환경의 기하학적 특성을 자동으로 수용하여 무의식적으로 처리하는 반면, 간접 지각 시스템은 중심시를 통해 획득한 단서들에 인지적 추론과 하향식 처리를 더해 깊이와 거리를 명시적으로 '판단'해야 하므로 더 큰 주의 자원(Attentional resources)을 소모하게 된다[^79].

[^71]: "Psychologists have reached broad consensus that there are two qualitatively different systems for perceiving 3D space (DeLucia, 2008)."
 
[^72]: "This system is useful for more explicit, deliberate judgments of depth and distance of objects, including those objects that are relatively far away from the observer."
 
[^73]: "In contrast, a system for indirect perception is much more dependent on inference and higher-level cognition."
 
[^74]: "Because of the use of higher-level cognition, indirect 3D perception imposes a burden on top-down processing and expectancies, in order to make depth and distance inferences."
 
[^75]: "We describe first a system for direct perception, which functions somewhat automatically and is designed for perceiving nearby objects and surfaces as we move through the 3D world, a process called egomotion."
 
[^76]: "Its operation in egomotion does not depend heavily upon higher cognitive inference, and so its properties are well represented by the dynamic geometry of the visual image."
 
[^77]: "It makes use of focal (usually foveal) vision, using ventral visual pathways, as opposed to ambient (or peripheral) vision"
 
[^78]: "It is sometimes said to characterize ambient vision... It employs dorsal visual pathways leading to the cortex."
 
[^79]: "This stands in contrast to the relatively automatic processing used for direct perception. Thus, indirect perception places greater demand on attentional resources (see Chapter 10) than direct perception."



## 3D 디스플레이에서 발생하는 '시선 모호성(LOS ambiguity)' 문제의 해결 방안은?


3D 디스플레이에서 발생하는 **시선 모호성(Line of Sight ambiguity, LOS ambiguity)**은 3차원 공간의 깊이 축이 2D 화면으로 압축되면서, 서로 다른 깊이 상에 위치한 객체들이 관찰자의 시야에서는 동일한 상대적 위치를 가진 것처럼 투영되어 정확한 거리나 위치를 판별할 수 없는 치명적인 인지 오류 현상이다. 제공된 출처에서는 이러한 시선 모호성 문제를 해결하고 3D 디스플레이의 정확도를 높이기 위해 다음과 같은 구체적이고 실질적인 해결 방안들을 제시하고 있다.

첫째, **가중 선형 단서 모델(WLCM)에 기반한 다중 깊이 단서(Depth cues)의 극대화**이다. 시선 모호성의 근본적인 해결의 실마리는 이미지 내에 가능한 한 많은 깊이 단서를 융합하여 제공하는 것이다. 특히 인간의 깊이 지각에서 가장 지배적이고 강력한 가중치를 갖는 **교차(Occlusion), 입체시(Stereopsis), 그리고 운동 시차(Motion parallax) 단서를 최우선으로 설계에 포함**해야 한다. 예를 들어, 운동 시차를 제공하기 위해 관찰자가 디스플레이 내의 3D 공간 전체를 마치 투명한 장난감 집을 다루듯 자유롭게 좌우로 흔들거나(rock) 기울일(tilt) 수 있도록 인터랙션을 허용하면 깊이에 대한 모호성이 크게 줄어든다.

둘째, **평면성 단서(Flatness cues)의 적극적인 억제 및 제거**이다. 아무리 3D 렌더링이 훌륭해도, 모니터의 테두리 프레임이나 화면 표면에서 발생하는 빛 반사는 관찰자의 뇌에 "이것은 2D 평면이다"라는 강력한 증거를 제공하여 깊이감을 망치고 모호성을 가중시킨다. 따라서 시선 모호성을 해소하려면 **주변의 조명을 어둡게 하여 화면의 빛 반사를 없애고, 디스플레이 프레임이 시야에 덜 띄게 물리적 환경을 통제**해야 한다. 궁극적으로는 화면 테두리라는 개념 자체가 사라지는 **몰입형 가상현실(VR) 기술을 활용**하는 것이 이러한 평면성 단서를 원천 차단하는 매우 효과적인 대안이 된다.

셋째, **인공적인 참조 프레임워크(Artificial frameworks)의 추가**이다. 3D 공간 상에 떠 있는 객체들의 위치 모호성을 시각적으로 고정해주기 위해 데이터나 객체 주변에 인공적인 기준선이나 척도를 그려 넣는 방식이다. 3D 그래프의 경우, 막대에 눈금(Tick marks)을 명확하게 추가하여 관찰자가 크기나 연장 정도를 정확히 비교할 수 있도록 도와야 한다. 특히 항공 관제 디스플레이처럼 객체의 위치를 정밀하게 파악해야 하는 상황에서는, 지표면 역할을 하는 바닥에 **격자 무늬(Gridlines)를 그리고, 각 항공기 기호 아래에서 바닥으로 이어지는 수직 '기둥(Posts)'을 세워주는 것이 매우 효과적**이다. 이를 통해 가로, 세로, 수직이라는 3D 직교 축 상에서 각 객체가 정확히 어디에 위치해 있는지 그 공간적 좌표를 직관적으로 식별할 수 있다.

넷째, **정밀한 과제 분석(Task analysis)에 따른 대안적 디스플레이와의 교차 활용**이다. 3D 디스플레이는 전반적인 지형의 형태 파악이나 '전역 상황 인식(Global situation awareness)'과 같이 정보의 총체적 통합이 필요한 과제에는 의심의 여지 없이 우수하다. 그러나, 사용자가 특정 단일 축(예: 고도 분리 타당성)에 대해 매우 정밀하고 한 치의 오차도 없는 판단을 내려야 하는 경우라면 3D 디스플레이 자체의 한계로 인해 모호성이 발생할 수밖에 없다. 따라서 설계자는 사용자 과제의 성격을 명확히 분석하여, 정밀한 판단이 필요한 경우 앞서 언급한 인공적 프레임워크를 반드시 보강하거나 아예 X-Y 평면도와 Z-Y 정면도를 명확히 나누어 보여주는 **평면 분할(Co-planar) 디스플레이의 사용을 적극적으로 도입**하는 유연한 접근이 필요하다.


## 에지 율(Edge rate)을 활용한 교통사고 방지 사례

시뮬레이터 
https://gemini.google.com/share/162ac9fad512

![image](https://i.ibb.co/39PjN73b/image.png)
<span class="fig-caption">[그림 25] edge Rate 시각 시뮬레이터</span>



에지 율(Edge rate)은 **관찰자의 시야를 가로지르는 불연속점이나 모서리(경계선)가 단위 시간당 통과하는 횟수**를 의미한다[^1]. 시야를 지나는 에지 율이 증가할수록(즉, 바닥이나 주변의 결이 더 조밀해질수록) 이동자는 자신이 더 빠른 속도로 이동하고 있다고 지각하게 된다[^2]. 전반적인 광학 흐름(Global optical flow)과 에지 율은 보통 상관관계를 가지지만, 비행 중 듬성듬성한 나무 지대에서 빽빽한 숲으로 바뀌는 것처럼 환경의 텍스처 밀도에 체계적인 변화가 생기면 광학 흐름 자체는 변하지 않더라도 에지 율은 크게 변동하게 된다[^3].

이러한 에지 율의 시각적 불변량 특성을 실제 교통사고 방지에 극적으로 활용한 대표적인 사례가 바로 Denton(1980)의 영국 스코틀랜드 회전 교차로(라운드어바웃) 안전 설계이다.

**Denton(1980)의 스코틀랜드 교차로 감속 유도 마커 설계**
당시 영국의 도로에서는 자동차 운전자들이 회전 교차로(Roundabout)에 진입할 때 속도를 충분히 줄이지 않고 과도하게 빠른 속도로 접근하여 치명적인 사고가 빈발하는 문제가 있었다[^4]. 
이 문제를 해결하기 위해 Denton은 운전자의 시각적 지각 편향을 역이용하는 도로 설계를 고안했다. 교차로 진입로에 가까워질수록 도로 노면에 칠해진 횡단 마커들의 간격을 점진적이고 연속적으로 줄어들게(좁아지게) 배치한 것이다[^5].

- 이 설계가 작동하는 인지적 메커니즘과 그 결과는 다음과 같다.
   1. **지각적 착각 유도 (가속 오인):** 운전자가 교차로에 접근하며 적절하게 속도를 줄이지 않은 채 일정 속도를 유지하거나 덜 감속하게 되면, 노면 마커의 간격이 좁아짐에 따라 시야를 통과하는 선의 개수, 즉 '에지 율'은 오히려 급격하게 증가하는 현상을 경험하게 된다[^6].
   2. **보상적 감속 행동 (브레이크 조작):** 인간의 무의식적인 직접 지각 시스템은 증가하는 에지 율을 차량이 '가속'하고 있는 것으로 오인하게 만든다[^7]. 자신이 생각한 것보다 차량이 빨라진다고 착각한 운전자는 이 속도감을 상쇄(보상)하기 위해 본능적으로 브레이크를 밟아 더 강한 감속을 수행하게 된다[^7].
    3. **실제 사고 감소 효과:** 이 기발한 해결책은 스코틀랜드의 특히 위험했던 교차로 진입로에 실제로 도입되었다[^8]. 그 결과, 마커가 도입된 이후 운전자들의 평균 교차로 접근 속도가 물리적으로 현저히 느려졌을 뿐만 아니라, 가장 중요하게는 치명적인 사망 사고의 발생률(rate of fatal accidents) 또한 감소하는 실질적인 사고 방지 효과를 거두었다[^8]. 

(제공된 출처의 범위 내에서 에지 율을 교통사고 예방에 직접적으로 활용한 사례는 위 Denton(1980)의 연구가 핵심적으로 다루어지고 있다.)

[^1]: "Edge rate can be defined as the number of edges or discontinuities that pass across the observer’s visual field per unit time."

[^2]: "As edge rate increases (texture is finer), the traveler perceives a faster velocity."

[^3]: "Global optical flow and edge rate are typically correlated, but edge rate is affected if systematic changes in texture density occur (e.g., if flying and sparse trees change to dense forest), whereas global optical flow is not."

[^4]: "The edge rate cue was exploited by Denton (1980), who was concerned with automobile drivers in Great Britain who approached traffic circles (roundabouts) at an excessive rate of speed."

[^5]: "His solution was to decrease the spacing between road markers gradually and continuously as the distance to the roundabout decreased."

[^6]: "A driver not slowing down appropriately would see the edge rate as increasing."

[^7]: "Believing the vehicle to be accelerating, the driver would compensate by imposing a more appropriate degree of braking or slowing."

[^8]: "Denton’s solution was imposed on the approach to a particularly dangerous roundabout in Scotland. Not only was the average approach speed slower following introduction of the markers, but the rate of fatal accidents was also reduced."**텍스트**
