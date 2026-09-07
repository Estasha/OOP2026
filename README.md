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


