# OOP2026
### Homework1
```java
public class HelloWorld {

	public static void main(String[] args) {

		int i, j;
		for(i=0;i<10;i++) {
			for(j=0;j<=i;j++) {
				System.out.print("#");
			}
			for(j=0;j<10;j++) {
				System.out.print(" ");
			}
			System.out.println();
		}
		
		System.out.println();
		
		for(i=10;i>=1;i--) {
			for(j=0;j<i;j++) {
				System.out.print("#");
			}
			for(;j<=10;j++) {
				System.out.print(" ");
			}
			System.out.println();
		}
				
		System.out.println();
		
		for(i=10;i>0;i--) {
			for(j=0;j<i;j++) {
				System.out.print(" ");
			}
			for(;j<=10;j++) {
				System.out.print("#");
			}
			System.out.println();
		}		
		
		System.out.println();
		
		for(i=0;i<10;i++) {
			for(j=0;j<=i;j++) {
				System.out.print(" ");
			}
			for(;j<=10;j++) {
				System.out.print("#");
			}
			System.out.println();
		}
		

	}

}
```

<img width="1109" height="737" alt="image" src="https://github.com/user-attachments/assets/a651d49d-a405-4a84-85c4-ed594726405a" />

### Homework2

```java

public class Homework2 {

	public static void main(String[] args) {
		int i;
		int a = 1, b = 1, c;
		for (i=0; i<20; i++) {
			System.out.print(a + " ");
			c = a + b;
			a = b;
			b = c;
		}

	}

}
```
<img width="1025" height="488" alt="image" src="https://github.com/user-attachments/assets/2f88439d-d749-4caf-ae7a-2ac5a9bca6a1" />

### Homework3

```java


public class Homework3 {

	public static void main(String[] args) {
		int i;
		double a = 1, b = 1, c;
		for (i=0; i<20; i++) {
			System.out.println((a + b)/b + " ");
			c = a + b;
			a = b;
			b = c;
		}

	}

}
```

<img width="1132" height="477" alt="image" src="https://github.com/user-attachments/assets/f09f56cc-614f-494d-8ee7-9a84b3ad2cb7" />

### Homework4

```java

public class Homework4 {

	public static void main(String[] args) {
		int i, j;
		for (i=1;i<10;i++) {
			for (j=1;j<10;j++) {
				System.out.print(j + " X " + i + " = " + i*j + "\t");
			}
			System.out.println();
		} 
		
	}

}
```

<img width="1305" height="763" alt="image" src="https://github.com/user-attachments/assets/749cd2a8-3822-4a5b-96e1-3b751ff81e22" />

## Homework5

```java

	public static void main(String[] args) {
		//라이프니츠 원주율 공식
		
		int k;
		double pi = 0;
		for (k=0; k < 1000; k++) {
			pi += 4*(Math.pow(-1, k)/(2*k + 1));
			System.out.println(pi);
		}
```
<img width="1173" height="637" alt="image" src="https://github.com/user-attachments/assets/cc44984c-666b-4d1e-9ab3-cdd62a726887" />

		
```java

	public static void main(String[] args) {
		//마디바 원주율 공식
		
		int k;
		double pi = 0;
		for (k=0; k < 1000; k++) {
			pi += Math.sqrt(12)*(Math.pow(-1.0/3.0, k)/(2*k + 1));
			System.out.println(pi);
		}
		
	}
```
<img width="1185" height="617" alt="image" src="https://github.com/user-attachments/assets/3ce83e76-11b5-4999-bff9-9d93b1c40475" />



## Homework6

```java

	public static void main(String[] args) {
		int n = 6;
		int[][] binomial = new int[n+1][n+1];
		
		for (int i = 0; i <= n; i++) {
			for (int j = 0; j <= i; j++) {
				if (j == 0 || j == i) {
					binomial[i][j] = 1;
				}
				else {
					binomial[i][j] = binomial[i-1][j-1] + binomial[i-1][j];
				}
			}
		}
		
		for (int i = 0; i <= n; i++) {
			for (int j = 0; j <= i; j++) {
				System.out.print(binomial[i][j] + " ");
			}
			System.out.println();
		}
	}
```

<img width="1219" height="629" alt="image" src="https://github.com/user-attachments/assets/00e062db-40fc-4672-904f-e32f468aa302" />

## Homework7

```java

	public static void main(String[] args) {
		//Selection-sorting 알고리즘 구현하기
		int data[] = new int[20];
		int n = data.length;
		
		for(int i=0; i<n; i++)
		    data[i]=(int)(Math.random()*100);
		
		System.out.print("기존의 배열\t>> ");
		for(int i=0; i<n; i++)
		    System.out.print(data[i] + " ");
		
		for (int i = 0; i < n-1; i++) {
			int minIndex = i;

			for (int j = i + 1; j < n; j++) {
				if (data[j] < data[minIndex]) {
					minIndex = j;
				}
			}
			int swap = data[minIndex];
			data[minIndex] = data[i];
			data[i] = swap;
		}
		System.out.println();
		System.out.println();
		
		System.out.print("정렬된 배열\t>> ");
		for(int i=0; i<n; i++)
		    System.out.print(data[i] + " ");


	}
```

<img width="646" height="752" alt="image" src="https://github.com/user-attachments/assets/579feba9-8653-4797-bb06-8aa0f894b6fb" />

## Homework8

