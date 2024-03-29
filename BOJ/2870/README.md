## 문제
[2870번](https://www.acmicpc.net/problem/2870)

## 풀이

성급하게 문제풀이를 시도하기보다 조건을 먼저 잘 들여다 봐야된다는 교훈을 준 문제이다. 이런 문제에서 자주 실수하는 점은 굉장히 길이가 긴 숫자가 등장할 수 있고 이로 인해 **atoi(stoi)를 사용하지 못한다**는 것이다. 따라서 string 형태로 숫자를 계속해서 담고 있어야하고 정렬할 때도 **custom sort를 통해 오름차순 정렬을 시도**해야한다.

풀이에서 기억할만한 점은 custom sort의 compare 함수를 만들 때 string 형끼리 a < b 와 같이 사용한다면 string.compare 처럼 사용할 수 있지만 정수형과 비교하는 연산이 다르기에 조심해야 한다는 것이다.

알파벳과 숫자를 파싱할 때도 flag 변수를 사용하는 등 굉장히 복잡하게 진행했는데 아스키 코드와 임시 string을 통해 훨씬 간단하게 할 수 있음을 배웠고 다음에 적용해보도록 하자.

