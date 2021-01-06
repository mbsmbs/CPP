# Input Stream  std::cin
- C하고는 달리 모든 입력이 스트림으로 들어온다.
```c
std::cin >> something;
```
std::cin >> variable_name;

## C 스타일 문자열 안전하게 읽기
- Manipulator를 이용한다
```c
cin >> setw(4) >> myName;
```

## 스트림 상태
- namespace : ios_base
- 비트 플래그:
  - goodbit
  - eofbit
  - failbit
  - badbit
- 메소드 버전:
  - good()
  - eof()
  - fail()
  - bad()
