# POSIX CLI

### *GUI VS CLI*
운영체제를 관리하는 방법에는 2가지가 있다. 

**GUI(Graphic user interface)** 와 **CLI(Command line interface)** 이다.

GUI는 그래픽컬한 방법으로 컴퓨터를 조작하는 것이다. 마우스, 터치, 버튼 등을 이용하는 것에 해당한다. 

CLI는 명령어를 이용하여 언어적으로 컴퓨터를 제어하는 것이다. 

당연히 GUI보다 어렵고 복잡할 것이다. 

그럼에도 불구하고 왜 CLI를 배워야하고 많은 프로그래머들이 이를 이용하는 것일까?

언어를 이용하면 우리의 의사를 정확하게 전달할 수 있다. 

CLI의 결정적인 장점 중 하나는 GUI는 절대 따라올 수 없는, 시간의 순서에 따라서 명령을 내릴 수 있다는 것이다. 

또한 CLI는 운영체제 용량도 매우 작고 CPU, 메모리도 적게 사용하기 때문에 컴퓨터가 본연의 일에 충실하게 동작하는데 매우 좋다.

### *POSIX*

**Posix(Portable operating system interface)** 는 Uinx계열의 컴퓨터(Unix, Linux, Mac OS)들을 서로 동일한 방법으로 제어하기 위한 일종의 표준이다.

Window 같은 경우에는 Posix를 따르지 않기 때문에 이와 호환되지 않는다. 

하지만 에뮬레이터, 일종의 통역과 같은 역할을 하는 프로그램을 설치하면 Posix와 같은 방법으로 컴퓨터를 제어할 수 있다. 

### *데이터 처리 방법*

우리가 데이터를 저장하는 곳은 file이다. 

이 많은 file들을 관리하기 위해 만들어진 도구가 directory이다.

즉 우리는 수많은 directory를 directory에 저장한다.

그렇다면 저장된 데이터들은 어떻게 처리할까?

4가지 데이터 처리방법이 있다.

```
C reate
R ead
U pdate
D elete
```

즉 생성, 읽기, 수정, 삭제를 할 줄 안다면 우리는 Cli를 할 수 있다. 

### *Directory의 사용*

파일에는 데이터, 데이터를 처리하는 프로그램 이 두가지 정보가 저장된다.

이 파일들은 디렉토리에서 관리된다. 

그러므로 운영체제를 다룬다는 것은 파일, 즉 디렉토리를 다룬다는 것이라고 할 수 있다. 

Cli방식을 사용하여 디렉토리를 관리하는 방법을 알아보자. 

나는 Window 운영체제를 사용하고 있기 때문에 에뮬레이터로 버전관리도구 중 하나인 **Git** 을 사용하였다. 

![directory의 사용 git bash 화면](https://user-images.githubusercontent.com/87311912/126054527-c3f2c783-decc-4b3b-be3e-863164db49e1.jpg)

첫번째 줄부터 살펴보자.

**pwd(print working directory)** 는 내가 지금 어디에 있는지 확인하는 방법이다. 

이를 통해 나는 지금 로컬 디스크c: 의 users의 82104 디렉토리에 있음을 알 수 있다. 

우리는 이 위치를 **home directory** 라고 부른다. 

즉 기본적으로 터미널을 열었을 때 위치하고 있는 곳으로 이는 컴퓨터마다 다를 것이다.  

**cd(change directory)** 는 위치하고 있는 디렉토리를 바꾸고 싶을 때 사용하는 명령어이다.  

**/(root directory)** 를 입력하게 되면 우리는 최상위 디렉토리로 이동할 수 있다. 

두번째 줄과 같이 cd / 를 입력하게 되면 최상위 디렉토리로 이동한 것을 확인할 수 있다. 

home directory로 다시 되돌아가는 방법에는 cd / (home directory 주소 입력) 과 cd ~ 를 입력하는 방법이 있다. 

### *현재 Directory의 상태보기와 명령어의 형식*

디렉토리에 어떤 디렉토리와 파일이 있는지 알기 위해 cli에서 어떤 명령어 형식을 사용하는 지 알아보자.

![ls](https://user-images.githubusercontent.com/87311912/126056510-6ec7746f-46da-4435-8640-fd344ec10d1c.jpg)

**ls** 를 입력하게되면 Git은 우리에게 home directory에 있는 디렉토리들과 파일들을 보여준다. 

만약 디렉토리, 파일에 관한 시간 정보, 용량 등 자세한 정보를 알고 싶을 때는 어떻게 할까?

![ls--help](https://user-images.githubusercontent.com/87311912/126056511-cd6db27e-500a-4159-b521-70c2aa6af389.jpg)

posix 계열의 시스템들은 주로 명령어 뒤에 **--help**를 입력하면 간략한 사용법을 알려주는 경우가 많다. 

![ls--l 설명](https://user-images.githubusercontent.com/87311912/126056512-14cf381b-bd13-4ace-ab9e-66fd4b7606fe.jpg)

ls --help를 입력하여 사용법을 확인해보니 -l 이 풍부한 형식으로 리스트를 보여준다는 방법이라는 것을 알 수 있었다. 

![ls--l](https://user-images.githubusercontent.com/87311912/126056514-e9c0db21-6a5d-4a19-ad05-1592a525eb75.jpg)

ls -l한 결과이다.

추가로 posix 계열의 시스템에서 내용이 없는 파일을 만드는 간편한 방법이 있다.

**touch** 명령어 뒤에 파일명을 쓰는 방법이다.

![touch showfile생성](https://user-images.githubusercontent.com/87311912/126056517-acee3b6f-4d96-4c80-b789-692424cd13b8.jpg)


touch 명령어를 사용해서 showfile.txt를 생성하고 ls를 통해 생성된 파일을 확인하였다.

posix 시스템들은  **.(파일명)** ,파일명 앞에 .이 붙어있으면 숨김 파일로 간주한다.

![touch  hiddenfile](https://user-images.githubusercontent.com/87311912/126056520-e142adfc-048e-4337-82db-9a7dabc8cd7a.jpg)

이를 사용하여 .hiddenfile.txt를 생성하고 ls 입력해보니 이 파일이 확인되지 않았다.

감춰진 파일을 확인하고 싶을 때는 어떻게 할까? 

ls --help를 보고 이에 관한 명령어를 찾아보자.

-a 명령어가 .으로 시작하는 파일도 출력해준다는 것을 알 수 있었다.

![ls --a](https://user-images.githubusercontent.com/87311912/126056530-037a02f1-5593-4ce6-b49d-339e5e02ec19.jpg)

ls -a를 입력해보니 .hiddenfile.txt을 발견할 수 있었다. 


