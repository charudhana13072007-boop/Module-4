## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
~~~


dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'c': 4, 'd': 5, 'e': 6}


def merge(d1, d2):
    return {**d1, **d2}   # unpacking operator

merged_dict = merge(dict1, dict2)
print("Merged dictionary:", merged_dict)
~~~

## Output
Merged dictionary: {'a': 1, 'b': 2, 'c': 4, 'd': 5, 'e': 6}


## Result
The program successfully merges two dictionaries. If a key exists in both dictionaries (like 'c'), the value from the second dictionary (dict2) overwrites the value from the first (dict1).
