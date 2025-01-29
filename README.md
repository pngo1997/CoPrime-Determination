# Coprime Checker 🔢

## 📜 Overview
This project determines whether two integers are **coprime**, meaning they share no common divisors except 1.  
The program continuously asks the user for input until they choose to exit.

## 🎯 Features
- **Automated Check:** Determines if two numbers are coprime using the **greatest common divisor (GCD)**.
- **Interactive Mode:** Users can enter multiple pairs and receive immediate feedback.
- **Loop Until Exit:** Runs until the user opts to stop.

## 🛠 How It Works
1. The `coprime_test_loop()` function:
   - Prompts the user for two numbers.
   - Passes them to `coprime(a, b)`, which returns **True** if coprime, otherwise **False**.
   - Displays the result and prompts for another pair.
   - The loop continues until the user chooses to exit.

2. The `coprime(a, b)` function:
   - Uses the **Euclidean Algorithm** (`math.gcd(a, b) == 1`) to check coprimality.

## 📝 Sample Output
```shell
Enter first number: 14
Enter second number: 25
✅ The numbers 14 and 25 are coprime.

Enter first number: 12
Enter second number: 18
❌ The numbers 12 and 18 are NOT coprime.

Do you want to check another pair? (yes/no): no
