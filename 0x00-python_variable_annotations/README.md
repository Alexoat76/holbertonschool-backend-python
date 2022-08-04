<p align="center">
<img src="https://img.shields.io/badge/LINUX-darkgreen.svg"/>
<img src="https://img.shields.io/badge/Shell-ligthgreen.svg"/>
<img src="https://img.shields.io/badge/Vim-green.svg"/>
<img src="https://img.shields.io/badge/Python-blue.svg"/>
<img src="https://img.shields.io/badge/Markdown-black.svg"/><br>	
</p>

---

# 0x00. Python - Variable Annotations

This project contains some tasks for learning how to use and implement *`Variable Annotations`* in *Python* language.

<p align="center">
  <img width="300"  
        src="https://media4.giphy.com/media/coxQHKASG60HrHtvkt/giphy.gif?cid=ecf05e47d3r74ql2puw2znfdxxwnruw6cpzyvqhczf94r1mj&rid=giphy.gif&ct=g"
  >
</p>

# Getting Started :running:	
<div style="text-align: justify">

## Table of Contents
* [About](#about)
* [Resources](#resources-books)
* [Requirements](#requirements)
* [Files](#files-file_folder)
* [Tasks](#tasks)
* [Credits](#credits)

## About

- [Advanced Python](https://intranet.hbtn.io/concepts/554)
- [Python 3 typing documentation](https://intranet.hbtn.io/rltoken/5XbVbzyPPe7ivdjVYMKlzg) 
- [MyPy cheat sheet](https://intranet.hbtn.io/rltoken/HYMdafJjNBrhPeMV9Fdj0A)

## Resources :books:
Read or watch:
	
[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/80px-Google_2015_logo.svg.png)](https://www.google.com/search?q=python+variable+type+annotation&bih=929&biw=1920&hl=en&ei=5xXsYrDYBdfKwbkP1POPkAw&oq=python+variableannotation&gs_lcp=Cgdnd3Mtd2l6EAEYATIGCAAQHhAHMgYIABAeEAcyCAgAEB4QCBAHMggIABAeEAgQBzIICAAQHhAIEAcyCAgAEB4QCBAHMggIABAeEAgQBzIICAAQHhAIEAcyCAgAEB4QCBAHMggIABAeEAgQDToHCAAQRxCwAzoHCAAQsAMQQzoECAAQDUoECEEYAEoECEYYAFCXCljgFWDsLmgBcAF4AIABgAGIAcQHkgEDMC44mAEAoAEByAEKwAEB&sclient=gws-wiz)

[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e1/Logo_of_YouTube_%282015-2017%29.svg/70px-Logo_of_YouTube_%282015-2017%29.svg.png)](https://www.youtube.com/results?search_query=python+variable+type+annotation)

## Requirements
### General
- Allowed editors: *` vi `*, *` vim `*, *` emacs `*.  
- All files will be interpreted on Ubuntu 20.04 LTS using *` python3 `*  (version 3.7)
- All files should end with a new line
- The first line of all files should be exactly  *` #!/usr/bin/env python3 `*
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the  *` pycodestyle `*  style (version 2.5.)
- All your files must be executable
- The length of your files will be tested using  *` wc `*
- All modules should have a documentation ( *` python3 -c 'print(__import__("my_module").__doc__)' `* )
- All classes should have a documentation ( *` python3 -c 'print(__import__("my_module").MyClass.__doc__)' `* )
- All functions (inside and outside a class) should have a documentation 
( *` python3 -c 'print(__import__("my_module").my_function.__doc__)' `*  and  
*` python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)' `* )
- A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, <br>
	class or method *(the length of it will be verified)*

## More Info
### Installation :computer:
	
- Clone this repository: `https://github.com/Alexoat76/holbertonschool-backend-python.git`	
- Access to directory: `cd 0x00-python_variable_annotations`
- `Compile` accord to `instructions` of each task.

## Files :file_folder:

### Tests :heavy_check_mark:

+ **[tests](./tests)**: Folder of test files. *`Provided by Holberton School`*.
		
---

## Tasks

+ [x] 0\. **Basic annotations - add**

+ **[0-add.py](./0-add.py)**

Write a type-annotated function   *` add `*   that takes a float   *` a `*   and a float  *` b `*   as arguments and returns their sum as a float.
 
```bash
$ cat 0-main.py
#!/usr/bin/env python3
add = __import__('0-add').add

print(add(1.11, 2.22) == 1.11 + 2.22)
print(add.__annotations__)

$ ./0-main.py
True
{'a':  <class 'float'>, 'b': <class 'float'>, 'return': <class 'float'>}

```
---

+ [x] 1\. **Basic annotations - concat**

+ **[1-concat.py](./1-concat.py)**

Write a type-annotated function   *` concat `*   that takes a string   *` str1 `*   and a string   *` str2 `*   as arguments and returns a concatenated string

```bash
$ cat 1-main.py
#!/usr/bin/env python3
concat = __import__('1-concat').concat

str1 = "egg"
str2 = "shell"

print(concat(str1, str2) == "{}{}".format(str1, str2))
print(concat.__annotations__)

$ ./1-main.py
True
{'str1': <class 'str'>, 'str2': <class 'str'>, 'return': <class 'str'>}

```
---

+ [x] 2\. **Basic annotations - floor**

+ **[2-floor.py](./2-floor.py)**

Write a type-annotated function   *` floor `*   which takes a float   *` n `*   as argument and returns the floor of the float.
```bash
$ cat 2-main.py
#!/usr/bin/env python3

import math

floor = __import__('2-floor').floor

ans = floor(3.14)

print(ans == math.floor(3.14))
print(floor.__annotations__)
print("floor(3.14) returns {}, which is a {}".format(ans, type(ans)))

$ ./2-main.py
True
{'n': <class 'float'>, 'return': <class 'int'>}
floor(3.14) returns 3, which is a <class 'int'>

```
---

+ [x] 3\. **Basic annotations - to string**

+ **[3-to_str.py](./3-to_str.py)**

Write a type-annotated function   *` to_str `*   that takes a float   *` n `*   as argument and returns the string representation of the float.

```bash
$ cat 3-main.py
#!/usr/bin/env python3
to_str = __import__('3-to_str').to_str

pi_str = to_str(3.14)
print(pi_str == str(3.14))
print(to_str.__annotations__)
print("to_str(3.14) returns {} which is a {}".format(pi_str, type(pi_str)))

$ ./3-main.py
True
{'n': <class 'float'>, 'return': <class 'str'>}
to_str(3.14) returns 3.14, which is a <class 'str'>

```
---


+ [x] 4\. **Define variables**

+ **[4-define_variables.py](./4-define_variables.py)**

Define and annotate the following variables with the specified values:
*  *` a `* , an integer with a value of **1**
*  *` pi `* , a float with a value of **3.14**
*  *` i_understand_annotations `* , a boolean with a value of **True**
*  *` school `* , a string with a value of **“Holberton”**

```bash
$ cat 4-main.py
#!/usr/bin/env python3

a = __import__('4-define_variables').a
pi = __import__('4-define_variables').pi
i_understand_annotations = __import__('4-define_variables').i_understand_annotations
school = __import__('4-define_variables').school

print("a is a {} with a value of {}".format(type(a), a))
print("pi is a {} with a value of {}".format(type(pi), pi))
print("i_understand_annotations is a {} with a value of {}".format(type(i_understand_annotations), i_understand_annotations))
print("school is a {} with a value of {}".format(type(school), school))

$ ./4-main.py
a is a <class 'int'> with a value of 1
pi is a <class 'float'> with a value of 3.14
i_understand_annotations is a <class 'bool'> with a value of True
school is a <class 'str'> with a value of Holberton

```
---

+ [x] 5\. **Complex types - list of floats**

+ **[5-sum_list.py](./5-sum_list.py)**

Write a type-annotated function   *` sum_list `*   which takes a list   *` input_list `*   of floats as argument and returns their sum as a float.

```bash
$ cat 5-main.py
#!/usr/bin/env python3

sum_list = __import__('5-sum_list').sum_list

floats = [3.14, 1.11, 2.22]
floats_sum = sum_list(floats)
print(floats_sum == sum(floats))
print(sum_list.__annotations__)
print("sum_list(floats) returns {} which is a {}".format(floats_sum, type(floats_sum)))

$ ./5-main.py
True
{'input_list': typing.List[float], 'return': <class 'float'>}
sum_list(floats) returns 6.470000000000001 which is a <class 'float'>

```
---

+ [x] 6\. **Complex types - mixed list**

+ **[6-sum_mixed_list.py](./6-sum_mixed_list.py)**

Write a type-annotated function   *` sum_mixed_list `*   which takes a list   *` mxd_lst `*   of integers and floats and returns their sum as a float.

```bash
$ cat 6-main.py
#!/usr/bin/env python3

sum_mixed_list = __import__('6-sum_mixed_list').sum_mixed_list

print(sum_mixed_list.__annotations__)
mixed = [5, 4, 3.14, 666, 0.99]
ans = sum_mixed_list(mixed)
print(ans == sum(mixed))
print("sum_mixed_list(mixed) returns {} which is a {}".format(ans, type(ans)))

$ ./6-main.py
{'mxd_lst': typing.List[typing.Union[int, float]], 'return': <class 'float'>}
True
sum_mixed_list(mixed) returns 679.13 which is a <class 'float'>

```
---

+ [x] 7\. **Complex types - string and int/float to tuple**

+ **[7-to_kv.py](./7-to_kv.py)**

Write a type-annotated function   *` to_kv `*   that takes a string   *` k `*   and an int OR float   *` v `*   as arguments and returns a tuple. 
The first element of the tuple is the string   *` k `*  . The second element is the square of the int/float   *` v `*   and should be annotated as a float.

```bash
$ cat 7-main.py
#!/usr/bin/env python3

to_kv = __import__('7-to_kv').to_kv

print(to_kv.__annotations__)
print(to_kv("eggs", 3))
print(to_kv("school", 0.02))

$ ./7-main.py
{'k': <class 'str'>, 'v': typing.Union[int, float], 'return': typing.Tuple[str, float]}
('eggs', 9)
('school', 0.0004)

```
---

+ [x] 8\. **Complex types - functions**

+ **[8-make_multiplier.py](./8-make_multiplier.py)**

Write a type-annotated function   *` make_multiplier `*   that takes a float   *` multiplier `*   as argument and returns a function that multiplies a float by   *` multiplier `*.

```bash
$ cat 8-main.py
#!/usr/bin/env python3

make_multiplier = __import__('8-make_multiplier').make_multiplier
print(make_multiplier.__annotations__)
fun = make_multiplier(2.22)
print("{}".format(fun(2.22)))

$ ./8-main.py
{'multiplier': <class 'float'>, 'return': typing.Callable[[float], float]}
4.928400000000001

```
---

+ [x] 9\. **Let's duck type an iterable object**

+ **[9-element_length.py](./9-element_length.py)**

Annotate the below function’s parameters and return values with the appropriate types

```
def element_length(lst):
    return [(i, len(i)) for i in lst]
``` 

```bash
$ cat 9-main.py 
#!/usr/bin/env python3

element_length =  __import__('9-element_length').element_length

print(element_length.__annotations__)

$ ./9-main.py 
{'lst': typing.Iterable[typing.Sequence], 'return': typing.List[typing.Tuple[typing.Sequence, int]]}

```
---

+ [x] 10\. **Duck typing - first element of a sequence**

+ **[100-safe_first_element.py](./100-safe_first_element.py)**

Augment the following code with the correct duck-typed annotations:

```bash
# The types of the elements of the input are not know
def safe_first_element(lst):
    if lst:
        return lst[0]
    else:
        return None
```

```bash
$ cat 100-main.py 
#!/usr/bin/env python3

safe_first_element =  __import__('100-safe_first_element').safe_first_element

print(safe_first_element.__annotations__)

$ ./100-main.py 
{'lst': typing.Sequence[typing.Any], 'return': typing.Union[typing.Any, NoneType]}

```
---

+ [x] 11\. **More involved type annotations**

+ **[101-safely_get_value.py](./101-safely_get_value.py)**

Given the parameters and the return values, add type annotations to the function

*` Hint `*: look into TypeVar

```bash
def safely_get_value(dct, key, default = None):
    if key in dct:
        return dct[key]
    else:
        return default
```
```bash
$ cat 101-main.py 
#!/usr/bin/env python3

safely_get_value = __import__('101-safely_get_value').safely_get_value
annotations = safely_get_value.__annotations__

print("Here's what the mappings should look like")
for k, v in annotations.items():
    print( ("{}: {}".format(k, v)))

$ ./101-main.py 
Here's what the mappings should look like
dct: typing.Mapping
key: typing.Any
default: typing.Union[~T, NoneType]
return: typing.Union[typing.Any, ~T]

```
---

+ [x] 12\. **Type Checking**

+ **[102-type_checking.py](./102-type_checking.py)**

Use   *` mypy `*   to validate the following piece of code and apply any necessary changes.

```bash
def zoom_array(lst: Tuple, factor: int = 2) -> Tuple:
    zoomed_in: Tuple = [
        item for item in lst
        for i in range(factor)
    ]
    return zoomed_in


array = [12, 72, 91]

zoom_2x = zoom_array(array)

zoom_3x = zoom_array(array, 3.0)

```

```bash
$ mypy 102-type_checking.py
Success: no issues found in 1 source file
```

```bash
$ cat 102-main.py 
#!/usr/bin/env python3

zoom_array =  __import__('102-type_checking').zoom_array

print(zoom_array.__annotations__)

$ ./102-main.py 
{'lst': typing.Tuple, 'factor': <class 'int'>, 'return': typing.List}

```
---

## Credits

## Author(s):blue_book:

Work is owned and maintained by 
	**`Alex Orland Arévalo Tribaldos`**  and credits for `group projects` are displayed in the respective `README.md` files.

<3915@holbertonstudents.com>
	
[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/Octicons-mark-github.svg/25px-Octicons-mark-github.svg.png)](https://github.com/Alexoat76)
[![M](https://upload.wikimedia.org/wikipedia/fr/thumb/c/c8/Twitter_Bird.svg/25px-Twitter_Bird.svg.png)](https://twitter.com/aoarevalot)
[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/c/ca/LinkedIn_logo_initials.png/25px-LinkedIn_logo_initials.png)](https://www.linkedin.com/in/Alexoat76/)

## Acknowledgments :mega: 

### **`Holberton School`** (*providing guidance*)
	
This program was written as part of the curriculum for Holberton School.
Holberton School is a campus-based full-stack software engineering program
that prepares students for careers in the tech industry using project-based
peer learning. For more information,  please visit [this link](https://www.holbertonschool.com/).
![Brand](https://assets.website-files.com/6105315644a26f77912a1ada/610540e8b4cd6969794fe673_Holberton_School_logo-04-04.svg)
