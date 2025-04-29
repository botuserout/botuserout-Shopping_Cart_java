# 🛍️💱 Java Shopping Cart + Currency Converter  
### A Beginner-Friendly Java Project Using Arrays 📚

---------------------------------------------------------------------------------------------------------------------------------------------------------

Welcome to the **Java Shopping Cart Currency Converter** – a fun and educational project that simulates a global shopping experience! 🌐💸 With just a few inputs, you can find out how much your international shopping spree will cost you in INR 🇮🇳.

This updated version uses **arrays** to handle currency data more efficiently — taking your Java learning to the next level! 🚀

**---------------------------------------------------------------------------------------------------------------------------------------------------------**

## ✅ What This Project Does

This Java console app lets the user:

🛒 Enter a product to buy  
🔢 Input the quantity of items  
💵 Enter the price in foreign currency  
🌍 Choose the currency (USD, EUR, GBP)  
💰 See the **converted price in INR**  
📦 Get a summary of their total bill

---

## 🧠 Key Concepts Demonstrated

| 💡 Concept                | ✅ Used in Code                    |
|--------------------------|------------------------------------|
| Scanner for input        | ✔️ `Scanner sc = new Scanner(...)` |
| Conditional logic        | ✔️ `if-else` for input validation   |
| Arithmetic operations    | ✔️ Multiplying price and quantity  |
| Arrays (DSA intro)       | ✔️ `String[]`, `double[]` used     |
| Index-based selection    | ✔️ Dynamic lookup using arrays     |

---

### 🔁 Arrays Used for Currency Mapping

Instead of using repeated `if-else` conditions, we now store the currencies and their conversion rates in **parallel arrays**:

```java
String[] currencies = {"USD", "EUR", "GBP"};
double[] conversionRates = {82.0, 90.0, 98.0};
```

When the user selects a currency, we map their choice directly using:
```java
int index = choice - 1;
convertedAmount = price * conversionRates[index];
```

This is a **classic example of using arrays for clean logic** and is a stepping stone to more advanced structures like `HashMap` or custom `Currency` classes!

---

## 🖥️ Sample Output

```bash
What item would you like to buy: Headphones

How much quantity do you want: 2
Enter the amount of item in worldwide currency:
100
In which currency are you purchasing the product?
1. USD
2. EUR
3. GBP
1
100.0 USD is equal to 8200.0 INR

Thanks for shopping from our store!
Here is your item: Headphones
Quantity purchased: 2
Your total bill is: 16400.0 INR
```

---

🎯 Why This Project Rocks
- ✅ **Perfect for Java beginners** 🚀  
- ✅ Introduces basic **Data Structures (Arrays)** 🧠  
- ✅ Simulates a **real-world scenario** (currency conversion + billing)  
- ✅ Lightweight, fast, and runs in any Java IDE or terminal 💻  

---------------------------------------------------------------------------------------------------------------------------------------------------------

💡 How to Run

1. Copy the code into a `.java` file (e.g., `Main.java`)
2. Compile:  
   javac Main.java
3. Run:  
   java Main
   

---------------------------------------------------------------------------------------------------------------------------------------------------------

## ⭐ Bonus Learning Tip

Want to improve this further?
🔁 Try using a `HashMap<String, Double>` for dynamic currency lookups  
📦 Wrap currency logic into a separate method or class  
🧪 Add more currencies (like JPY, AUD) just by updating the arrays!

------------------------------------------------------------------------------------------------------------------------------------------------------------

## ❤️ Final Words

This project blends **logic + math + a real use case** – the perfect combo for aspiring Java devs!  
If you enjoyed it, ⭐️ star the repo, fork it, and build your own upgrades!

Happy coding! 🧑‍💻🧑‍🏫  
*Made with Java & Love 💖*

