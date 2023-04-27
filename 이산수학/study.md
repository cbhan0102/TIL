[이산수학]
이산수학(Discrete mathematics)
이산적인 수학구조에 대해서 연구하는 학문.


Discrete mathematics is the study of mathematical structures that are fundamentally discrete rather than continuous.
[참고] http://en.wikipedia.org/wiki/Discrete_mathematics
2. 추상화(abstraction)
   문제와 관련된 핵심내용만 남기고 관련 없는 내용을 제거하여 문제를 단순화 시키는 과정.
   Abstraction is a process by which concepts are derived from the usage and classification of literal ("real" or "concrete") concepts, first principles (such as an axiom), or other methods.
   [참고] http://en.wikipedia.org/wiki/Abstraction
3. 알고리즘(algorithm)
   알고리즘 표현방법으로는 컴퓨터 프로그래밍 언어(computer programming language), 순서도 (flow chart), 의사코드 (pseudocode) 등의 방법이 있음.
   An algorithm is a set of instructions, sometimes called a procedure or a function, that is used to perform a certain task.
   [참고] http://en.wikipedia.org/wiki/Algorithm
4.
관계
두 집합 X와 Y가 존재하고 X에서 Y로의 관계 R이 있을 때, R은 이들의 곱집합 X×Y의 부분집합이다. 만약 x와 y가 각각 X와 Y의 원소이고 (x, y)∈R이면 xRy로 표기하며, x는 y와 R의 관계가 있다라고 한다. 두 집합 X와 Y가 X=Y를 만족하면 이들 사이의 관계 R을 X에서의 관계라고 한다.
[정의 6.1]
[참고] http://en.wikipedia.org/wiki/Relation_(mathematics)

관계의 성질(반사적, 대칭적, 추이적)
집합 A에 대한 관계 R이 있을 때,
(1) 모든 a∈A에 대해 aRa이면 반사적이라 한다.
(2) 모든 a,b∈A에 대해 aRb→bRa 가 성립하는산 경우 관계 R은 대칭적이라 한다.
(3) 모든 a,b,c∈A에 대해 (aRb∧bRc)→aRc가 성립하는 경우 관계 R은 추이적이라고 한다.
[정의 6.2]
[참고] http://en.wikipedia.org/wiki/Reflexive_relation
http://en.wikipedia.org/wiki/Symmetric_relation
http://en.wikipedia.org/wiki/Transitive_relation

역관계
집합 X에서 집합 Y로의 관계 R이 있을 때, 관계를 구성하는 각 순서쌍의 원소 순서를 바꾸면 Y에서 X로의 관계가 되며, 이를 역관계라고 한다. 기호로 R⁻¹이라 표기하며 다음과 같이 정의한다.
R⁻¹={(y,x)∣(x,y)∈R}
[정의 6.3]
[참고] http://en.wikipedia.org/wiki/Inverse_relation

합성관계
집합 A에서 집합 B로의 관계 R이 있고, 집합 B에서 집합 C로의 관계 S가 있을 때,
S ∙ R={(a,c)∈A×C ∣ a∈A,b∈B,c∈C,(a,b)∈R,(b,c)∈S}로 정의되는 A에서 C로의 관계를 합성관계라 한다.
[정의 6.4]
[참고] http://en.wikipedia.org/wiki/Composition_of_relations

동치관계
집합 A에 대한 관계 R이 있을 때, R이 반사적이고, 대칭적이고, 추이적이면 R은 동치관계이다.
[정의 6.5]
[참고] http://en.wikipedia.org/wiki/Equivalence_relation

동치류
집합 A에 대한 관계 R이 있을 때, A의 각 원소 a에 대하여 a의 동치류는 a와 R의 관계를 가지는 A의 원소들의 집합이며, [a]로 표기한다. 기호로 나타내면
[a]={x∈A∣xRa} 또는 [a]={x∈A∣aRx} 이다.
[정의 6.6]
[참고] http://en.wikipedia.org/wiki/Equivalence_class

명제(Discrete mathematics)
[정의2.1]
참과 거짓을 구별할 수 있는 문장이나 수학적 식
추가설명 - 합성명제, 조건명제, 쌍조건명제, 항진명제, 모순명제 등의 의미도 확인하기바람.
[참고] http://en.wikipedia.org/wiki/Discrete_mathematics

논리적 동치
어떤 주어진 문제를 수학적 표현(방정식)으로 변환하는 것이다.
[정의 2.7]
두 명제 𝒑 와 𝒒 가 논리적으로 동등하면 논리적 동치라고 하고, 𝒑≡𝒒 로 표시한다.
[참고] http://en.wikipedia.org/wiki/Abstraction

명제함수(propositional function)
[정의 2.9]
변수의 값에 의해 함수의 진리값이 결정되는 문장이나 식
[참고] http://en.wikipedia.org/wiki/Algorithm

