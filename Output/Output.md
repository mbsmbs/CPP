# Output Stream  std::cout
```c
std::cout << something << std::endl;
```
- endl : 줄바꿈

## 1. namespace
- Java의 패키지나 C#의 네임스페이스와 비슷
- 이름 충돌을 피하는 것
```c
using namespace std;    // std::cout -> cout
```

### ```#pragma once``` : 이렇게 하면 헤더가 한 번만 #include 됨

### '<<' 연산자
- C++은 연산자 오버로딩으로 연산자의 동작을 바꿀 수 있다

### 출력 형식 지정 ([manipulator](https://en.cppreference.com/w/cpp/io/manip))
- 조정자는 여러가지 형식으로 출력할 수 있다.
