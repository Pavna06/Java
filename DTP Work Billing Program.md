# DTP Work Billing Program

Write a program to calculate the bill of a DTP work as follows. Use if-else statement to 
determine if the user wants typing or copying done.
<br>
a. The rate of typing Rs. 3/Page 
<br>
b. Printing of first copy Rs.5/page and later every copy Rs.3/Page. Given the number of pages,
print the total cost.

### Code
import java.util.*;
class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter type of work (typing/copying): ");
        String a=sc.nextLine();
        System.out.print("Number of pages: ");
        int n=sc.nextInt();
        a=a.toLowerCase();
        int tot=0;
        if(a.equals("typing"))
        tot=n*3;
        else if(a.equals("copying"))
        {
            System.out.print("Enter number of copies: ");
            int c=sc.nextInt();
            tot=(n*5)+((c-1)*3);
        }
        else
        System.out.println("Invalid");
        System.out.print("The cost is: "+tot);
    }
}