```java

	public static void main(String[] args) {
		int[][] score = new int[30][5];
		
		for (int i = 0; i < 30; i++) {
			int sum = 0;
			
			for (int j = 0; j < 4; j++) {
				score[i][j] = (int)(Math.random()*101);
				sum += score[i][j];
			}
			score[i][4] = sum;
		}
		
		System.out.println("번호 \t국어 \t영어 \t수학 \t과학 \t합계");
		for (int i = 0; i < 30; i++) {
			System.out.print((i+1) + "번\t");
			
			for (int j = 0; j < 5; j++) {
				System.out.print(score[i][j] + "\t");
			}
			System.out.println();
		}

	}
```

<img width="1431" height="757" alt="image" src="https://github.com/user-attachments/assets/95777b26-2a3e-4792-83a6-e32b18bce4e1" />

## Homework9

```java
import java.util.Scanner;
public class Homework9 {

	public static void main(String[] args) {
		// 10진법을 2진법으로 변환
		Scanner stdIn = new Scanner(System.in);
		int[] binary = new int[16];
		int n = binary.length;
		
		System.out.print("십진수 입력 >> ");
		double input = stdIn.nextDouble();
		
		int intPart = (int)input;
		double fracPart = input - intPart;
		
		//정수부 변환
		int i = 0;
		int decimal = intPart;
		while (decimal > 0 && i < n) {
			binary[i] = decimal % 2;
			decimal /= 2;
			i++;
		}
		
		//소수부 변환
		StringBuilder fracResult = new StringBuilder();
		int limit = 10;
		
		for(int k = 0; k < limit && fracPart != 0; k++) {
			fracPart *= 2;
			int bit = (int)fracPart;
			fracResult.append(bit);
			fracPart -= bit;
		}
		
		
		//출력
		System.out.print("십진수를 이진수로 변환: ");
		for (int j = i-1; j >= 0; j--) {
			System.out.print(binary[j]);
		}
		
		System.out.println("." + fracResult);
		
		System.out.println();
		System.out.println();
		
		//2진법을 10진법으로 변환
		System.out.print("이진수 입력 >> ");
		double binaryInput = stdIn.nextDouble();
		
		double binaryToDecimalResult = 0;
		
		int decimalIntPart = (int) binaryInput;
		double decimalFracPart = binaryInput - decimalIntPart;
		
		//정수부 변환
		i = 0;
		while (decimalIntPart > 0) {
			long digit = decimalIntPart % 10;
			binaryToDecimalResult += digit * Math.pow(2, i); // Math.pow함수 아웃풋이 항상 double형 이므로 double로의 형변환 불필요
			decimalIntPart /= 10;
			i++;
		}
		
		//소수부 변환
		i = -1;
		while (i > -10) {
			decimalFracPart *= 10;
			int digit = (decimalFracPart >= 0.9999999) ? 1 : 0; //double 부동소수점 오차를 잡아주는 코드
			binaryToDecimalResult = binaryToDecimalResult + digit * Math.pow(2, i);
			decimalFracPart -= digit;
			i--;
		}
		
		//출력
		System.out.print("\n이진수를 십진수로 변환: " + binaryToDecimalResult);

	}

}
```

<img width="1429" height="817" alt="image" src="https://github.com/user-attachments/assets/6882c6db-f9a7-4ffa-b85d-105085e288b2" />
<img width="1376" height="801" alt="image" src="https://github.com/user-attachments/assets/861340f5-629f-4ceb-bb57-1e70b7610651" />




## Homework10

```java
	public static void main(String[] args) {
		// 도수분포표 만들기
		for (int i=0; i<args.length; i++) {
			//System.out.println(args[i]);   
			Integer.parseInt(args[i]);
			}
		
		int arrayCount   = Integer.parseInt(args[0]);  // 100 (데이터 개수)
		int maxValue     = Integer.parseInt(args[1]);  // 100 (0~100 범위)
		int binSize      = Integer.parseInt(args[2]);  // 10  (10 단위로 구간 나누기)
		int displayScale = Integer.parseInt(args[3]);  // 1   (# 하나가 몇 개를 의미하는지)
		/*
		int arrayCount   = 100;  // 100 (데이터 개수)
		int maxValue     = 100;  // 100 (0~100 범위)
		int binSize      = 10;  // 10  (10 단위로 구간 나누기)
		int displayScale = 1;  // 1   (# 하나가 몇 개를 의미하는지)
		*/
		//data배열에 0~99까지 랜덤 값 대입
		int[] data = new int[arrayCount];
		for (int i = 0; i < data.length; i++) {
			data[i] = (int)(Math.random()*(maxValue));
		}
		
		int binCount = (maxValue + 1) / binSize;	//구간 갯수 계산
        int[] frequency = new int[binCount];		//구간 10개 짜리 배열 생성

        
        for (int i = 0; i < data.length; i++) {
            int binIndex = data[i] / binSize;       // 어느 구간에 속하는지 계산
            frequency[binIndex]++;					// binIndex가 0이라면  frequency[0] 값이 1증가함
        }
        
        for (int i = 0; i < binCount; i++) {
            int rangeStart = i * binSize;
            int rangeEnd = rangeStart + binSize - 1;

            System.out.print(rangeStart + "~" + rangeEnd + "\t\t");

            int barLength = frequency[i] / displayScale;
            for (int j = 0; j < barLength; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
	}
```

<img width="1448" height="818" alt="image" src="https://github.com/user-attachments/assets/707b1e49-ec34-4946-a5e5-08982371ccb7" />






