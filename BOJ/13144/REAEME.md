## 문제
[13144번](https://www.acmicpc.net/problem/13144)

## 풀이
투 포인터로 해결한 문제이다. 문제가 굉장히 짧고 간단하기에 이중 반복문 등을 사용하면 간단하게 '답'을 낼 수는 있지만 코드를 작성하기 전에 항상 입력의 범위를 신경써야 한다. N이 100,000 이하이기에 O(N^2)의 시간복잡도를 가진 코드일 경우 문제를 해결할 수 없을 가능성이 높다. 따라서 O(N) or O(NlogN) 이하의 시간복잡도를 가진 풀이를 시도할 필요가 있다.

투 포인터를 통해 left pointer, right pointer 사이의 수를 수열로 생각하고 right pointer가 늘어나면 더 큰 수열, left pointer가 늘어나면 수열이 작아진다라고 생각한다. check(중복 체크)배열을 통해 r이 증가할 때 중복이 발생할 경우 해당 수열을 포함한 모든 경우의 수를 제거한다.

Ex)
수열 : 1 2 1 2 4
l = 0, r = 2 일 때 수열은 \[1,2,1]을 나타내며 이 수열을 포함할 수 있는 경우의 수는 \[1,2,1,2],\[1,2,1,2,4]이다. 이 두 가지 경우의 수를 제거하는 것이다.


