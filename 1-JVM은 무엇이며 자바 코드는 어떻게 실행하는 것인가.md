# 목표

> 자바 소스 파일(.java)을 JVM으로 실행하는 과정 이해하기.

---

## 학습할 것

- JVM이란 무엇인가
- 컴파일 하는 방법
- 실행하는 방법
- 바이트코드란 무엇인가
- JIT 컴파일러란 무엇이며 어떻게 동작하나
- JVM 구성 요소
- JDK와 JRE의 차이

---

# 1. JVM은 무엇이며, 자바 코드는 어떻게 실행하는 것인가?
---
## 1. JVM이란 무엇인가
---
> 자바 가상 머신. 자바 바이트 코드(.class)를 OS에 특화된 코드로 변환(인터프리터와 JIT)하여 실행

JVM은 플랫폼(예로 운영체제) 독립적으로, JVM이 실행 가능한 환경이라면 어디서든 자바 프로그램을 실행 가능하도록 함.

## 2. 컴파일 하는 방법

### Java 코드

```java
public class Java_study {
    public static void main(String[] ar) {
        System.out.println("Hello, JAVA");
    }
}
```

### 컴파일 후 결과

![컴파일](./img/1-javac.png)