# OOP2026
### Homework1
```java
public class Homework1{
  public static void main(String[] args) {
		int i, j;
		for(i=0; i<10; i++) {
			  for(j=0; j<=i; j++) {
			    System.out.print(" ");
			  }
			  for(; j<=10; j++) {
			    System.out.print("#");
			  }
			  System.out.println();
			}
	}

}
### Homework2


### Homework3
public class GoldenRatio {
    public static void main(String[] args) {
        long a = 1; // F_1
        long b = 1; // F_2
        
        System.out.println("=== 피보나치 황금비율 계산 (1~20번째) ===");

        // F_2 / F_1 부터 F_21 / F_20 까지 총 20개의 비율 계산
        for (int i = 1; i <= 20; i++) {
            long next = a + b; // 다음 피보나치 수 (F_n+1)
            
            // double 형변환을 통해 소수점 연산 수행
            double ratio = (double) b / a; 
            
            System.out.printf("%2d번째: %d / %d = %.6f%n", i, b, a, ratio);
            
            a = b;
            b = next;
        }
    }
}

### Homework4
