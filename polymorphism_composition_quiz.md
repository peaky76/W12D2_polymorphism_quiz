# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the **_word_** 'polymorphism' mean?

Polymorphism means the ability to take many forms.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It means that an object can "pass" as one of many different classes, typically when a child class inherits from a parent class. For example a class Car may extend an abstract class Vehicle. An instance of the Car class is also an instance of the Vehicle class so could be used wherever a Vehicle type is required, say in a function.

3. What can we use to implement polymorphism in Java?

Inheritance and interfaces

4. How many 'forms' can an object take when using polymorphism?

It depends how many links it has in the inheritance chain and how many interfaces it has.

5. Give an example of when you could use polymorphism.

Say you were creating a football team app, where the user could select eleven footballers to make a team.
The app may have different classes of footballer - goalkeeper, defender, striker etc. - each derived from the parent Footballer class. Polymorphism would allow you to create a team of eleven players in any formation using an ArrayList of type Footballer. You wouldn't have to specify a particular number in each position as every defender, striker etc. would also pass as a type Footballer.

# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

Composition is when a class is created using objects of another class and the objects of the other class do not really have an independent existence of their own. It can be thought of a "has-a" relationship.

7. When would you use composition? Provide a simple example in Java.

You would use it when the "has-a" relationship provides a suitable model. For instance, we may choose to represent a keyboard as a set of key objects. The keys are objects in their own right with their own properties (e.g. symbol, size) and the keyboard is composed of them.

8. Give a difference between composition and aggregation?

Composition is an ownership relationship. When the owning object is destroyed, the objects of which it is composed are destroyed too. This does not happen with aggregation. Objects can be created as an aggregation of other objects, e.g. a team may be made up of an aggregration of staff, but the aggregating objects (the staff) are initiated separately and continue to exist if the overarching object (the team) is destroyed.

9. What is/are the advantage(s) of using composition/aggregation?

It is flexible. You can swap in other objects of the same type, e.g. if a team was composed of a manager and staff members, you can easily swap one manager for another without having to create another team.

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

They are destroyed too.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

They are not destroyed.
