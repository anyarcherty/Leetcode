# Python

1. Reverse Str
  
   `res = res[::-1]`

2. Reverse Int
   
    ```
    res = int(str(abs(x))[::-1])
    if x < 0:
        return -res
    else
        return res
    ```
3. Subset 
    
    set() provides classes for constructing and manipulating unordered collections of unique elements
    
    `{0, 1}.issubset({0, 1, 2}) return True`
    
    `{1}.issubset({'A', 'B', 'C'}) return False`

4. Srting handling

   `str.isalpha()` return True if all character in the string are alphabets. Otherwise return False
   
   `str..isdigit()` return True if all character is number. otherwise return False
   
5. remove all same value in list

   `list(filter(lambda x: x!=0, nums))` remove 0 in nums list
     
6. eval()
    
    The `eval()` function evaluates or executes an argument. If the argument is a string and with number and expression, it will return expression result
    
    `eval('2+3')` return 5
