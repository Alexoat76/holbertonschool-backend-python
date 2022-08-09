<p align="center">
<img src="https://img.shields.io/badge/LINUX-darkgreen.svg"/>
<img src="https://img.shields.io/badge/Shell-ligthgreen.svg"/>
<img src="https://img.shields.io/badge/Vim-green.svg"/>
<img src="https://img.shields.io/badge/Python-blue.svg"/>
<img src="https://img.shields.io/badge/Markdown-black.svg"/><br>	
</p>

---

# 0x02. Python - Async Comprehension

This project contains some tasks for learning how to use and implement *`Asynchronous Comprehensions / Generators`* in *Python* language.

<p align="center">
  <img width="500"
        src="https://files.realpython.com/media/A-Complete-Walkthrough-of-Pythons-Asyncio_Watermarked.5b6b9a01fdc9.jpg"
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


## Resources :books:
Read or watch:
	
[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/80px-Google_2015_logo.svg.png)](https://www.google.com/search?q=python+concurrent+coroutines&oq=concurrent+coro&aqs=chrome.2.69i57j0i512j0i22i30l4j0i15i22i30.9365j0j15&sourceid=chrome&ie=UTF-8)

[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e1/Logo_of_YouTube_%282015-2017%29.svg/70px-Logo_of_YouTube_%282015-2017%29.svg.png)](https://www.youtube.com/results?search_query=Coroutine+Concurrency+in+Python+3+with+asyncio)

## Requirements
### General
* A  *` README.md `*  file, at the root of the folder of the project, is mandatory
* Allowed editors:  *` vi `* ,  *` vim `* ,  *` emacs `* 
* All files will be interpreted/compiled on Ubuntu 18.04 LTS using  *` python3 `*  (version 3.7)
* All files should end with a new line
* All files must be executable
* The length of files will be tested using  *` wc `* 
* The first line of all files should be exactly  *` #!/usr/bin/env python3 `* 
* The code should use the  *` pycodestyle `*  style (version 2.5.x)
* All functions and coroutines must be type-annotated.
* All modules should have a documentation ( *` python3 -c 'print(__import__("my_module").__doc__)' `* )
* All functions should have a documentation ( *` python3 -c 'print(__import__("my_module").my_function.__doc__)' `*
* A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method <br>
	(the length of it will be verified)

## More Info
### Installation :computer:
	
- Clone this repository: `https://github.com/Alexoat76/holbertonschool-backend-python.git`	
- Access to directory: `cd 0x02-python_async_comprehension`
- `Compile` accord to `instructions` of each task.

## Files :file_folder:

### Tests :heavy_check_mark:

+ **[tests](./tests)**: Folder of test files. *`Provided by Holberton School`*.
		
---

## Tasks

+ [x] 0\. **The basics of async**

+ **[0-basic_async_syntax.py](./0-basic_async_syntax.py)**

Write an asynchronous coroutine that takes in an integer argument ( *` max_delay `* , with a default value of 10) named  *` wait_random `*  that waits for a random delay 
between 0 and  *` max_delay `* (included and float value) seconds and eventually returns it.

Use the   *` random `*   module.

```bash
$ cat 0-main.py
#!/usr/bin/env python3

import asyncio

wait_random = __import__('0-basic_async_syntax').wait_random

print(asyncio.run(wait_random()))
print(asyncio.run(wait_random(5)))
print(asyncio.run(wait_random(15)))

$ ./0-main.py
9.034261504534394
1.6216525464615306
10.634589756751769

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
