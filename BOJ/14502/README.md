## 문제
[14502번](https://www.acmicpc.net/problem/14502)

## 풀이

처음 문제를 해석할 때에는 정말 말도 안되는 수준의 문제일 수도 있겠구나라는 생각에 조금 두려웠다. 하지만 M,N의 범위가 8보다 작은 것을 보고 모든 3개의 벽설치를 탐색하는 **경우의 수가 많아야 8^6**임을 알고 단순 무식하게(brute force) 모든 3개의 벽설치 조합에 대해 DFS를 사용해 문제를 풀었다.

조금 아쉬운 점은 손이 가는 대로 풀다 보니 좀 더 가독성 있게 코드를 리팩터링할 수 있었던 부분이다. 초기에 바이러스의 위치, 안전 영역의 위치를 vector로 저장하고 시작했다면 훨씬 가독성 있는 코드가 되었을 것이다.