추론(inference)
[정의 2.12]
참으로 알려진 명제를 기초로 하여 다른 명제를 유도해 내는 과정을 추론이라고 한다.

그래프
그래프는 꼭지점(vertex)의 집합과 변(edge)의 집합으로 정의된다. 꼭지점 집합 V와 변의 집합 E를 가지는 그래프 G는 G=(V, E)와 같이 표현한다. 변은 두 꼭지점을 연결하는 역할을 수행하는데, 만일 변 e가 꼭지점 v와 w를 연결하는 경우 v와 w는 e에 의해 발생(incident)되었다고 하고, 연결된 두 꼭지점 v와 w는 서로 인접(adjacent)한다고 한다. 동일한 꼭지점을 연결하는 변은 특별히 루프(loop)라 한다. 동일한 두 꼭지점을 연결하는 변이 두 개 이상 있을 대 이러한 변들을 병렬(parallel) 변이라 한다. 어떠한 변도 연결되지 않은 꼭지점은 고립(isolated)되었다고 한다.
[정의 9.1]
[참고] http://en.wikipedia.org/wiki/Graph_(mathematics)

방향 그래프
그래프의 변이 방향을 가지고 있으면 방향 그래프(directed graph)라 하고, 변이 방향을 가지지 않는 그래프를 무향 그래프(undirected graph)라 한다.
[정의 9.2]
[참고] http://en.wikipedia.org/wiki/Graph_(mathematics)

단순 그래프
꼭지점의 집합 V와 변의 집합 E로 이루어진 단순 그래프 G=(V, E) 는 두 개의 꼭지점 사이에 최대 하나의 변을 가지는 무향 그래프이다. 다시 말하면, 어떤 루프나 어떠한 병렬 변을 가지지 않는 그래프이다.
[정의 9.3]
[참고] http://en.wikipedia.org/wiki/Graph_(mathematics)

부분 그래프
그래프 H와 그래프 G가 있을 때, H의 모든 꼭지점이 G의 꼭지점이고, H의 모든 변이 G의 변일 경우 H를 G의 부분 그래프라고 한다. 만약, H의 꼭지점과 G의 꼭지점이 완전히 일치하면 H는 G의 신장 부분 그래프라 한다.
즉, H=(V, E)이고, G=(V’, E’)일 때,
(1) 부분그래프는 V’ ⊆ V 이고 E’ ⊆ E 인 그래프이고,
(2) 신장 부분 그래프는 V’ = V 이고 E’ ⊆ E 인 그래프이다.
[정의 9.4]
[참고] http://en.wikipedia.org/wiki/Spanning_subgraph#Subgraphs

그래프의 차수
그래프 G의 꼭지점 v에 대해 v에 인접한 변의 수를 v의 차수라 한다. 변이 루프일 경우 2를 더한다. G의 총 차수는 G에 있는 모든 꼭지점 차수의 합이다.
[정의 9.5]
[참고] http://en.wikipedia.org/wiki/Degree_(graph_theory)

워크, 트레일, 경로
[정의 9.6]
[참고] http://en.wikipedia.org/wiki/Path_(graph_theory)

연결 그래프
그래프에서 두 꼭지점을 서로 연결하는 경로가 있을 경우, 두 꼭지점은 서로 연결되어 있다고 한다. V의 꼭지점들은 서로 연결되고 다른 집합과 겹치지 않는 꼭지점의 집합 V₁, V₂ ..., Vₘ 로 나눌 수 있는데, 이들 각각을 연결 성분이라 한다. 그래프에 오직 하나의 연결된 요소만 있을 경우를 연결 그래프라고 한다.
[정의 9.8]
[참고]http://en.wikipedia.org/wiki/Connected_graph

완전 그래프
그래프에 속한 모든 꼭지점이 다른 꼭지점과 인접할 경우 완전 그래프라 하고, n개의 꼭지점을 가지는 완전 그래프는 Kₙ 으로 나타낸다.
[정의 9.9]
[참고] http://en.wikipedia.org/wiki/Complete_graph

이분 그래프
그래프 G=(V, E)의 V가 연결성분 V₁과 V₂로 분할되어 있고, 모든 변들이 V₁의 꼭지점과 V₂의 꼭지점을 연결할 경우 이분 그래프라고 한다.
[정의 9.10]
[참고] http://en.wikipedia.org/wiki/Bipartite_graph

정규 그래프
그래프 G=(V, E)의 모든 꼭지점들이 동일한 수의 이웃을 가질 경우, 정규 그래프라 한다. 즉, 정규 그래프의 모든 꼭지점들은 동일한 차수를 가지며, 각 꼭지점이 k의 차수를 가진다면 k-정규 그래프라고 한다. 0-정규 그래프는 변이 없는 그래프이고, 1-정규 그래프는 독립된 꼭지점으로 이루어진 그래프이며, 2정규 그래프는 사이클로 구성된 그래프이다. 3-정규 그래프는 큐빅 그래프라고도 부른다.
[정의 9.12]
[참고] http://en.wikipedia.org/wiki/Regular_graph

