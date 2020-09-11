# WIPRO-Programs
Hello this is Repository file where i'll be sharing the WIPRO basic programs related to JAVA Programming Language
Go throught the list

-Programms edited by 
-Weaver

1) User ID creation using First Name, Last Name, Pin and a extra value. 


import java.util.Scanner;
public class UserId generation{
public String userIdGeneration(String input1,String input2,int input3,int input4)
int s1=input1.length();
        int s2=input2.length();
        String longer="";
        String smaller="";
        String output1="";
        if(s1==s2)
        {
        if(input1.compareTo(input2)>0)
        {
            longer=input1;
            smaller=input2;
        }
            else
            {
                longer=input2;
                smaller=input1;
            }
        }
           
        if(s1>s2){
            longer=input1;
            smaller=input2;
        }
        else if(s1<s2)
        {
            longer=input2;
            smaller=input1;
        }
        String pin=input3+"";
        String output=longer.charAt(0)+smaller+pin.charAt

(input4-1)+pin.charAt(pin.length()-input4);
        for(int i=0;i<output.length();i++)
        {
            if(Character.isLowerCase(output.charAt

(i)))
            {
                output1+=Character.toUpperCase

(output.charAt(i));
               
            }
            else
            {
                output1+=Character.toLowerCase

(output.charAt(i));
            }
        }
        return output1;
      }
   }
