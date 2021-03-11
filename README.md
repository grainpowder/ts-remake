<a href=https://arxiv.org/abs/1707.02038>이 책</a>은 실시간 의사결정 시스템을 만드는 데 사용될 수 있는 머신러닝 기법인 Thompson sampling의 개념과 시뮬레이션 결과를 제시한다. 저자는 자신의 <a href=https://github.com/iosband/ts_tutorial>repository</a>를 통해 책에 담은 시뮬레이션 결과들을 재현할 수 있는 코드를 제공하는데, 그 코드들은 이 결과들을 재생성하는 데 초점이 맞춰져 있어서 책에서 설명하는 알고리즘을 이해하는 데 사용하기에는 불편한 점이 있다. 그래서 이 책의 개념들을 학습하는 동시에 알고리즘을 이해하기 편한 형식으로 저자의 코드를 리팩토링해서 정리했다.

## BernoulliBandit
Multi-Armed Bandit 문제를 간단히 설명하고, 책의 3장에 소개된 내용을 정리
- action에 대한 reward가 0 또는 1인 Multi-Armed Bandit(Bernoulli Bandit) 문제에서 실시간으로 의사결정을 내리는 알고리즘을 설명
- 책의 예시를 사용자들의 클릭 여부를 가지고 여러 선택지들 중 최적을 고르는 A/B 테스트 문제를 이 알고리즘을 통해 해결하는 내용으로 rephrase해서 예시에 대한 설명의 구체성을 더함

## ShortestPath(independent)
BernoulliBandit에서 설명한 내용들을 바탕으로 4장에서 본격적으로 소개되는 최단 경로 탐색 문제에 대한 정리. 리팩토링은 완결, 설명은 미완결