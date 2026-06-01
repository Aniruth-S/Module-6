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
