# 2024101027_ClassActivity2

In line1 , I put a colon after defining function to remove error.
Also in line3 and line4 , It should be a single equal to(=is correct  == is incorrect) as we are assigning the value and not comparing.
In line 6 , there must be 2 stars which indicates power and not 3 stars ( ** is correct and *** is incorrect).
In Line 10 where we define a function called print_narcis_numbers , we must put a comma(,) between start and end so as to indicate two arguements to the function.
In Line 12 and 13 , we need to put a colon after for loop and also the if condition for proper syntax.
Also in Line 13 , the name of the function is wrong , so I corrected it to the one defined above.
In Line 16 , the function called again is of wrong name , I corrected it to the one defined above.


# Corrected Code

def is_narc(n):
    """Check if a number is narc."""
    num_str = str(n)
    num_digits = len(num_str)
    
    sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)
    
    return sum_of_powers == n

def print_narcis_numbers(start,end):
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1):
        if is_narc(num):
            print(num)

print_narcis_numbers(1000, 10000)


Output is 1634.


