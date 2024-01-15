# Asynchronous Python Project

## Learning Objectives
By the end of this project, you will be able to explain:

- The basics of async and await syntax
- How to execute an async program with asyncio
- Running concurrent coroutines
- Creating asyncio tasks
- Using the random module

## Requirements
### General
- A README.md file is mandatory at the root of the project folder.
- Allowed editors: vi, vim, emacs
- All files will be interpreted/compiled on Ubuntu 18.04 LTS using Python 3 (version 3.7)
- All files should end with a new line
- All files must be executable
- The length of your files will be tested using wc
- The first line of all your files should be exactly #!/usr/bin/env python3
- Code should use the pycodestyle style (version 2.5.x)
- All functions and coroutines must be type-annotated
- All modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
- All functions should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'`)

### Tasks
#### 0. The basics of async
- Write an asynchronous coroutine named `wait_random` that takes an integer argument `max_delay` (with a default value of 10).
- Use the random module to generate a random delay between 0 and `max_delay` (inclusive) seconds.
- The coroutine should return the random delay.

Example:
```python
import asyncio

wait_random = __import__('0-basic_async_syntax').wait_random

print(asyncio.run(wait_random()))
print(asyncio.run(wait_random(5)))
print(asyncio.run(wait_random(15)))
