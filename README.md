## Task1
import java.util.Scanner;  // Import the Scanner class

public class Ch5_3RectangleArea {
    
    
    
    /**
   You must complete this program so it calculates
   and displays the area of a rectangle. 
*/


   public static void main(String[] args)
   {
       
       
      // declare variables
      double length = 0.0, width = 0.0, area = 0.0;
   
      // Get the rectangle's length from the user.
      length = getLength();
   
      // Get the rectangle's width from the user.
      width = getWidth();

      // Get the rectangle's area.
      area = getArea(length, width);

      // Display the rectangle data.
      displayData(length, width, area);
   }
   
   /**
   * getLength() method
   * this method asks the user for the length of a rectangle
   * and returns that length as a double
   */
   public static double getLength()
   {
       
    System.out.print("\t \t \t ********** Rectangle Area **********\n\n");

    // prompts user to input length
     System.out.print("Enter the length of the rectangle: ");
     
          // creating a variable for scanner class

     Scanner userInput = new Scanner(System.in);
     
     // check to make sure the user entered a number
     if (!userInput.hasNextInt())
     {
      System.out.println("You did not enter a number!");
      System.exit(1);
     }
     
     // store the number entered by the user
     double result = userInput.nextInt();
     
     // return the number
     return result;
   }
   
   /**
    * getWidth() method
    * this method asks the user for the width of a rectangle
    * and returns that width as a double
    */
   public static double getWidth()
   {
     System.out.print("Enter the width of the rectangle: ");
     Scanner userInput = new Scanner(System.in);
     
     // check to make sure the user entered a number
      if (!userInput.hasNextInt())
      {
       System.out.println("You did not enter a number!");
       System.exit(1);
      }

      // store the number entered by the user
      double result = userInput.nextInt();

      // return the number
      return result;
   }
   
   /**
    * getArea() method
    * this method accepts two arguments of type double and multiplies them
    * it returns the result as a double
    */
   public static double getArea(double l, double w)
   {
     double result = l * w;
     return result;
   }
   
   /**
    * displayData() method
    * this method accepts 3 doubles as arguments and prints them with println()
    */
   public static void displayData(double l, double w, double a)
   {
     System.out.println("The length is: " + l);
     System.out.println("The width is: " + w);
     System.out.println("The area is: " + a);
   }
}
    
    
