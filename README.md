# Python Exercises, Practice Questions and Solutions

## Python List Exercises

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

