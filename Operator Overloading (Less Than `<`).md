# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.
## 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```py
class Beans(): 
     def type(self): 
       print("Vegetable") 
     def color(self):
       print("Green") 
class Mango(): 
     def type(self): 
       print("Fruit") 
     def color(self): 
       print("Yellow")      
def func(obj): 
       obj.type()
       obj.color()
#creating objects
obj_beans = Beans() 
obj_mango = Mango() 
func(obj_beans) 
func(obj_mango)
```
## Output
<img width="306" height="235" alt="image" src="https://github.com/user-attachments/assets/913d02d5-d168-4ebc-86a7-0aa1f299bc2d" />

## Result
Successfully created two specific classes — `Beans` and `Mango`. Then, created a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.
2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```py
class Marks(object):
    def __init__(self, x):
        self.x = x
    def __lt__(self, other):
        return self.x < other.x
obj1 = Marks(20)
obj2 = Marks(10)

print("ob2 is less than ob1" if obj2 < obj1 else "ob1 is less than ob2")
```
## Output
<img width="661" height="248" alt="image" src="https://github.com/user-attachments/assets/396dd304-e9a2-4e44-b127-7b3a333b276a" />


## Result
Successfully wrote a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.
