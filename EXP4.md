# Ex.No: 4 check the given number is Armstrong number or not and inspect for failures.
### DATE:                                                                            
### REGISTER NUMBER: 212222040178
### AIM: 
Write a python program to check the number is Armstrong number or not and inspect for failures.

### Algorithm:
1.  Start the program.
2.	Read an integer input number.
3.	Initialize the variables current_digit, sum = 0, and num = number.
4.	Repeat Steps 5 to 7 until num > 0
5.	current_digit = (num % 10).
6.	sum = sum + (current_digit * current_digit * current_digit). 7. Stop the program.
7.	num = num / 10.
8.	Check if sum == number. If true, print "It is an Armstrong Number." Otherwise, print "It is not an Armstrong Number."
9.	Stop the program.

### Program:

```
def is_armstrong(number):
    num_str = str(number)
    num_digits = len(num_str)
    sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)
    return sum_of_powers == number

try:
    number = int(input("Enter a number: "))
    if is_armstrong(number):
        print(f"{number} is an Armstrong number.")
    else:
        print(f"{number} is not an Armstrong number.")
except ValueError:
    print("Invalid input. Please enter an integer.")

```

### Output:

![stl exp4 c](https://github.com/user-attachments/assets/2fe05eb5-1146-44bd-829e-9b01edd91b7d)


![stl exp4 t](https://github.com/user-attachments/assets/66a1e2cd-be98-4bbb-aaa2-5323a9720f3a)



### Result:
Thus, the python program to check the number is Armstrong number or not implemented and the output is verified successfully.


