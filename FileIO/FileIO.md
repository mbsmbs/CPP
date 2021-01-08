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

### - 파일에서 문자 하나씩 읽기
- 
