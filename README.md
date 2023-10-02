# Python Exercises, Practice Questions and Solutions

## Python List Exercises


| Program Description                             |
|-------------------------------------------------|
| Interchange first and last elements in a list   |
| Swap two elements in a list                     |
| Swap elements in a String list                  |
| Ways to find the length of a list               |
| Maximum of two numbers in Python               |
| Minimum of two numbers in Python               |
| Reversing a List                                |
| Cloning or Copying a list                      |
| Count occurrences of an element in a list      |
| Find sum and average of List in Python         |
| Sum of number digits in List                   |
| Multiply all numbers in the list               |
| Find the smallest number in a list             |
| Find the largest number in a list              |
| Find the second largest number in a list       |
| Print even numbers in a list                   |
| Print odd numbers in a List                    |
| Print all even numbers in a range              |
| Print all odd numbers in a range               |
| Count Even and Odd numbers in a List           |
| Print positive numbers in a list               |
| Print negative numbers in a list               |
| Print all positive numbers in a range          |
| Print all negative numbers in a range          |
| Count positive and negative numbers in a list  |
| Remove multiple elements from a list in Python |
| Remove empty tuples from a list                |
| Program to print duplicates from a list of integers |
| Remove empty List from List                    |
| Convert List to List of dictionaries           |
| Convert Lists of List to Dictionary            |
| Uncommon elements in Lists of List             |
| Select Random value from list of lists         |
| Reverse Row sort in Lists of List              |
| Pair elements with Rear element in Matrix Row   |

# Answer :


1. Python program to interchange the first and last elements in a list:

```python
def interchange_first_last(lst):
    if len(lst) < 2:
        return lst

    lst[0], lst[-1] = lst[-1], lst[0]
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
interchanged_list = interchange_first_last(my_list)
print(interchanged_list)
```

2. Python program to swap two elements in a list:

```python
def swap_elements(lst, index1, index2):
    if 0 <= index1 < len(lst) and 0 <= index2 < len(lst):
        lst[index1], lst[index2] = lst[index2], lst[index1]
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
swap_elements(my_list, 1, 3)
print(my_list)
```

3. Python program to swap elements in a String list:

```python
def swap_elements_string_list(lst, index1, index2):
    if 0 <= index1 < len(lst) and 0 <= index2 < len(lst):
        lst[index1], lst[index2] = lst[index2], lst[index1]
    return lst

# Example usage:
string_list = ["apple", "banana", "cherry", "date"]
swap_elements_string_list(string_list, 1, 3)
print(string_list)
```

4. Python program to find the length of a list:

```python
def find_length_of_list(lst):
    return len(lst)

# Example usage:
my_list = [1, 2, 3, 4, 5]
length = find_length_of_list(my_list)
print("Length of the list:", length)
```

5. Python program to find the maximum of two numbers:

```python
def find_maximum(a, b):
    return max(a, b)

# Example usage:
num1 = 10
num2 = 20
maximum = find_maximum(num1, num2)
print("Maximum:", maximum)
```

6. Python program to find the minimum of two numbers:

```python
def find_minimum(a, b):
    return min(a, b)

# Example usage:
num1 = 10
num2 = 20
minimum = find_minimum(num1, num2)
print("Minimum:", minimum)
```

7. Python program to reverse a list:

```python
def reverse_list(lst):
    return lst[::-1]

# Example usage:
my_list = [1, 2, 3, 4, 5]
reversed_list = reverse_list(my_list)
print(reversed_list)
```

8. Python program to clone or copy a list:

```python
def clone_list(lst):
    return lst.copy()

# Example usage:
original_list = [1, 2, 3, 4, 5]
copied_list = clone_list(original_list)
print(copied_list)
```

9. Python program to count occurrences of an element in a list:

```python
def count_occurrences(lst, element):
    return lst.count(element)

# Example usage:
my_list = [1, 2, 2, 3, 4, 2, 5]
element_to_count = 2
occurrences = count_occurrences(my_list, element_to_count)
print(f"{element_to_count} occurs {occurrences} times in the list.")
```

10. Python program to find the sum and average of a list:

```python
def sum_and_average(lst):
    if len(lst) == 0:
        return 0, 0  # Handle empty list

    list_sum = sum(lst)
    list_average = list_sum / len(lst)
    return list_sum, list_average

# Example usage:
my_list = [1, 2, 3, 4, 5]
total_sum, average = sum_and_average(my_list)
print(f"Sum: {total_sum}, Average: {average}")
```

11. Python program to find the sum of the digits in a list of numbers:

```python
def sum_of_digits_in_list(lst):
    return sum(int(digit) for num in lst for digit in str(num))

# Example usage:
my_list = [123, 45, 678]
digit_sum = sum_of_digits_in_list(my_list)
print("Sum of digits:", digit_sum)
```

12. Python program to multiply all numbers in a list:

```python
def multiply_all_numbers(lst):
    result = 1
    for num in lst:
        result *= num
    return result

# Example usage:
my_list = [1, 2, 3, 4, 5]
product = multiply_all_numbers(my_list)
print("Product of all numbers:", product)
```

13. Python program to find the smallest number in a list:

