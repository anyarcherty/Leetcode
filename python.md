# Python

1. reverse str, list
  
   `res = res[::-1]` res = 'abc', return 'cba'
   
   `lst = lst[::-1]` lst = ['a', 'b', 'c'] return ['c', 'b', 'a']

2. severse int
   
    ```
    res = int(str(abs(x))[::-1])
    if x < 0:
        return -res
    else
        return res
    ```
3. subset 
    
    set() provides classes for constructing and manipulating unordered collections of unique elements
    
    `{0, 1}.issubset({0, 1, 2}) return True`
    
    `{1}.issubset({'A', 'B', 'C'}) return False`

4. string handling

   `str.isalpha()` return True if all character in the string are alphabets. Otherwise return False
   
   `str..isdigit()` return True if all character is number. otherwise return False
   
5. remove all same value in list

   `list(filter(lambda x: x!=0, nums))` remove 0 in nums list
     
6. eval()
    
    The `eval()` function evaluates or executes an argument. If the argument is a string and with number and expression, it will return expression result
    
    `eval('2+3')` return 5

7. string upper and lower

    `str.lower()` return all lowercase string
    
    `str.upper()` return all uppercase string

8. str to lst

    `lst_s =[x for x in s]`
  
    `lst_s = list(s)`

9. all alphbetic character in list

    `[chr(i) for i in range(ord('a'),ord('z')+1)]`
    
    ```
    import string
    
    ascii_letters = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
    ascii_lowercase = 'abcdefghijklmnopqrstuvwxyz'
    ascii_uppercase = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
    digits = '0123456789'
    hexdigits = '0123456789abcdefABCDEF'
    octdigits = '01234567'
    printable = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ \t\n\r\x0b\x0c'
    punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
    whitespace = ' \t\n\r\x0b\x0c'
    ```
    
10. list running time
    
    ```
    
    `len(list)` is an `O(1)` operation
    
    `append(list)` is an `O(1)` operation
    
    `set(list)` is an `O(1)` operation
    
    `list.pop(index)` is an `O(index)` operation, `list.pop(0)` is an `O(1)` operation
    
    `max(list)` or `min(list)` is an `O(n)` operation 
    
    `delete(list)` is an `O(n)` operation
    
    `iternation` is an `O(n)` operation
    
    `x in list` is `O(n)` operation
    
    ```
    
11. set add and list append

    `set.add()` is far `fast` than `lst.append()`

12. 32bits
    
    `'{0:032b}'.format(x)` return len of 32 format for bits
    
    `int({0:032b}'.format(x), 2)` return int from binary

12 binary to int

   `int('1010', 2)` return 10
   
   `bin(10)` return 1010
    
13. sorted(list) vs list.sort()

    `list.sort` mutates `the list` in-place & returns None. Modify the raw list!
    
    `sorted(list)` takes any iterable & returns a `new list`, sorted. Do not modify the raw list!

    `sorted(list, reverse=Ture)` get the reverse order of list
    
14. list.append(lst) vs list.extend(lst)

    `append` adds its argument as a `single element` to the end of a list
    
    `extend` iterates over its argument adding `each element` to the list

15. str.strip()

    `str.strip()` with no arguments (or None as the first argument) `remove all whitespace` at the start and end, including `spaces`, `tabs`, `newline`s and `carriage returns`

16. list[:]

    It takes a copy of the tuple, instead of a reference to the tuple itself.

    The [:] syntax is a slice with the default start and end values (0 and the length of the list), returning a new tuple with those indices, so effectively an exact copy of the contents

17. list.count(value)

    ```
    lst = [1,1,2,3,4,1,1]
    
    lst.count(1) return 3
    ```

18. dict.update()

    append new key/value in dict
    ```
    dic = {}
    
    dic.update({a: 1})
    
    dic return {a: 1}
    
    dic.update({b: 2})
    
    dic return {a: 1, b: 2}
    ```
    
19. sort dict
    
    ```
    Sort dict by key
    mydict = {'carl':40,
              'alan':2,
              'bob':1,
              'danny':3}

    for key in sorted(mydict.iterkeys()):
        print "%s: %s" % (key, mydict[key])
    ```
    
    ```
    sort dict by value
    for key, value in sorted(mydict.iteritems(), key=lambda (k,v): (v,k)):
        print "%s: %s" % (key, value)
    ```

20. Python's slice notation
    
    `sliceable[start:stop:step]` 
    
    ```
    lst = [1,2,3,4,5,6]
    lst[:2] = [1,2]
    lst[::2] = [1,3,5]
    lst[:2:2] = [1]
    lst[2::3] = [3, 6]
    ```
    
21. bitwise operators
    
    `&` `a & b` 
    
    bitwise and, each bit position in the result is the logical `And` of the bits in the corresponding position of the operands. 
    
    Each bit of the output is 1 if the corresponding bit of x and of y is 1, otherwise is 0
