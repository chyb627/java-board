
### docker
```bash
# container up
$ make db-up

# container down
$ make db-down
```


### git
```bash
# git 저장소 초기화
$ git init

# git 추가
$ git add --all

# git commit
$ git commit -m "커밋 내용"
$ git commit -m "추가: first commit"

# git remote 설정
$ git remote add origin 주소
$ git remote add origin https://github.com/chyb627/java-board.git

# git push
$ git push -u origin main
```


### 인텔리제이 커맨드
```bash
# 왼쪽 프로젝트창 열기/닫기 (vscode의 command + b)
$ command + 1

# 한줄 복사  (vscode의 option + shift + ↓)
$ command + d
```

### DB Setting
```sql
show databases;

create database board;

create user 'yb'@'localhost' identified by 'javalocal123';

select `user` from `mysql`.`user`;

show grants for 'yb'@'localhost';

grant all on `board`.*to 'yb'@'localhost' with grant option;

# 운영상 많이 보게됨. 권한테이블을 실제로 DB가 다시 읽게끔 해준다.
flush privileges;
```