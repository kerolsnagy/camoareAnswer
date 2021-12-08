# camoareAnswer
package com.company;

import jdk.swing.interop.SwingInterOpUtils;

import java.util.Scanner;

public class Main
{
    public static void main (String args[])
    {
        Scanner k = new Scanner(System.in);
        System.out.println("test yourself :");
        System.out.println("what is '5+10/2*10 = ?' ");
        float userAnswer,theCorrectAnswer=55;
        boolean questionAnswer=false;
        for (int i = 1; i <= 3; i++)
        {
        userAnswer=k.nextFloat();
        if (userAnswer==theCorrectAnswer) 
        {
            questionAnswer=true;
            break;
        }
        else if (userAnswer != theCorrectAnswer)
        {
            System.out.println("Chance # " + (i+1) + " : ");
            continue;
         }
        }
        if (questionAnswer)
            System.out.println("Correct Answer");
        else
            System.out.println("wrong Answer");
    }
}
