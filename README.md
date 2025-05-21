# PYTHON-WEEK-5-ASSIGNMENT
# 🧠 OOP Assignment - Custom Classes & Polymorphism in Python

Welcome to my Object-Oriented Programming (OOP) assignment repository! This project demonstrates key OOP concepts including **class creation**, **inheritance**, **encapsulation**, and **polymorphism** using fun and relatable examples.


## Assignment 1 & 2: Design Your Own Class

### `superhero.py`
In this file, I created a custom class called `Superhero` and a subclass `FlyingSuperhero` to demonstrate:
- Class attributes and methods
- Use of constructors (`__init__`)
- Inheritance
- Encapsulation (with private attributes and getter methods)

**Example Output:**
```python
I am Flash, and my power is Super Speed!
Flash uses Super Speed with strength level 90!
I am Superman, and my power is Super Strength!
Superman uses Super Strength with strength level 100!
Superman is flying at 500 km/h!

**## Polymorphism Challenge - OOP in Python**

This mini-project demonstrates **polymorphism** in Python using Object-Oriented Programming (OOP). The goal is to show how different classes can implement the same method in their own unique way.

---

## 🧪 What This Project Does

We define a base class `Vehicle` and several subclasses:
- `Car`
- `Plane`
- `Bicycle`

Each subclass overrides the `move()` method to behave differently. This demonstrates **runtime polymorphism**, where the same method name produces different results depending on the object calling it.

---

## 📄 Code Breakdown

### `vehicles.py`

```python
class Vehicle:
    def move(self):
        raise NotImplementedError("Subclass must implement this method")

class Car(Vehicle):
    def move(self):
        return "Driving 🚗"

class Plane(Vehicle):
    def move(self):
        return "Flying ✈️"

class Bicycle(Vehicle):
    def move(self):
        return "Pedaling 🚲"

# Polymorphism in action
vehicles = [Car(), Plane(), Bicycle()]
for vehicle in vehicles:
    print(vehicle.move())
