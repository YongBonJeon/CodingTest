### 문제
[19942번](https://www.acmicpc.net/problem/19942)

## 풀이
완전 탐색(백트래킹)으로 해결한 문제이다. N이 상대적으로 매우 작기에 모든 경우의 수를 탐색할 수 있다고 판단했고 탐색시에 최소 영양 성분을 만족한 경우 최소 비용을 최신화하고 vector를 통해 선택한 식재료들의 index를 저장했다. 모든 탐색이 끝나고 vector로 저장된 식재료들의 집합을 sort 함수를 통해 정렬함으로써 사전순으로 정렬하고 0번 index에 있는 식재료들의 index를 출력했다.