```python
def find_smallest_number(lst):
    if len(lst) == 0:
        return None  # Handle empty list
    return min(lst)

# Example usage:
my_list = [10, 2, 45, 7, 1]
smallest = find_smallest_number(my_list)
print("Smallest number:", smallest)
```

14. Python program to find the largest number in a list:

```python
def find_largest_number(lst):
    if len(lst) == 0:
        return None  # Handle empty list
    return max(lst)

# Example usage:
my_list = [10, 2, 45, 7, 1]
largest = find_largest_number(my_list)
print("Largest number:", largest)
```

15. Python program to find the second largest number in a list:

```python
def find_second_largest_number(lst):
    if len(lst) < 2:
        return None  # Handle insufficient elements
    sorted_list = sorted(lst, reverse=True)
    return sorted_list[1]

# Example usage:
my_list = [10, 2, 45, 7, 1]
second_largest = find_second_largest_number(my_list)
print("Second largest number:", second_largest)
```

16. Python program to print even numbers in a list:

```python
def print_even_numbers(lst):
    for num in lst:
        if num % 2 == 0:
            print(num)

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
print("Even numbers:")
print_even_numbers(my_list)
```

17. Python program to print odd numbers in a list:

```python
def print_odd_numbers(lst):
    for num in lst:
        if num % 2 != 0:
            print(num)

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
print("Odd numbers:")
print_odd_numbers(my_list)
```

18. Python program to print all even numbers in a range:

```python
def print_even_numbers_in_range(start, end):
    for num in range(start, end + 1):
        if num % 2 == 0:
            print(num)

# Example usage:
start = 1
end = 10
print("Even numbers in the range:")
print_even_numbers_in_range(start, end)
```

19. Python program to print all odd numbers in a range:

```python
def print_odd_numbers_in_range(start, end):
    for num in range(start, end + 1):
        if num % 2 != 0:
            print(num)

# Example usage:
start = 1
end = 10
print("Odd numbers in the range:")
print_odd_numbers_in_range(start, end)
```

20. Python program to count even and odd numbers in a list:

```python
def count_even_and_odd_numbers(lst):
    even_count = 0
    odd_count = 0
    for num in lst:
        if num % 2 == 0:
            even_count += 1
        else:
            odd_count += 1
    return even_count, odd_count

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
even, odd = count_even_and_odd_numbers(my_list)
print(f"Even numbers: {even}, Odd numbers: {odd}")
```

21. Python program to print positive numbers in a list:

```python
def print_positive_numbers(lst):
    for num in lst:
        if num > 0:
            print(num)

# Example usage:
my_list = [-1, 2, -3, 4, 5, -6]
print("Positive numbers:")
print_positive_numbers(my_list)
```

22. Python program to print negative numbers in a list:

```python
def print_negative_numbers(lst):
    for num in lst:
        if num < 0:
            print(num)

# Example usage:
my_list = [-1, 2, -3, 4, 5, -6]
print("Negative numbers:")
print_negative_numbers(my_list)
```

23. Python program to print all positive numbers in a range:

```python
def print_positive_numbers_in_range(start, end):
    for num in range(start, end + 1):
        if num > 0:
            print(num)

# Example usage:
start = -5
end = 5
print("Positive numbers in the range:")
print_positive_numbers_in_range(start, end)
```

24. Python program to print all negative numbers in a range:

```python
def print_negative_numbers_in_range(start, end):
    for num in range(start, end + 1):
        if num < 0:
            print(num)

# Example usage:
start = -5
end = 5
print("Negative numbers in the range:")
print_negative_numbers_in_range(start, end)
```

25. Python program to count positive and negative numbers in a list:

```python
def count_positive_and_negative_numbers(lst):
    positive_count = sum(1 for num in lst if num > 0)
    negative_count = sum(1 for num in lst if num < 0)
    return positive_count, negative_count

# Example usage:
my_list = [-1, 2, -3, 4, 5, -6]
positive, negative = count_positive_and_negative_numbers(my_list)
print(f"Positive numbers: {positive}, Negative numbers: {negative}")
```

26. Remove multiple elements from a list in Python:

To remove multiple elements from a list, you can use list comprehension. Here's an example that removes elements based on a condition:

```python
my_list = [1, 2, 3, 4, 5, 6]
elements_to_remove = [2, 4, 6]
my_list = [x for x in my_list if x not in elements_to_remove]
print(my_list)
```

27. Python program to remove empty tuples from a list:

```python
def remove_empty_tuples(lst):
    return [tup for tup in lst if tup]

# Example usage:
my_list = [(1, 2), (), (3, 4), (), (5, 6)]
filtered_list = remove_empty_tuples(my_list)
print(filtered_list)
```

28. Python program to print duplicates from a list of integers:

```python
def find_duplicates(lst):
    seen = set()
    duplicates = set()
    for num in lst:
        if num in seen:
            duplicates.add(num)
        else:
            seen.add(num)
    return list(duplicates)

# Example usage:
my_list = [1, 2, 2, 3, 4, 4, 5, 6]
duplicates = find_duplicates(my_list)
print("Duplicate elements:", duplicates)
```
