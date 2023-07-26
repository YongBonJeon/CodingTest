## 문제
[20529번](https://www.acmicpc.net/problem/20529)

## 풀이
각 테스트케이스마다 주어지는 N의 범위가 100,000 이하이기 때문에 
그냥 감정적으로 문제를 해결하려고 보면 약 nH3(중복조합) 정도의 시간복잡도를 
가지기에 문제를 해결할 수 없음을 파악했다. 
시간복잡도를 최소화해야하는데 단순하게 보면 문제에서 주어지는 경우는 16가지의
MBTI 밖에 없으므로 16 사이즈의 배열을 통해 문제의 볼륨을 대폭 줄일 수 있었다. 
총 16가지 중에 3가지를 중복해서 뽑는 경우의 시간복잡도는 PS에서 부담없는 수준이다.

그 이후에는 단순하게 모든 경우의 수를 확인하여 최솟값을 구했는데 서칭해보니 조금 더 시간복잡도를 줄일 수 있는 방법으로 **비둘기집 원리**를 사용할 수 있었다.
16가지의 MBTI 경우에 32개 초과 입력이 들어온다면 반드시 3개가 중복이 되는 MBTI가 존재하고 이 경우에 최소 심리적 거리가 0임을 바로 파악할 수 있다. 