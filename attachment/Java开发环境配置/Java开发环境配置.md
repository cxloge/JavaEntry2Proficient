#Java 开发环境配置

##window系统安装java
###下载安装JDK
[JDK下载地址](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

安装：JDK安装完成后事接着JRE的安装，所以JRE可装也可不装。。。无影响的。因为JDK 里面已经有了一个JRE。（**JDK的安装路径最好不要带中文和空格。**）

JDK与JRE的区别

| 简称   | 全称                      | 解释                                       |
| ---- | ----------------------- | ---------------------------------------- |
| JDK  | Java Development Kit    | 简单的说JDK是面向开发人员使用的SDK，它提供了Java的开发环境和运行环境。SDK是Software Development Kit 一般指软件开发包，可以包括函数库、编译程序等。 |
| JRE  | Java Runtime Enviroment | 是指Java的运行环境，是面向Java程序的使用者，而不是开发者。        |

###配置环境变量

|    变量名    | 变量值                                      | 备注                                       |
| :-------: | :--------------------------------------- | :--------------------------------------- |
| JAVA_HOME | C:\Program Files\Java\jdk1.7.0           | //这里是你JDK的安装路径，可以更换。JAVA_HOME指向的是JDK的安装路径 |
|   Path    | %JAVA_HOME%\bin; %JAVA_HOME%\jre\bin;    | PATH环境变量原来Windows里面就有，你只需修改一下，使他指向JDK的bin目录 |
| CLASSPATH | .;%JAVA_HOME%\lib\dt.jar; %JAVA_HOME%\lib\tools.jar; | //记得前面有个"."。dt.jar是关于运行环境的类库,主要是swing的包。设置Classpath的目的，在于告诉Java执行环境，在哪些目录下可以找到您所要执行的Java程序所需要的类或者包。 |



###测试JDK是否安装成功

1."开始"->;"运行"，键入"cmd"；

2.键入命令"java -version"，"java"，"javac"几个命令，出现画面，说明环境变量配置成功；

| 命令    | 用法                                       |
| ----- | ---------------------------------------- |
| java  | java是用来运行编译好的.class文件的。命令行下直接输入java可以看到大量提示信息，提示java命令的用法。**java -version  输出产品版本并退出** |
| javac | avac是用来编译.java文件的。命令行下直接输入javac可以看到大量提示信息，提示javac命令的用法 |

java的环境配置，配置完成后直接启动eclipse，它会自动完成java环境的配置。

## window系统使用Eclipse

[Eclipse下载地址](http://www.eclipse.org/downloads/)

[Eclipse语言包babel下载地址](http://www.eclipse.org/babel/downloads.php)

注意：JDK版本的位数需要与Eclipse对应。java -version 没有提示是64位，默认是32位。

### HelloWorld.java

```java
//HelloWorld.java
public class HelloWorld {
	// main 然后 alt+/
	public static void main(String[] args) {
		// 打印HelloWord字符串,Syso然后按 ALT+/,快捷输出
		System.out.println("Hello World !");
	}

}
```

###用Eclipse编译运行HelloWorld.java

![Eclipse-HelloWorld](C:\Users\chenxiaolong\Desktop\Java开发环境配置\Eclipse-HelloWorld.png)

##Mac OS X 下搭建 Java 开发环境

（未完，待续.......）