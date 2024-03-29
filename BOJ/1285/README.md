### 문제
[1285번](https://www.acmicpc.net/problem/1285)

## 풀이
문제를 처음 보고 풀이를 시도했을 때 굉장히 막막했다. N이 20까지 가능하므로 완전 탐색(모든 행과 열을 탐색)을 통해 풀면 시간복잡도가 무려 2^40 이기에 이 문제는 그렇게는 절대 풀 수 없다는 것을 알았다. 혼자서 몇 시간을 고민해도 풀지 못해 구글링으로 힌트를 얻었다. 행(혹은 열)에 대해서 완전 탐색을 진행하고 열은 한 열마다 뒤집는가 마는가로 판단하여 최적해를 얻을 수 있다는 것이다. 이런 아이디어를 떠올렸을 때 문제 풀이 코드를 작성하는 것은 그렇게 어려운 일이 아니었다.

문제에서 얻어갈만한 점은 미리 시간복잡도를 적당히 파악하고 평범한 풀이로는 절대 해결할 수 없다는 것을 깨달았을 때 문제에 방향성을 새로 고민하고 새로운 풀이를 찾아내려 노력해야 한다는 것이다.


