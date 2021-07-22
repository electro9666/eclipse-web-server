터미널에서 실행

## 주의
기본 패키지 사용하지 말기!!! 에러 발생.

# agent 컴파일
javac com/example/MyAgent.java
# myagent.jar 만들기
jar -cmf manifest.txt myagent.jar com/example/MyAgent.class

# Main 실행하기
javac com/example/MyMain.java
java com.example.MyMain
java -javaagent:myagent.jar -cp . com.example.MyMain


## 참고
https://www.javamex.com/tutorials/memory/instrumentation.shtml
https://www.python2.net/questions-481944.htm