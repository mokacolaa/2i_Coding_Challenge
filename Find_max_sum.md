# Assumptions:
- Each sigit is a single character between 0-9
- Strings may contain characters and no digits
- Non digit characters will output no value

```python
def max_digit_sum:
  max_sum = 0
  for s in strings:
      digit_sum = sum(int(c) for c in s if c.isdigit())
      max_sum = max(max_sum, digit_sum)
  return max_sum

if __name__ == "__main__":
  input_strings = ["dh7js4jf", "or2rjvn2w", "h1n36mfl", "a7e6fw"]
  result = max_digit_sum(input_strings)
  print ("maximum digit sum is:", result)
 ``` 
