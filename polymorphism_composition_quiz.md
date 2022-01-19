# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Polymorphism means the condition of occuring in many forms. 

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

When we apply polymorphism to OO design, it means we can define variables or parameters which can be of many different types. For example, if we have classes ```Car``` and ```Motorbike``` which both inherit from the abstract class ```Vehicle```, wherever a type is declared as ```Vehicle```, the subclasses ```Car``` and ```Motorbike``` can be validly substituted.
```java
public abstract class Vehicle {}
public class Car extends Vehicle{}
public class Motorbike extends Vehicle{}
ArrayList<Vehicle> vehicles = new ArrayList<>();
vehicles.add(new Car());
vehicles.add(new Motorbike());
```   

3. What can we use to implement polymorphism in Java?

In Java, we can implement polymorphism using inheritance with classes or abstract classes; or interfaces.

4. How many 'forms' can an object take when using polymorphism?

The number of forms an object can take when using polymorphism is determined by the number of classes or interfaces which extend or implement the base class or interface.

5. Give an example of when you could use polymorphism.

You could use polymorphism when you require a variable which could be of many types which all have the same methods/properties or similar behaviours. For example, you could require a vehicle which could be a car/motorbike/train etc.

# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

Composition refers to an object being composed of other other objects.

7. When would you use composition? Provide a simple example in Java.

You would use composition where a *is-a-part-of* or *has-a* relationship exists between two objects. For example, a roof *is a part of* a house. A car *has an* engine but an engine can exist independently and can form part of other vehicles such as a motorbike.

8. Give a difference between composition and aggregation?

Composition refers to objects which exist solely as part of another object. Aggregation refers to objects which exist as part of another object but can exist independently.

9. What is/are the advantage(s) of using composition/aggregation?

The advantage of using composition/aggregation in comparison to inheritance is that it better reflects real-world objects and reduces complex inheritance hierarchies.

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

When an object using composition is destroyed, all objects which form part of that object are also destroyed.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

When an object aggregation is destroyed, the objects which form part of that object will not necessarily be destroyed.