# CH1. 자료구조(DataStructure), 알고리즘(Algorithm)
* **자료**: **저장공간(Memory)** 필요, **연산(읽기, 쓰기, 삽입, 삭제, 탐색(검색))** -> ::**구조**::
* **알고리즘**: 자료구조 속 데이터를 가공 및 연산하여 원하는 값을 출력하는 방법
- - - -
## 자료구조 예시
### 변수(Variable)
* 자료와 1:1
* 변수에 객체 자체를 저장하는 것이 아니라, 객체의 **주소**를 저장
* 쓰기, 읽기 등

### 배열(Array)
* 복수의 객체를 원소로 하며 순서대로(idx) 구성
* 각 원소의 idx로 접근 -> A[idx]
* 읽기, 쓰기, 삽입(append, insert), 삭제(pop, remove) 등
- - - -
## 알고리즘
**인류 최초의 알고리즘**: 최대공약수(GCD)
* 두 수가 있을 때, 큰 수에서 작은 수를 빼는 행동을 반복하여 한 쪽이 0이 되었을 때, 0이 아닌 남은 수가 GCD이다.
-> **파이썬**으로?

::1번 알고리즘:: 반복 뺄셈으로 GCD return
```
def gcd_sub(a,b):
	while a!=0 and b!=0: # 한 쪽이 0이 될 때까지 큰 수에서 작은 수를 빼는 반복 뺄셈
		if a>b: a=a-b 
		else: b=b-a
	return a+b
```

::2번 알고리즘:: 반복 뺄셈으로 0이 되었다 == 반복하여 나누어 나머지가 0이 된다
```
def gcd_mod(a,b):
	while a!=0 and b!=0:
		if a>b: a=a%b 
		else: b=b%a
	return a+b
```

::3번 알고리즘:: 재귀함수
```
def gcd_rec(a,b):
	if a!=0 and b!=0:
		if a>b: return gcd_rec(a%b,b)
		else: return gcd_rec(a,b%a)
	else: return a+b
```



