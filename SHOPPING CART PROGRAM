import java.util.*;

// SHOPPING CART PROGRAM using arrays for currency selection
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String item;
        double price;
        int quantity;
        double total;

        // Currency names and corresponding INR conversion rates (parallel arrays)
        String[] currencies = {"USD", "EUR", "GBP"};
        double[] conversionRates = {82.0, 90.0, 98.0};

        // Input item name
        System.out.print("What item would you like to buy: ");
        item = sc.nextLine();

        // Input quantity
        System.out.print("\nHow much quantity do you want: ");
        quantity = sc.nextInt();

        // Input price in foreign currency
        System.out.println("Enter the amount of item in worldwide currency:");
        price = sc.nextDouble();
        sc.nextLine(); // Consume newline left-over

        // Show currency options from array
        System.out.println("In which currency are you purchasing the product?");
        for (int i = 0; i < currencies.length; i++) {
            System.out.println((i + 1) + ". " + currencies[i]);
        }

        int choice = sc.nextInt();

        double convertedAmount = 0.0;

        if (choice >= 1 && choice <= currencies.length) {
            int index = choice - 1;
            convertedAmount = price * conversionRates[index];
            System.out.println(price + " " + currencies[index] + " is equal to " + convertedAmount + " INR");
        } else {
            System.out.println("Invalid choice. Please select a valid currency.");
            sc.close();
            return;
        }

        // Calculate total cost
        total = convertedAmount * quantity;

        // Output bill summary
        System.out.println("\nThanks for shopping from our store!");
        System.out.println("Here is your item: " + item);
        System.out.println("Quantity purchased: " + quantity);
        System.out.println("Your total bill is: " + total + " INR");

        sc.close();
    }
}
