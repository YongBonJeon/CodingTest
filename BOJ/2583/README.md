## 문제
[2583번](https://www.acmicpc.net/problem/2583)

## 풀이
기존에 풀었던 문제들과 같이 입력은 Map으로 주어지고 DFS, BFS를 통해 Connected Components를 찾는 문제이다. 다른 점은 탐색 횟수를 기억하여 영역의 넓이를 출력해야 한다는 점이다. 나는 전역변수를 통해 dfs  함수 호출 시에 1을 더하는 것으로 해결했다.

기억할만한 점은 void형 dfs와 전역변수로 풀이해도 되지만 리턴값을 가지는 **int형 dfs를 통해서도 풀이할 수 있다**는 점이다. 앞으로 많이 사용할 것이기에 잘 인지하고 사용법에 대해 기억해야한다.
