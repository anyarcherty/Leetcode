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
     
