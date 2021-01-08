# 파일 입출력 <fstream>
- ifstream  : 입력
- ofstream  : 출력
- fstream : 입력 + 출력
- Manipulator등도 쓸 수 있음

## 파일 열기
- 읽기 전용
```c++
ifstream fin;
fin.open("helloworld.txt");
```

- 쓰기 전용
```c++
ofstream fout;
fout.open("helloworld.txt");
```

- 읽기 + 쓰기
```c++
fstream fs;
fs.open("helloworld.txt");
```

### - open()
- 각 스트림마다 open()메서드가 있다.
- mode flags들이 있다. ios_base : 31
```c++
open("HelloWorld.txt", ios_base:: in | ios_base::binary);
```

### - close()
- 각 스트림마다 close() 메서드가 있음

### - is_open()
- 파일이 열려 있는지 확인

### - 파일에서 한 문자, 한 단어, 한 줄 읽기 : 32

### 파일 읽기 베스트 프랙티스
- 테스트:
1. 유효하나입력 뒤에 EOF
2. 유효한 입력과 뉴라인뒤에 EOF
3. 유효하지 않은 입력 뒤에 EOF
4. 유효하지 않은 입력 뒤에 EOF
5. 공백: 탭도 포함할 건가?
6. 키보드 입력과 입력 리다이렉션을 둘 다 확인할 것


### 파일에 쓰기, 바이너리 파일 읽기, 파일 안에서의 탐색 : 37
