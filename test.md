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
