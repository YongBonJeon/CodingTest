### 문제
<https://www.acmicpc.net/problem/1509>

## 풀이
[10942번](https://velog.io/@bon0057/CC-%EB%B0%B1%EC%A4%80-10942%EB%B2%88-%ED%8E%A0%EB%A6%B0%EB%93%9C%EB%A1%AC)문제처럼 다이내믹 프로그래밍 방법으로 부분적으로 팰린드롬을 확인할 수 있는 2차원 배열을 만든다. 그 후에 다이내믹 프로그래밍을 한번 더 사용하는 것이다. 두번째 메모이제이션 배열이 나타내는 것은 DP2\[N]은 N까지의 분할 개수의 최솟값이다.

