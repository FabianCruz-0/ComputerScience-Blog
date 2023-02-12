---
layout: default
title: Object-Oriented Programming
permalink: /oop/
nav_order: 2
# has_children: true
has_toc: false
---

# Object-Oriented Programming
### Introduction
<p>
  <i>What is Object-Oriented Programming?</i>
</p>

<p class="concept l-font">
 They are a way to represent information about a "real world" 
 idea and they contain ways to manipulate that information.
Is a programming paradigm based on the concept of "objects", 
which contain information in the form of fields 
(sometimes also referred to as <span class="fw-700">attributes</span> or <span class="fw-700">properties</span>) 
and code in the form of <span class="fw-700">methods</span>. The object-oriented programming has key concepts
called <span class="fw-700">"pillars of object-oriented programming"</span>. These are: 
<code class="fw-700">inheritance</code>, <code class="fw-700">abstraction</code>, <code class="fw-700">polymorphism</code> and <code class="fw-700">encapsulation</code>.
</p>

<p class="l-font">
    OOP has a lot of fundamental concepts, let's start with the most important:
</p>

## Class

<p class="l-font">
    A class is a kind of "<i>template</i>" in which the attributes 
    and methods of a type of object are defined. 
    This template is created to be able to create objects easily. 
    The method of creating new objects by reading and retrieving the 
    attributes and methods of a class is known as <span class="fw-700">instantiation</span>.
</p><br>
This is an example of a class of a Car:

```mermaid
classDiagram
    direction RL 
    Nissan 370Z .. Car
    class Car{
        <<Class>>
        +String Color
        +String Model
        +String Transmission
        +TurnOnEngine()
        +TurnOffEngine()
    } 
    class Nissan 370Z{
        <<Object>>
        +String Color: "Black"
        +String Model: "Nissan 370Z"
        +String Transmission: "Automatic"
        +TurnOnEngine()
        +TurnOffEngine()
    }
```
{: .bg-white }

<p class="l-font">
    In this example we can see how "Nissan 370Z" is an <b>instance</b> of the <code>Car class</code>. 
    Objects receive the attributes of the instantiated class.
</p>

<code>Car Class:</code>
{% capture some_var %}
{% highlight java linenos %}
public class Car{
  public String color;
  public String model;
  public String transmission;

  public void turnOnEngine(){
    System.out.println("Engine Turned On.");
  }
  
  public void turnOffEngine(){
    System.out.println("Engine Turned Off.");
  }

  public Car(String color,String model, String transmission){
    this.color = color;
    this.model = model;
    this.transmission = transmission;
  }
}
{% endhighlight %}
{% endcapture %}
{% include fix_linenos.html code=some_var %}

<code>Instantiation of the Car Class:</code>
{% capture some_var %}
{% highlight java linenos %}
class Main {
  public static void main(String[] args) {
    Car myCar = new Car("Black","Nissan 30Z", "Automatic");
    System.out.println(myCar.color); // Will print: Black.
  }
}
{% endhighlight %}
{% endcapture %}
{% include fix_linenos.html code=some_var %}

## Inheritance

<p class="l-font">
    Inheritance allows classes to inherit features of other classes. 
    Parent classes extend attributes and behaviors 
    to child classes. Inheritance supports reusability.

    If basic attributes and behaviors are defined in a parent class, 
    child classes can be created, extending the functionality of the 
    parent class <b>and adding additional attributes and behaviors</b>.
</p>

<p class="important">
Parent classes are also known as superclasses or base classes. 
The child class can also be called a subclass, derived class, or extended class.
</p>

## Encapsulation
<p class="l-font">

</p>

## Abstraction
<p class="l-font">
    
</p>

## Polymorphism
<p class="l-font">
    
</p>

introducir valor de num1
inoikhkh