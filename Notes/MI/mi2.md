---
layout: page
title: 2 UML Diagrams
---

* Use case diagram
{:toc}

# Use case diagram



Describes the static behavior of a system from the user point of view. Identify the
behavior of a system without entering in its details. Describes the functions (uses)
offered by the system. It is useful for identify the system requirements.
Use Case diagrams capture functional requirements for a system. They provide an
implementation-independent view of what a system is supposed to do and allow the
modeler to focus on user needs rather than realization details.

* “​ **use case** ​” is the description of a series of action accessible for the user and
that lead to an end result which is observable
* **Actor** :​ initiates the use-cases and/or receives use-cases. It is an entity external
to the boundaries of the system that interacts with the system assuming a
specific role
* **Scenario** is defined as a sequence of steps describing an interaction between a
user and a system:
  * **Basic scenario** ​: usual path of steps
  * **Alternate scenarios** :represent alternative paths for the use case

## Relationships among use cases


*   Inclusion :​ When you have behavior that is similar across more than one use
case you can define that behavior as a use case, so you can reuse it avoiding
repetition. Instead of repeating this shared activity, it become a use case that is
included in the more complex ones. Similar to the sub-routine call in a
programming language

*   Generalizations :​ When you have a use case similar to another but having
something more; the new use case inherits the behaviors of the parent use
case; the child use case is enriched by new scenarios. The «child» use case can:
○ Inherit all the attributes, the scenarios the extension points defined in
the «father» use case
○ Partecipate to all the relationships in which is involved the «father» use
case
○ Have new scenarios with respect to the «father» use case

*   Extension :​ Similar to the Generalization but you wish to use the more
controlled form, declaring your extension points for the basic use case. It
represents the optional behaviour


# Activity diagram

The activity diagram describes the sequence of activities including conditional and
parallel behaviours. Conditional behaviour is represented as:

*   branch (one input multiple outputs)
*   merge (multiple inputs one output)

Parallel behaviour is represented as:
*   fork (one input multiple outputs): indicates that all of the outputs are executed
in parallel as follows
  * Simultaneously
  * Sequentially
  * Interleaved

*   join (multiple inputs one output): synchronizes all of the activities. The output
transaction is executed only when all the states of the input transactions
completed their activity.

A SWIMLANE is a way to group activities executed by the same actor (responsible). It
is a way to represent responsabilities.

Guidelines:
*   Give a logic order to the swimlanes
*   Use a maximum of 5 swimlanes
*   Use for linear processes
*   Consider the swimareas for complex systems
An activity diagram is to use when is needed:
*   To analyse a use case
*   To understand a workflow
*   To describe a complex algorithm
*   To document multi-threads applications


# Class diagram

## Essential elements

A class diagram describes the static architecture of a system using classes (types of
objects) and the various relationships existing among them. Essential Elements are:
*   CLASS: describes a set of objects that have the same attributes, methods and
behaviors. It is composed by:
  * Name
  * Attributes: properties of the class. Their visibility can be pubilc, private,
protected or package
  * Methods: implement “procedures” and “functions”


*   RELATIONSHIPS:
  * Associations: establishes a logical connection between classes.
Associations are also described by cardinalities: the cardinality
indicates the number of instances of a class that can be associated to
single instances of the other class. It should be indicated at both the
ends of the association; when it is not reported it does not mean that is
equal to 1
  * Subtypes

## Primary and foreign keys

The primary key is the unique identifier of a class (it is an attribute or a set of
attributes). This implies that there are not two objects identified with the same value
of the attribute that is chosen as PK. The PK cannot have NULL values.
The foreign key is a constraint of referencial integrity. It constraints, identifies and
enforces the association between classes. In a foreign key reference, a link is created
between two classes when the attribute that hold the primary key value for one class
is refernced by the attribute in another class. This attribute becomes a foreign key FK
in the second class.

## Different types of relationship


