# Assumptions:

- Each sigit is a single character between 0-9
- Strings may contain characters and no digits
- Non digit characters will output no value

# Functionality 

```python
def max_digit_sum(strings):
  max_sum = 0
# Loop through each string in the input list
  for s in strings:
# Sum all characters that are digits (int(c) converts digits to integers before addition)
      digit_sum = sum(int(c) for c in s if c.isdigit())
# Update max_sum if current digit_sum string is higher
      max_sum = max(max_sum, digit_sum)
# Return highest digit sum
  return max_sum

# Runs only when file executed directly
if __name__ == "__main__":
# Example used in main question
  input_strings = ["dh7js4jf", "or2rjvn2w", "h1n36mfl", "a7e6fw"]
# Call function with the example used
  result = max_digit_sum(input_strings)
# Print results
  print ("maximum digit sum is:", result)
 ``` 
