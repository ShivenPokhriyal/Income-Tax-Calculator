# Income-Tax-Calculator
This Java program calculates the income tax based on predefined tax brackets. The current implementation uses a simple structure with three income ranges and corresponding tax rates. 




        import java.util.* ;
        
        public class IncomeTaxCalculator {
        public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        int income = sc.nextInt();   
        int tax = 0;
        
        if (income < 500000) {
            tax = 0;
        } else if (income >= 500000 && income < 1000000) {
            tax = (int) (income * 0.2);

        } else {
            tax = (int) (income * 0.3);

        }
        System.out.println("Your tax is : " + tax);
    }
    }
