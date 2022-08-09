<p align="center">
<img src="https://img.shields.io/badge/LINUX-darkgreen.svg"/>
<img src="https://img.shields.io/badge/Shell-ligthgreen.svg"/>
<img src="https://img.shields.io/badge/Vim-green.svg"/>
<img src="https://img.shields.io/badge/Python-blue.svg"/>
<img src="https://img.shields.io/badge/Markdown-black.svg"/><br>	
</p>

---

# 0x02. Python - Async Comprehension

This project contains some tasks for learning how to use and implement **`Asynchronous Comprehensions / Generators`** in *Python* language.

<p align="center">
  <img width="300"
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

- **[PEP 530 – Asynchronous Comprehensions](https://intranet.hbtn.io/rltoken/92LFCh7ZO9-ousmsmxCcEw)**
- **[What’s New in Python: Asynchronous Comprehensions / Generators](https://intranet.hbtn.io/rltoken/bOGIzGlugH-SxS3xuFDvEA)**
- **[Type-hints for generators](https://intranet.hbtn.io/rltoken/Tk9Qhv_ZgzGdoQJJN0O20g)** 
- How to write an asynchronous generator
- How to use async comprehensions
- How to type-annotate generators

## Resources :books:
Read or watch:
	
[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/80px-Google_2015_logo.svg.png)](https://www.google.com/search?q=Python+-+Async+Comprehension+gif&source=lmns&bih=929&biw=1903&hl=en&sa=X&ved=2ahUKEwi7g7CKhLr5AhWLA98KHfh4A4YQ_AUoAHoECAEQAA)

[![M](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e1/Logo_of_YouTube_%282015-2017%29.svg/70px-Logo_of_YouTube_%282015-2017%29.svg.png)](https://www.youtube.com/results?search_query=Python+-+Async+Comprehension)

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

+ [x] 0\. **Async Generator**

+ **[0-async_generator.py](./0-async_generator.py)**

Write a coroutine called   *` async_generator `*   that takes no arguments. 
The coroutine will loop 10 times, each time asynchronously wait 1 second, then yield a random number between 0 and 10. Use the   *` random `*   module.

```bash
$ cat 0-main.py
#!/usr/bin/env python3

import asyncio

async_generator = __import__('0-async_generator').async_generator

async def print_yielded_values():
    result = []
    async for i in async_generator():
        result.append(i)
    print(result)

asyncio.run(print_yielded_values())

$ ./0-main.py
[4.403136952967102, 6.9092712604587465, 6.293445466782645, 4.549663490048418, 4.1326571686139015, 
9.99058525304903, 6.726734105473811, 9.84331704602206, 1.0067279479988345, 1.3783306401737838]

```
---

+ [x] 1\. **Async Comprehensions**

+ **[1-async_comprehension.py](./1-async_comprehension.py)**

Import   *` async_generator `*   from the previous task and then write a coroutine called   *` async_comprehension `*   that takes no arguments. 
The coroutine will collect 10 random numbers using an async comprehensing over   *` async_generator `*, then return the 10 random numbers.

```bash
$ cat 1-main.py
#!/usr/bin/env python3

import asyncio

async_comprehension = __import__('1-async_comprehension').async_comprehension


async def main():
    print(await async_comprehension())

asyncio.run(main())

$ ./1-main.py
[9.861842105071727, 8.572355293354995, 1.7467182056248265, 4.0724372912858575, 0.5524750922145316,
8.084266576021555, 8.387128918690468, 1.5486451376520916, 7.713335177885325, 7.673533267041574]

```
---

+ [x] 2\. **Run time for four parallel comprehensions**

+ **[2-measure_runtime.py](./2-measure_runtime.py)**

Import *` async_comprehension `* from the previous file and write a *` measure_runtime `* coroutine that will execute *` async_comprehension `* four times in parallel using *` asyncio.gather `*.
*` measure_runtime `* should measure the total runtime and return it. <br>
Notice that the total runtime is roughly 10 seconds, explain it to yourself.

```bash
$ cat 2-main.py
#!/usr/bin/env python3

import asyncio


measure_runtime = __import__('2-measure_runtime').measure_runtime


async def main():
    return await(measure_runtime())

print(
    asyncio.run(main())
)

$ ./2-main.py
10.021936893463135


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
