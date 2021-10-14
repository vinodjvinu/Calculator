package calculator;

import java.util.Scanner;	

public class Calculator {	
	
	public static void main(String[] args) {
			// TODO Auto-generated method stub
				ArithmeticOP op = new ArithmeticOP();
				short num;
				int a, b;
				System.out.print("Welcome to Arithmetic Calculator: ");
				System.out.println("Choose one of the below operations:");
				System.out.println(" Type 1 for Addition\n Type 2 for Subtraction\n "
							+ "Type 3 for Multiplication \n Type 4 for Division \n");
				System.out.print("Enter now: ");
				Scanner inp = new Scanner(System.in);
				
				num = inp.nextShort();
				
				System.out.print("\nEnter Num1 : ");
				
				a = inp.nextInt();
				
				System.out.print("Enter Num2 : ");
				
				b = inp.nextInt();
				
				if (num == 1)
						op.add(a, b);
				else
					if (num == 2)
							op.subtract(a, b);
					else if (num == 3)
								op.multiply(a, b);
						 else if (num == 4)	
								 	op.division(a, b);
						 	  else 
						 		 System.out.println("Wrong option");
				
				}
}


