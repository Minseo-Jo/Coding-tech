# Git이란?

>#### **Git**이란 버전 관리 시스템(VSC, Version Control System)의 한 종류이다. 


### Git의 3대 목적

#### 1. *version*
```
Git에서는 소스코드가 변경된 이력을 쉽게 확인할 수 있고, 특정 시점에 저장된 버전과 비교하거나 특정 시점으로 돌아갈 수 있다.
```
> #### *ex)*

![create a new repository](https://user-images.githubusercontent.com/87311912/125887104-005002b5-ee28-4156-9259-7c72c888271c.jpg)
 
 Github-test라는 새로운 repository를 만들면 Github-test라는 폴더가 생성되고 그 안에는 .git이라는 폴더가 생성되는 걸 확인할 수 있다.
 
 새롭게 만들어진 버전들은 이 .git 폴더에 저장된다. 
 
 
![create new file](https://user-images.githubusercontent.com/87311912/125887163-27f1af1f-57f8-4c26-bba1-76dcbcc99b9d.jpg)
  
  Github-test 폴더 안에 hello.txt파일을 생성해보자. 
  
  Git은 hello.txt파일이 생성되었다는 것을 인지하고 Desktop에 이 파일을 올려둔다. 
 
 
![first commit](https://user-images.githubusercontent.com/87311912/125887211-62d97103-8ba1-4a2f-9f5b-476493dfc227.jpg) 
 
 hello.txt파일에 내용을 입력하고 작업의 이름을 Message 1으로 남겨 둔 다음 commit 한다. 
 
 **commit**이란 버전을 생성한다는 뜻 정도로 이해하면 될 것 같다. 
 
 
![second commit](https://user-images.githubusercontent.com/87311912/125890360-2997a64f-9bd3-4d3f-b0c5-e9f1c807cedc.jpg)

hello.txt파일을 수정한 뒤 작업의 이름을 Message 2로 남겨두고 commit 한다.

Git의 버전관리의 핵심은 **각각의 버전 사이의 차이점을 손쉽게 볼 수 있다**는 것이다.

이를 어떻게 확인할 수 있을까?

좌측 상단의 History를 클릭해본다. 

![confirm history](https://user-images.githubusercontent.com/87311912/125890401-589c7d20-907e-4fcb-a9f7-834f53cb2667.jpg)

History의 기록을 통해 문서들의 변경사항들을 추적해나갈 수 있다.

또한 몇 번의 클릭으로 우리는 과거의 프로젝트로 돌아갈 수도 있다. 








#### 2. *backup*
```
Git은 정보를 안전하게 보호하기 위한 수단으로 사용된다. 
```

우리는 언젠가 우리 컴퓨터 내의 파일들이 유실될 것임을 확신할 수 있다.
그러므로 그 파일들이 귀중한 정보라면 **백업(backup)** 을 해야한다. 

즉 다른 컴퓨터에 이 파일들을 복제해야한다.

우리는 백업할 컴퓨터를 살 수도 있고 이를 제공해주는 사업자들의 서비스를 이용할 수 있다.  

가장 대표적인 서비스가 **github.com**이다.

> #### *ex)*



#### 3. *collaborate*