*   Generalization :​ implement the IS-A ​ relationship. It connects a specialized
class (sublcass) to a general class (parent class). Subclasses inherits from
superclasses methods, attributes and relationships. Subclasses can have more
attributes and methods, more relationships and overloading of operators

*   Aggregation :​ is a type of association that models a relationship among an
object and its parts. It models the relationship “​ Is a part of” (e.g. door is a part
of the car)

*   Composition ​: is a strong type of aggregation which states that:
  * The aggregate is the only owner of its part
  * The part can belong to only one aggregate
  * The life of the part depends on the life of the aggregate


*   Dependency ​: is the lightest relationship among classes. IT models the “ Use” ​
relationship.

# Physical diagrams

They document the physical aspects of a system. There are two types of physical
diagrams:

**1. Deployment diagram** ​: it shows the static relationships among software and
    hardware components of a system during runtime

**2. Component diagram** ​: it shows the architecture and the dependency involved
    into the implementation of the system
       a. Node is a class that represent a physical element existing during
          runtime
       b. Component is a class that represent a physical paort of a system

# Interaction diagrams

Interaction diagrams model the collaboration between objects while executing a
specific activity. They represent the ​ **dynamic** behaviour of a specific use case in terms
of objects and messages exchanged between objects. There are two interaction
diagrams in UML: Sequence and Collaboration diagram.

## Sequence diagram

It shows the interaction between objects by means of a temporal sequence of actions.
Principal features are:
*   Objects
*   Temporal sequences of exchanged messages
*   There are not associations between objects
*   The different objects are placed horizontally
Time is the vertical flow (life-line), the timescale is not important. It is important the
temporal sequence of the events but not the absolute distance between events or the
durations of events they are used to describe real-time systems.


An important part of sequence diagrams are the message exchanged between objects:
Major considerations:
*   The strength of the sequence diagram is the simplicity and the immediate
visual interpretation.
*   The meaning of the represented dynamics can be relative to objects of the
domain (conceptual) or of the system to be realized (implementation and
technical specifications).
*   The sequence diagram is very important in the project documentation because
it shows the main control flow.
*   The sequence diagram can be used to represent concurrent processes
There are other elements in a sequence diagrams:
**Frame** ​: is the graphical boundary of the sequence diagram and it’s optional
**Combined fragment** :​ is a part of the sequence diagram defined by an operator of the
interaction. The operators can be:
*   Alt- alternative
*   Break
*   Opt-optional
*   Neg- deny
*   Loop- cycle


**Guard** ​: the guards are the conditions that define when the fragment can be executed

## Collaboration diagram

Objects are represented as icons. Messages are arrows between objects. The sequence
is indicated by the message enumeration. It’s different from the sequence diagram
because:

1. The emphasis is not on time, but on the ​ **collaboration between objects** ​.
2. There is not a precise time dimension, the temporal sequences are described
    only by the enumeration of the exchanged messages

# State diagrams

## Statechart

It is a state machine describing events, transitions and activities to model the dyamic
behaviour of a system or an element. As the activity diagram they are used to
**describe the lifeline of an object** ​.

In the activity diagram the emphasys is on the flow of the activities and the transition
between two activities is dependent only on the end of the first activity. In the
statechart the flow between states is represented and the transition between them is
well described by the arrival of a specific event.
Essential elements are:

* **State** :​ specific situation in which an object is because it satisfies a specific
condition or it executes a specific activity or waits for an event
*   **Transition** is the relationship between two state. It indicates that an object in
state  1  is doing some operations and when a specific event occurs (or specific
conditions are fulfilled) the object goes to the State 2
*   **Event** ​ is an occurrence of a stimulus that triggers a state transition. The event
is an observable occurrence. There could be:
  * **Interaction** :​ call event (synchronous operation) or asynchronous
reception of a signal
  * **Time event**
  * **Change event**
Statecharts are used to represent classes and objects having a complex life cycle that
includes well defined steps.
