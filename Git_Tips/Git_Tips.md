# Git Tips
Windows 기준으로 설명하고 있습니다.

## Git Bash 터미널 계정 변경 방법
git push 과정에서 사용하고 있는 컴퓨터에서의 터미널 계정이 push할려는 계정과 달라서 에러가 나올 수 있다.  
이럴때는 아래의 과정을 확인해보고 다시 git push를 하면 push가 된다.  

### 1. 현재 설정된 계정 정보 확인
git bash를 열고 아래의 명령어를 입력하면 현재 지정되어 있는 계정이름, 이메일을 확인 할 수 있다.  
``` 
$ git config user.name
```
```
$ git config user.email
```

### 2. 명령어를 통해 계정 바꾸기
변경하고 싶은 계정으로 변경할 수 있다.  
```
$ git config --global user.name 변경 하고싶은 계정
```
```
$ git config --global user.email 변경 하고싶은 이메일
```
### 3. Windows 자격증명 수정하기
제어판 > 사용자 계정 > 자격 증명 관리 > Windows 자격 증명 > github항목 삭제 후 수정  
- 인터넷 또는 네트워크 주소를 지정하는 칸 : 깃허브의 주소  
```
https://api.github.com/변경할 계정 이름

```
- 사용자 이름 : 계정 이름  
- 암호 : 해당 계정의 비밀번호  