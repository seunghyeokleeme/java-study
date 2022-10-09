# String method

```java

import java.awt.*;

public class Sample {
    public static void main(String[] args) {
        // indexOf
        /*
        문자열에서 특정 문자가 시작되는 인덱스를 return!
         */

        String a = "Hello Java";
        System.out.println(a.indexOf("Java"));

        // contains - 특정 문자열이 포함되어 있는지의 여부 판별
        System.out.println(a.contains("Java"));

        // charAt - 특정 위치의 문자를 리턴한다. -> char 자료형의 값
        System.out.println(a.charAt(6)); // j

        // replaceAll - 특정 문자열을 다른 문자열로 바꾸고 싶을 경우
        System.out.println(a.replaceAll("Java", "World")); // 원본 자체 수정 X
        System.out.println(a);

        /* substring - 특정 부분을 뽑아낼 경우
        기록!) substring(시작위치, 끝위치) -> 끝 위치는 포함 되지 않는다.
         */
        System.out.println(a.substring(0, 4)); // Hell 출력 ,원본 자체 수정 X

        // toUpperCase - 문자열 모두 대문자로 변경하고 싶을 경우
        System.out.println(a.toUpperCase()); // 원본 자체 수정 X
        System.out.println(a);

        // split - 문자열을 특정 구분자로 분리
        String b = "a:b:c:d";
        String[] result = a.split(":"); //{"a", "b", "c", "d"}

        // - 문자열 포메팅 - String.format()

        // 1. 숫자 바로 대입
        System.out.println(String.format("I eat %d apples.", 3)); // %d -> 문자열 포멧코드(int): 숫자

        // 2. 문자열 바로 대입
        System.out.println(String.format("I eat %s apples.", "five")); // %s - 문자열

        // 3. int 자료형 변수 대입
        int number = 3;
        System.out.println(String.format("I eat %d apples.", number));

        // 4. 2개 이상의 값 넣기
        int number2 = 10;
        String day = "three";

        System.out.println(String.format("I ate %d apples. so I was sick for %s days.", number2, day));

        // 포멧 코드와 숫자 함께 사용하기
    }

}
```
