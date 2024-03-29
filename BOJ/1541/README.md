## 문제
[1541번](https://www.acmicpc.net/problem/1541)

## 풀이

주어진 식의 최솟값을 구하는 문제이다. 문제에서 피연산자 앞의 연산자가 식의 계산에 영향을 주므로 문제를 푸는 과정에서 모든 연산자와 피연산자를 미리** 파싱하는 것이 필요**했다.


파싱하는 과정에서 기억할만한 점은 **피연산자의 길이 제한이 있기에  atoi(stoi)를 사용**할 수 있다는 것이다. 예를 들어 100000 ... 000009와 같은 굉장히 긴 길이의 피연산자가 등장할 수 있는 입력의 경우 atoi (stoi)를 사용하지 못한다.

이 문제를 풀 때 핵심은 **괄호를 내가 임의로 어디에서나 사용할 수 있다**는 점이다. 물론 실제로 넣지는 않았지만 그렇게 상상할 수 있었다는 것이다. 식에서 '-'기호가 한번 등장하는 경우 그곳부터 괄호를 시작해 뒤에 오는 모든 '+'기호를 묶는다면 모두 마이너스 연산을 할 수 있다. '-' 기호 뒤에 '-'기호가 또 등장한다면 그때는 괄호로 묶지 않고 각각 계산한다면 모두 마이너스 연산을 할 수 있다. 중요한 것은 '-'기호가 등장해야 이런 괄호를 통한 계산이 가능하기에 flag 변수를 통해 '-'기호가 앞에 등장한 적이 있는지 확인한다.

