1. **Passing Arguments to a Function**:

    ```python
def greet(name):
    print("Hello, " + name + "!")

greet("John")
```

2. **Passing Multiple Arguments to a Function**:

    ```python
def greet(first_name, last_name):
    print("Hello, " + first_name + " " + last_name + "!")

greet("John", "Doe")
```

3. **Passing Arguments with Default Values**:

    ```python
def greet(name = "World"):
    print("Hello, " + name + "!")

greet()  # Output: Hello, World!
greet("John")  # Output: Hello, John!
```

4. **Passing a Variable Number of Arguments**:

    ```python
def greet(*names):
    for name in names:
        print("Hello, " + name + "!")

greet("John", "Jane", "Bob")
```

5. **Passing Keyword Arguments**:

    ```python
def greet(**kwargs):
    if 'name' in kwargs:
        print("Hello, " + kwargs['name'] + "!")
    else:
        print("Hello, World!")

greet(name="John")
```

6. **Passing a Variable Number of Keyword Arguments**:

    ```python
def greet(**kwargs):
    for key, value in kwargs.items():
        print(key + ": " + value)

greet(name="John", age="30", country="USA")
```

7. **Using the `*args` and `**kwargs` Together**:

    ```python
def greet(*args, **kwargs):
    for arg in args:
        print(arg)
    for key, value in kwargs.items():
        print(key + ": " + value)

greet("Hello", "World", name="John", age="30")
```

8. **Unpacking Arguments**:

    ```python
def greet(name, age):
    print("Hello, " + name + "! You are " + age + " years old.")

person = ["John", "30"]
greet(*person)
```

9. **Unpacking Keyword Arguments**:

    ```python
def greet(name, age):
    print("Hello, " + name + "! You are " + age + " years old.")

person = {"name": "John", "age": "30"}
greet(**person)
```

10. **Using Lambda Functions with Arguments**:

    ```python
greet = lambda name: print("Hello, " + name + "!")
greet("John")
```
Sure! Here are 10 different variants of Python code that demonstrate multiple parameters and multiple arguments:

1. **Simple Multiple Parameters and Arguments**:

    ```python
def greet(first_name, last_name):
    print("Hello, " + first_name + " " + last_name + "!")

greet("John", "Doe")
```

2. **Multiple Parameters with Default Values**:

    ```python
def greet(first_name, last_name = "Doe"):
    print("Hello, " + first_name + " " + last_name + "!")

greet("John")
greet("Jane", "Smith")
```

3. **Variable Number of Arguments**:

    ```python
def greet(*names):
    for name in names:
        print("Hello, " + name + "!")

greet("John", "Jane", "Bob")
```

4. **Variable Number of Keyword Arguments**:

    ```python
def greet(**kwargs):
    for key, value in kwargs.items():
        print(key + ": " + value)

greet(name="John", age="30", country="USA")
```

5. **Combining Multiple Parameters and Variable Arguments**:

    ```python
def greet(first_name, *last_names):
    print("Hello, " + first_name + "!")
    for last_name in last_names:
        print("Hello, " + last_name + "!")

greet("John", "Doe", "Smith")
```

6. **Combining Multiple Parameters and Variable Keyword Arguments**:

    ```python
def greet(first_name, **kwargs):
    print("Hello, " + first_name + "!")
    for key, value in kwargs.items():
        print(key + ": " + value)

greet("John", age="30", country="USA")
```

7. **Using `*args` and `**kwargs` Together**:

    ```python
def greet(*args, **kwargs):
    for arg in args:
        print(arg)
    for key, value in kwargs.items():
        print(key + ": " + value)

greet("Hello", "World", name="John", age="30")
```

8. **Unpacking Multiple Arguments**:

    ```python
def greet(first_name, last_name):
    print("Hello, " + first_name + " " + last_name + "!")

names = ["John", "Doe"]
greet(*names)
```

9. **Unpacking Multiple Keyword Arguments**:

    ```python
def greet(first_name, last_name):
    print("Hello, " + first_name + " " + last_name + "!")

person = {"first_name": "John", "last_name": "Doe"}
greet(**person)
```

10. **Using Lambda Functions with Multiple Parameters and Arguments**:

    ```python
greet = lambda first_name, last_name: print("Hello, " + first_name + " " + last_name + "!")
greet("John", "Doe")
```
