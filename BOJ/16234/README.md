## 문제
[16234번](https://www.acmicpc.net/problem/16234)


## 풀이
BFS를 돌면서 연합을 찾는다.

|v|||
|---|---|---|---|
|1|1|1|2|
|1|1|2|2|
|3|2|2|2|
|3|4|4|4|
2차원 배열을 통해 연합을 기록하는데 같은 번호를 가진 국가끼리 연합이다.

연합인 국가는 총 인구수 / 연합 국가의 수 를 통해 인구를 이동(조정)한다.
변화가 없을 때까지 계속 반복한다.



