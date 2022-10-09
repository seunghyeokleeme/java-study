# equal method

```java
// String method
        /* eauals
        - 문자열 동일 한지 비교 후, return value!
         */
        String a = "hello";
        String b = "java";
        String c = "hello";
        System.out.println(a.equals(b));
        System.out.println(a.equals(c)); // 기록!) 문자열의 값을 비교 할때는 반드시 equals을 사용해야 한다!!!!  == 연산자 사용 X
        System.out.println(a == c); // false 를 반환! why..? a와 c는 서로 다른 객체!, 즉 == 는 두개의 자료형이 동일한 객체인지를 판별할 때 사용하는 연산자.
```
