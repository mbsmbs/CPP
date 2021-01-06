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


## 입력 버리기 (discarding input)
### clear()
- 스트림을 good state로 돌려 줌
```c++
cin.clear();
```

### ignore()
- 파일 끝에 도달하거나 지정한 수만큼 문자를 버리면 멈춤
```c++
cin.ignore();           // 문자 1개를 버림
cin.ignore(10);         // 문자 10개를 버림
cin.ignore(10, '\n');   // 문자를 10개 버림. 단, 그 전에 뉴라인 문자가 있으면 버리고 멈춤 
```

## get()
- code : 19
- 뉴라인 문자를 만나기 직전까지의 모든 문자를 가져옴
- 뉴라인 문자는 입력 스트림에 남아 있음
```c++
get(firstName, 100);       // 99개의 문자를 가져오거나 뉴라인 문자가 나올 때까지의 문자를 가져오고 char배열(firstName)에 문자들을 배치함

get(firstName, 100, '#');  // 99개의 문자를 가져오거나 '#' 문자가 나올 때까지의 문자를 가져오고 char배열(firstName)에 문자들을 배치함
```

## getline()
- code : 19
- 뉴라인 문자를 만나기 직전까지의 모든 문자를 가져옴
- 뉴라인 문자는 입력 스트림에서 버림
```c++
getline(firstName, 100);
getline(firstName, 100, '#');
```