발생 행렬
그래프의 꼭지점을 행렬의 행으로 변을 행렬의 열로 하여, 꼭지점과 변의 연결관계를 표현한 것이 발생행렬이다. 변과 꼭지점 사이에 인접관계에 있을 경우 1의 원소를, 인접관계가 아닐 경우 0의 원소를 가진다. 그래프의 행의 꼭지점의 개수가 │V│개, 열의 개수가│E│개 있을 경우 │V│×│E│크기의 행렬이 만들어진다.
[정의 9.13]
[참고] http://en.wikipedia.org/wiki/Incidence_matrix

인접 행렬
그래프의 꼭지점을 행렬의 행과 열로 하여 꼭지점들 사이의 연결관계를 표현한 것이 인접행렬이다. 꼭지점 Vi,에서 Vj로의 연결개수가 행렬의 (i,j) 원소의 값이 되며, 그래프에서 행의 꼭지점의 개수가 │V│개일 경우, │V│×│V│크기의 행렬이 만들어진다. 무향 단순 그래프의 경우 인접행렬로 표현하면 모든 원소는 0 또는 1의 값을 가지게 되고, 대각원소는 0의 값을 가진다.
[정의 9.14]
[참고] http://en.wikipedia.org/wiki/Adjacency_matrix

인접 리스트
그래프 G=(V, E')의 각 꼭지점에 인접하는 꼭지점들을 차례로 연결 리스트로 표현한 것을 인접 리스트(adjacency list)라 한다.
[정의 9.15]
[참고] http://en.wikipedia.org/wiki/Adjacency_list

오토마타
스스로 움직이는 기계를 오토마타라고 말한다. 다른 말로는 자동 장치라고 말하며, 오토마타는 튜링머신, 컴퓨터(유한 상태 오토마타) 등이 있다.
[참고] http://en.wikipedia.org/wiki/Automata_theory

튜링머신
튜링 머신은 테이프, 헤드, 상태 기록부, 유한한 표로 이루어진 유한 상태 기계를 말하며, 역사상 가장 정교하고 실제로 구현된 오토마타이다.
[참고] http://en.wikipedia.org/wiki/Turing_machine

유한 오토마타
유한 오토마타 𝑴=(𝑰, 𝑶, 𝑸, 𝒇, 𝒈, 𝝈)는 다음 6개의 튜플로 구성된다.
(1) 𝑰 : 입력기호의 유한집합
(2) 𝑶 : 출력기호의 유한집합
(3) 𝑸 : 상태의 유한집합
(4) 𝒇 : 𝑸×𝑰→𝑸의 전이함수
(5) 𝒈 : 𝑸×𝑰→𝑶 의 출력함수
(6) 𝝈: 초기상태(𝝈 ∈𝑸)
[정의 14.1]
[참고] http://en.wikipedia.org/wiki/Finite_Automata
마르코프 연쇄
다음 조건을 만족하는 이산확률과정 (𝐗₀, 𝐗₁, ..., 𝐗ₙ,...)을 마르코프 연쇄라고 한다.
[정의 14.4]
[참고] https://en.wikipedia.org/wiki/Markov_chain
형식 언어
형식 언어는 재귀 열거 언어, 문맥 의존 언어, 문맥 자유 언어, 정규 언어가 있으며, 언어를 표현하는 것은 다음과 같다.
∑를 유한 알파벳이라고 하자. 양의 정수 n에 대하여
∑,ⁿ, ∑⁺, ∑＊는 다음과 같이 정의한다.
∑,ⁿ : 길이가 n인 ∑상의 모든 문자열의 집합
∑⁺ : 길이가 적어도 1이상의 ∑상의 모든 문자열의 집합
∑＊ : 길이가 0이상의 ∑상의 모든 문자열의 집합
∑＊의 임의의 부분집합을 언어라고 한다.
[정의 14.6]
[참고] http://en.wikipedia.org/wiki/Formal_language

형식 문법
다음과 같이 4개의 원소의 순서쌍으로 정의되는
𝑮=(𝑽, 𝑻, 𝑷, 𝑺)를 문법이라고 한다.
𝑽 : 비단말(nonterminal) 기호들의 유한집합
𝑻 : 단말(terminal) 기호들의 유한집합
𝑷 : 생성 규칙(production)
𝛂 → 𝛃, 𝛂, 𝛃∈(𝑽U𝑻)＊, 𝛂는 적어도 하나의 비단말 기호를 포함.
𝑺 : 𝑽에 속하는 변수로서 시작 기호
[정의 14.8]
[참고] http://en.wikipedia.org/wiki/Formal_grammar
