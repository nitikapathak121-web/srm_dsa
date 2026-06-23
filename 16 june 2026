1. If-Else ladder...

import java.util.Scanner;

public class GradeCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Marks: ");
        int marks = sc.nextInt();

        if (marks >= 40 && marks <= 49) {
            System.out.println("Grade: D");
        }
        else if (marks >= 50 && marks <= 59) {
            System.out.println("Grade: D+");
        }
        else if (marks >= 60 && marks <= 69) {
            System.out.println("Grade: C");
        }
        else if (marks >= 70 && marks <= 75) {
            System.out.println("Grade: C+");
        }
        else if (marks >= 76 && marks <= 80) {
            System.out.println("Grade: B+");
        }
        else if (marks >= 81 && marks <= 87) {
            System.out.println("Grade: A");
        }
        else if (marks >= 88 && marks <= 96) {
            System.out.println("Grade: A");
        }
        else if (marks > 96) {
            System.out.println("Grade: A+");
        }
        else {
            System.out.println("Fail");
        }

        sc.close();
    }
}

-------------------------------------------------------------------------------

2. Pattern 1...

* * * * *
* * * * *
* * * * *
* * * * *
* * * * *

class Main {
    public static void main(String[] args) {
        for(int i=1; i<=5; i++)
        {
            for(int j=1; j<=5; j++)
            {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}

-----------------------------------------------------------------------------------

3. Pattern 2...

*
* *
* * *
* * * *
* * * * *

class Main {
    public static void main(String[] args) {
        for(int i=1; i<=5; i++)
        {
            for(int j=1; j<=i; j++)
            {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}

-----------------------------------------------------------------------------------

4. Reverse Integer(LeetCode problem 7)...

class Solution {
    public int reverse(int x) {
        int min = Integer.MIN_VALUE;
        int max = Integer.MAX_VALUE;
        
        if(x == min || x == max){
            return 0;
        }
        int rev = 0;
        while(x != 0)
        {
            int lastDigit = x%10;
            if(rev>max/10 || rev<min/10){
                return 0;
            }
            rev = rev * 10 + lastDigit;
            x = x/10;
        }
        return rev;
    }
}
