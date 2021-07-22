터미널에서 실행

myagent.jar 만들기
jar -cmf META-INF/manifest.txt myagent.jar bin/com/example/javaagent/MyAgent.class

Main 실행하기
cd bin/
myagent.jar bin에 복사
java -javaagent:myagent.jar -cp . com.example.javaagent.Main


# 빌드 bin폴더, 패키지 문제로 S03에서 다시 테스트..