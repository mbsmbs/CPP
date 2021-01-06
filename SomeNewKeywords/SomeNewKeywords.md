# 일부 새로운 C++기능

## bool 형
- 참, 거짓을 나타낸다.
```c++
bool varName;
```

## 참조형 (reference) : 23
- 포인터를 사용하는 좀 더 안전한 방법
- 별칭이다
- NULL이 될 수 없음
- 초기화때 반드시 선언
- 참조하는 대상을 바꿀 수 없음
```c++
int number = 100;
int& reference = number;
```
