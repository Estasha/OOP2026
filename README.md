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

<img width="1426" height="748" alt="image" src="https://github.com/user-attachments/assets/f2f06160-4edd-45a3-8919-074e31b1a806" />




