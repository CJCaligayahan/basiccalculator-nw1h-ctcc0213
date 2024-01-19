package consolebased.basiccalculator;

import java.util.Scanner;

public class BasicCalculator {

    public static void main(String[] args) {
        
     int  counter = 1;
     
     do { counter = (1 + 1);
         
      Scanner user = new Scanner(System.in);
    
      System.out.println("Welcome to Math World, Wizards!");
      
      System.out.println("Mathematical Operator");
     
      String [] operators = {"1. Addition", "2. Subtraction", "3. Multiplication", "4. Division", "5. Exit"};
          for (String a : operators) {
          System.out.println(a);
     }
    
     System.out.print("Choose Operator: ");
      int choice = user.nextInt();
      
       if (choice == 5) {
          System.out.println("Thank you!");
          System.exit(0);
          
     } if(choice >= 6 || choice == 0) {
          counter = (1 * 0);
           System.out.println("ERROR! Please select from option ");
      
     } else if (choice <= 4) {
      System.out.print("Enter 1st Number: ");
      float num1 = user.nextFloat();
      
      System.out.print("Enter 2nd Number: ");
      float num2 = user.nextFloat();
      
      switch (choice) {
            

          case 1: 
               float sum = num1 + num2;
               System.out.println("Sum: " + sum);
         
              break;
              
          case 2:
               float difference = num1 - num2;
               System.out.println("Difference: " + difference);
               
              break;
              
          case 3:
               float product = num1 * num2;
               System.out.println("Product: " + product);
             
              break;
              
          case 4:
              float quotient = num1 / num2;
              
              if (num2 != 0) {
                  System.out.println("Quotient: " + quotient);
              } else {
               System.out.println("Math ERROR");
              }
              break;
    
          
              
      } 

      }
      
      } 
     
        while(counter == 0 );      
        
       
  }
}
