## 문제
[15684번](https://www.acmicpc.net/problem/15684)

## 풀이
입력으로 주어지는 N,H의 값이 상당히 작으므로 백트래킹(완전 탐색)으로 풀 수 있는 문제이다. 그래프 문제처럼 보이지만 일반적으로 주어지는 그래프의 모양과는 조금 다르기에 어떻게 그래프를 구성하느냐에 따라 문제 난이도가 달라질 것 같았다. 처음 시도에는 평소와 같이 인접 리스트로 시도했는데 이 문제에서는 간선이 존재하는 지도 중요하지만 존재하지 않는지, 간선이 연속적으로 등장하는 지도 중요하기에 인접 리스트로는 처리하기 귀찮은 부분들이 있었다. 인접 행렬을 선호하진 않지만 이 문제에서 N,H가 상당히 작고 연속적인 간선 처리도 쉽기에 인접 행렬로 시도했을 때 상당히 간단히 해결할 수 있었다.

