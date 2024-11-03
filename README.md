PrimeNumberFinder

This project is a simple Java program designed to find and display all prime numbers between 1 and 1000. A prime number is a number that has no divisors other than 1 and itself. This program includes a method to check if a number is prime and uses this method to identify all primes in the specified range.
Project Structure

    PrimeNumberFinder.java: Contains the main method that iterates from 1 to 1000, as well as the isPrime method, which checks if a number is prime.

Code Overview
Methods

    main Method
        Functionality: Iterates through numbers from 1 to 1000 and calls isPrime for each number. If a number is prime, it is printed to the console.

    isPrime(int number)
        Description: Checks if a given number is prime.
        Parameters: int number - the number to check for primality.
        Returns: boolean - true if the number is prime, false otherwise.
        Logic:
            If number is less than or equal to 1, it is not prime.
            For numbers greater than 1, the method checks divisibility from 2 up to the square root of the number (for optimization). If the number is divisible by any integer in this range, it is not prime.

Usage

Expected output (first few primes):

    Prime numbers between 1 and 1000:
    2 3 5 7 11 13 17 19 23 29 ... 997

Key Concepts

    Prime Number: A number that has exactly two divisors: 1 and itself.
    Optimization with Square Root: Instead of checking divisibility up to number - 1, we only check up to the square root of number, which reduces the number of operations and improves efficiency.

Author

This project is an educational example for finding prime numbers in a given range in Java.


