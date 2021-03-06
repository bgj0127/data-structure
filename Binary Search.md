# 이분 탐색 - Binary Search

n개의 수가 크기 순서대로 배열되어 있을 때 특정의 수 k 가 몇 번재 위치에 있는지 빠르게 찾는 방법. 탐색 범위를 절반씩 줄여나가며 찾아가는 탐색 방법이다. 

이분 탐색은 순차 탐색이 아니다.

### 특징

중앙 값을 찾는 값에 비교한다. 줄어든 범위에서 재귀적으로 해결한다.

### 알고리즘

배열의 중간에 있는 임의의 값을 선택하여 찾고자 하는 값 X와 비교한다. X가 중간 값보다 작으면 중간 값을 기준으로 좌측의 데이터들을 대상으로, X가 중간값보다 크면 배열의 우측을 대상으로 다시 탐색한다. 동일한 방법으로 다시 중간의 값을 임의로 선택하고 비교한다. 해당 값을 찾을 때까지 이 과정을 반복한다.

한번에 절반 씩 줄어들기 때문에 시간복잡도는 O(logN) 이다.