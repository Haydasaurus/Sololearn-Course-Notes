# Time Converter
You need a program to convert days to seconds.  
The given code takes the amount of days as input. Complete the code to convert it to seconds and output the result.  
  
**Sample Input:**  
12  
  
**Sample Output:**  
1036800

>🛈 Explanation: 12 days are 12 x **24** = 288 hours, which are 288 x **60** = 17280 minutes, which are 17280 x **60** = **1036800** seconds.

```java
import java.util.Scanner;

public class Program {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		int days = scanner.nextInt();

		//your code goes here
		System.out.print(days*24*60*60);

	}
}
```
