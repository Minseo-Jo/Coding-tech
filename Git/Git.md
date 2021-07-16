# Git이란?

>#### **Git**이란 버전 관리 시스템(VSC, Version Control System)의 한 종류이다. 


### Git의 3대 목적

#### 1. *version*
```
Git에서는 소스코드가 변경된 이력을 쉽게 확인할 수 있고, 특정 시점에 저장된 버전과 비교하거나 특정 시점으로 돌아갈 수 있다.

또한 내가 올리려는 파일이 누군가 편집한 내용과 충돌한다면, 
서버에 업로드 할 때 경고 메시지가 발생하여 누군가 애써 편집한 내용을 덮어써버리는 실수를 피할 수 있게 한다. 

```
> #### *ex)*

![create a new repository](https://user-images.githubusercontent.com/87311912/125887104-005002b5-ee28-4156-9259-7c72c888271c.jpg)
 
 Github-test라는 새로운 repository를 만들면 Github-test라는 폴더가 생성되고 그 안에는 .git이라는 폴더가 생성되는 걸 확인할 수 있다.
 
 새롭게 만들어진 버전들은 이 .git 폴더에 저장된다. 
 
 
![create new file](https://user-images.githubusercontent.com/87311912/125887163-27f1af1f-57f8-4c26-bba1-76dcbcc99b9d.jpg)
  
  Github-test 폴더 안에 hello.txt파일을 생성해보자. 
  
  Git은 hello.txt파일이 생성되었다는 것을 인지하고 Desktop에 이 파일을 올려둔다. 
 
 
![first commit](https://user-images.githubusercontent.com/87311912/125887211-62d97103-8ba1-4a2f-9f5b-476493dfc227.jpg) 
 
 hello.txt파일에 내용을 입력하고 작업의 이름을 Message1으로 남겨 둔 다음 commit 한다. 
 
 **commit**이란 버전을 생성한다는 뜻 정도로 이해하면 될 것 같다. 





#### 2. *backup*
```
정보를 안전하게 보호하기 위한 수단 
```



#### 3. *collaborate*

