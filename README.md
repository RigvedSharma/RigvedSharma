/* Currency Converter 
 * Example of menu driven programs
*/
import java.util.*;
public class Currency_Converter
{
     public static void main(String[] args) 
     {
        // declaration
        Scanner sc = new Scanner (System.in);
        int originalcurrency;
        double convertedcurrency;
        byte choice;
        //Process
        System.out.println("Enter the value in Indian Ruppees to be converted");
        originalcurrency = sc.nextInt();
        System.out.println("Enter 1 for conversion to dollars, 2 for conversion to euros, 3 for converion to dirhams, 4 for conversion to pounds and 5 for conversion to kuwaiti dinar");
        choice = sc.nextByte();
        switch (choice)
        {
            case 1: System.out.println("Conversion from Ruppees to US Dollars");
                    convertedcurrency = originalcurrency/82.90;                                                   // 1 dollar = 82.90 ruppees
                    System.out.println(originalcurrency+" ruppees converts to "+convertedcurrency+" dollars");
                    break;

            case 2: System.out.println("Conversion from Ruppees to Euros");
                    convertedcurrency = originalcurrency/90;                                                      // 1 euro = 90 ruppees
                    System.out.println(originalcurrency+" ruppees converts to "+convertedcurrency+" Euros"); 
                    break;

            case 3: System.out.println("Conversion from Ruppees to UAE Dirhams");
                    convertedcurrency = originalcurrency/22.57;                                                   // 1 dirham = 22.57 ruppees
                    System.out.println(originalcurrency+" ruppees converts to "+convertedcurrency+" dirhmas");
                    break;

            case 4: System.out.println("Conversion from Ruppees to British pounds");
                    convertedcurrency = originalcurrency/105.06;                                                  // 1 pound = 105.06 ruppees
                    System.out.println(originalcurrency+" ruppees converts to "+convertedcurrency+" pounds");
                    break;

            case 5: System.out.println("Conversion from Ruppees to Kuwaiti Dinar");
                    convertedcurrency = originalcurrency/269.51;                                                  // 1 dollar = 269.51 ruppees
                    System.out.println(originalcurrency+" ruppees converts to "+convertedcurrency+" dinars"); 
                    break;

            default: System.out.println("Incorrect Input, Try Again!!");
            
        }
     }
     sc.close()
    
}
