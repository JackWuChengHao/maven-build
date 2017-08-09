# maven-build
新建maven-build登入 http://mirror.bit.edu.cn/apache/ 选择maven的最新版本的二进制，并进行解压
设置环境变量MAVEN_HOME 为解压的路径D:\apache-maven-3.5.0
设置环境变量为 Path 为 ;%MAVEN_HOME%\bin
进入dos环境mvn --version  有反应成功
使用对应jar的pom.xml文件
接下来 mvn -f pom.xml dependency:copy-dependencies 即可
或者将其写进bat脚本中也很简单call mvn -f pom.xml dependency:copy-dependencies \n @pause
然后双击脚本或者执行7步中的命令就可以在当前脚本处生成target文件夹，里面就是所需的jar
