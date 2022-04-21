# nexus-deploy-tekton 테스트를 위한 spring 소스코드 입니다.

## Nexus (192.168.9.194:32001) "test-hosted" repository 에 deploy
```
mvn clean
mvn deploy
```
## Deploy 확인
1. nexus (http://192.168.9.194:32001/#browse/browse) 에 접속 후 로그인 진행 (아이디: admin / 비밀번호: admin)
2. "test-hosted" repository 에 echo_maven 업로드 확인

## Terminal 에서 jar 실행 
```
java -jar ./target/echo_maven-0.0.1.SNAPSHOT.jar
```

## 코드실행화면
{address}/echo/hello -> hello 출력

![image](/figure/소스코드_실행화면1.png)

{address}/echo/안녕하세요 -> 안녕하세요 출력

![image](/figure/소스코드_실행화면2.png)
