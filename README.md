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


### Homework2

public class Homework2 {
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

public class Homework3 {
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

public class Homework4 {
    public static void main(String[] args) {
        for (int i = 1; i <= 9; i++) {
            for (int j = 1; j <= 9; j++) {
                
                System.out.printf("%d*%d=%-2d\t", j, i, j * i);
            }
            System.out.println(); // 한 줄 출력 후 줄바꿈
        }
    }
}

### Homework5


### Homework6


### Homework7
public class SelectionSort {
    public static void main(String[] args) {
        int[] data = new int[20];

    
        for (int i = 0; i < 20; i++) {
            data[i] = (int) (Math.random() * 100);
        }

        
        System.out.println("=== 정렬 전 ===");
        for (int i = 0; i < 20; i++) {
            System.out.print(data[i] + " ");
        }
        System.out.println("\n");

        
        for (int i = 0; i < data.length - 1; i++) {
            int minIndex = i; 

          
            for (int j = i + 1; j < data.length; j++) {
                if (data[j] < data[minIndex]) {
                    minIndex = j;
                }
            }

            int temp = data[i];
            data[i] = data[minIndex];
            data[minIndex] = temp;

        
        System.out.println("=== 정렬 후 (오름차순) ===");
        for (int i = 0; i < 20; i++) {
            System.out.print(data[i] + " ");
        }
        System.out.println();
    }
}


### Homework8

public class StudentScores {
    public static void main(String[] args) {
        int studentCount = 30;
        int subjectCount = 4;
        
        
        int[][] score = new int[studentCount][subjectCount];
        
        for (int i = 0; i < studentCount; i++) {
            for (int j = 0; j < subjectCount; j++) {
                score[i][j] = (int) (Math.random() * 101);
            }
        }
        
        System.out.println("번호\t국어\t영어\t수학\t과학\t합계");
        System.out.println("--------------------------------------------");

        
        for (int i = 0; i < studentCount; i++) {
            int sum = 0;
            System.out.printf("%-2d\t", i + 1); 

            for (int j = 0; j < subjectCount; j++) {
                System.out.printf("%d\t", score[i][j]);
                sum += score[i][j]; 
            }

            System.out.printf("%d\n", sum); 
        }
    }
}
