## 문제
[2170번](https://www.acmicpc.net/problem/2170)

## 풀이
boolean 카운팅 배열을 사용해 선이 그어진 위치를 파악하고 총 길이를 구하는 풀이부터 생각이 났지만 주어진 입력의 범위가 -10억 ~ 10억이기에 배열의 인덱스로는 사용할 수 없고 또 N의 범위가 0~백만 이므로 O(N^2)이상의 풀이로는 어렵겠다라는 생각을 하면서 문제 풀이를 시도했다.

먼저 Sort 함수를 통해 주어진 입력들을 정렬한다. Sort 함수의 시간복잡도는 O(NlogN)이므로 충분히 가능하고 그 이후에 스위핑(O(N))을 통해 문제를 해결했다.
