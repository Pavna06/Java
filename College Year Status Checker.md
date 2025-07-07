# College Year Status Checker

Write a Python program in which a student enters the number of college credits earned. If     
the number of credits is greater than 90, 'Senior Status' is displayed; if greater than 60,  
'Junior  Status' is displayed; if greater than 30, 'Sophomore Status' is displayed; else,      
'Freshman Status'  is displayed. 

### Code
import java.util.*;
class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the number: ");
        int a=sc.nextInt();
        if(a>90)
        System.out.println("Senior status");
        else if(a>60)
        System.out.println("Junior status");
        else if(a>30)
        System.out.println("Sophmore status");
        else
        System.out.println("Fresher status");
    }
}
