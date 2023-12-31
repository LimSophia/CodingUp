✍ #`백트래킹_알고리즘` #`경우의_수`
## 백트래킹 알고리즘
#### 백트래킹과 DFS(Depth First Search) 깊이 우선 탐색의 차이
나는 처음에 백트래킹과 DFS이 모두 깊이 우선 탐색으로 차이가 없는데 이름이 2개나 있다고 생각했다. 그러나 이는 오산이었다..<br>
DFS는 완전 탐색 방법으로 모든곳을 탐색한다. 이에 반해 백트래킹은 가도되지 않는 루트를 고려하지 않고 탐색하는 완전 탐색 기법이다. 즉 두 방법 모두 깊이 탐색이지만 다른 차이점이 있다는 것이다. <br>
다음은 간단하게 정리한 표이다. <br>

<table>
  <th></th><th>DFS</th><th>백트래킹</th>
  <tr>
    <td>목적</td>
    <td>모두 탐색</td>
    <td>불필요한 경우 탐색 X</td>
  </tr>
  <tr>
    <td>적용 분야</td>
    <td>그래프 알고리즘에서 사용되며, 최단 경로 찾기, 사이클 검사, 연결 요소 찾기 등에 활용</td>
    <td>조합 최적화, 순열, 스도쿠, N-퀸 문제 등과 같이 다양한 조합 문제나 제약 충족 문제에서 적용</td>
  </tr>
  <tr>
    <td>방식</td>
    <td>재귀적인 방법이나 스택을 이용하여 깊이 방향으로 탐색</td>
    <td> DFS를 기반으로 하되, 문제의 조건을 만족하지 않으면 해당 경로를 더 이상 탐색하지 않고 이전 단계로 돌아가서 다른 가능성을 탐색</td>
  </tr>
  <tr>
    <td>가지치기</td>
    <td>모든 경로를 탐색</td>
    <td>가지치기를 통해 불필요한 경우에는 해당 분기를 탐색하지 않고 이전 단계로 돌아가는데 중점</td>
  </tr>
</table>

