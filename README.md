# OOP2026
### Homework1
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");


public class Homework1{
  public static void main(String []args){
    int i, j;
    for(i=0; i<10; i++) {
      for(j=0; j<10; j++) {
        System.out.print("#");
      }
      System.out.println("");
    }
  }
}

```
![Alt homework11](./images/homework1.jpg)


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
public class Fibonacci {
    public static void main(String[] args) {
        int count = 20;
        long[] fibonacci = new long[count];
        
        fibonacci[0] = 1;
        fibonacci[1] = 1;

        for (int i = 2; i < count; i++) {
            fibonacci[i] = fibonacci[i - 1] + fibonacci[i - 2];
        }

        
        System.out.println("피보나치 수열 (1 ~ 20번째):");
        for (int i = 0; i < count; i++) {
            System.out.print(fibonacci[i] + " ");
        }
    }
}

### Homework3
public class GoldenRatio {
    public static void main(String[] args) {
        long a = 1; // F_1
        long b = 1; // F_2
        
        System.out.println("=== 피보나치 황금비율 계산 (1~20번째) ===");

        for (int i = 1; i <= 20; i++) {
            long next = a + b;
            
            double ratio = (double) b / a; 
            
            System.out.printf("%2d번째: %d / %d = %.6f%n", i, b, a, ratio);
            
            a = b;
            b = next;
        }
    }
}

### Homework4

