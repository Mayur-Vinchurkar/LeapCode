# LeapCode
package program;

import java.util.Scanner;

public class Leapyear {
	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		System.out.print("Enter a year: ");
		int year = input.nextInt();

		if (year % 400 == 0) {
			// System.out.println("*****in condition 1st*****");

			System.out.println(year + " is  a leap year.");
			// All years divisible by 400 ARE leap years
		} else if ((year % 100 == 0) && (year % 400 != 0)) {
			// System.out.println("*****in condition 2nd*****");

			System.out.println(year + " is not a leap year.");
			// All year divide by 100 but year is not divisible by 400
		} else if ((year % 4 == 0) && (year % 100 != 0)) {
			// System.out.println("*****in condition 3rd*****");

			System.out.println(year + " is  a leap year.");
			// All years divisible by 4 but not by 100 ARE leap years
		} else if ((year % 4 != 0)) {
			// System.out.println("*****in condition 4th*****");

			System.out.println(year + " is not a leap year.");
			// All years not divisible by 4 are NOT leap years
		}

	}

}
