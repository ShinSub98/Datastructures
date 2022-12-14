# Day4. Big-O
## 알고리즘 수행시간의 비교
* 알고리즘의 수행시간 = 가장 긴 수행시간에 대한 연산 횟수(WTC)
-> 평균을 구하기에는 너무 힘들기 때문에
* T(n)으로 표현된 시간복잡도는 n에 관한 그래프로 표현할 수 있기 때문에, _그래프를 통해 알고리즘 간의 수행시간을 비교할 수 있다._
-> n이 제곱으로 표현된다면 _수행시간의 증가율은 n이 커질수록 증가한다_

## Big-O
* **Big-O**: 알고리즘의 수행시간을 함수의 _최고차항만으로 간단하게 표기_ (계수는 생략)
Ex1) T(n) = 2n-1일 경우, _T(n) = O(n)_
Ex2) T(n) = 3n^2 +1일 경우, T(n) = O(n^2)
Ex3) 상수 밖에 없는 알고리즘이라면 n^0=1이기 때문에 O(1)
Ex4) 2진수를 구하는 경우와 같이 n이 log로 표현되는 알고리즘이라면 O($$\log_a n$$)

**즉, O(n^x)는 x차식으로 이루어진 모든 알고리즘을 포함하는 집합**

#자료구조