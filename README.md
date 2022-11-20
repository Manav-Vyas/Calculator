# cal
import java.util.Scanner;
public class Calculator {
	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
		int result = 0;
		while(true)
		{
			System.out.println("Enter the operator: ");
			char op = in.next().trim().charAt(0);
			
			if(op=='+' || op=='-' || op=='*' || op=='/' || op=='%') {
				System.out.println("Enter the two number: ");
				int n1 = in.nextInt();
				int n2 = in.nextInt();
				
				if(op=='+') {
					result = n1+n2;
				}
				if(op=='-') {
					result = n1-n2;
				}
				if(op=='*') {
					result = n1*n2;
				}
				if(op=='/') {
					if(n2!=0) {
						result = n1/n2;
					}	
				}
				if(op=='%') {
					result = n1%n2;
				}
			}
				else if(op=='x'||op=='X') {
					break;
				}
				else {
					System.out.println("Invalid operator!!");
				}
				System.out.println("Result is : "+result);
			}
		}
	}

	
