## 문제
<https://www.acmicpc.net/problem/2342>

## 풀이
100,000번을 완전 탐색으로 풀 생각도 안했다. 바로 DP 메모이제이션으로 접근했고 state를 (수열 idx, 왼발 위치, 오른발 위치)로 설정하고 해결했다. 최소값을 구하는 것이므로 기존 DP를 최대값으로 설정하고 점점 최소값을 찾아가는 방식으로 해결한다.

