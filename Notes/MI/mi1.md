---
layout: page
title: 1 Data in Medicine
---
* Data in medicine
{:toc}

# Data in medicine

Medical informatics is the body of knowledge, methods, and theories that focus on the
effective use of Information and knowledge to improve the quality, the safety, and the
cost-effectiveness of patient care as well as the health of both individuals and
populations.
Medical informatics deals with many types of data:

* Numerical values
* Biosignals
* Bioimages
* Multilevel bioimages
* Biomovies
* Fusion of bioimages
* Plain text in natural language
* Structured text

All these data can be stored in the electronic medical record EMR.

## Electronic medical records EMRs

EMRs are digital versions of the paper charts in clinician offices, clinics, and hospitals.
EMRs contain notes and information collected by and for the clinicians in that office,
clinic, or hospital and are mostly used by providers for diagnosis and treatment.
EMRs are more valuable than paper records because they enable providers to track
data over time, identify patients for preventive visits and screenings, monitor
patients, and improve health care quality.
General operations that can be done to a EMR are:

1. Data entry
2. Query
3. Archiving and Conservation

EMR is composed by different sections such as:
*  Personal data
*  Historical data
*  Admission data
*  Anamnesis, medical history
*  Physiological anamnesis
*  Pathological anamnesis
*  Past pathological anamnesis
*  Physical examination
*  Laboratory test
*  Diagnosis
*  Decision-therapy

An EMR is more beneficial than a paper records because it allows providers to:
  * Track data over time
  + Identify patients who are due for preventive visits and screenings
  + Monitor how patients measure up to certain parameters, such as vaccinations
and blood pressure readings
  + Improve overall quality of care in a practice

### Medical data summary

Medical data are used for mainly 4 reasons:

1. **Recording** ​aim:
    1. Historical record
    2. Legal record
2. **Communication** ​ aim: communication among providers
3. **Risk assessment** ​ aim:
    1. Anticipate future health problems
    2. Identify deviations from expected trends
4. **Research** ​ aim: support clinical research


Related to these reasons there are also 3 main arguments that emphasize the
importance of digitally collecting medical data:

**1. Pragmatic and logistical issues:**
  1. Timeliness of data accessibility
  2. Readiness of data
  3. Possibility to update data when new observations are made

**2. Avoid redundancy and inefficiency:**
  1. Avoid data duplication that may introduce errors
  2. Avoid sparse information

**3. Support data re-use** ​:
  1. Clinical and epidemiological research
  2. Data mining
  3. Input for decision support systems

Medical data need to be collected in database: structured collection of individual
observartions without any summarizing analysis. Databases can be used to create
new data, read existing ones, change existing ones and delete. Every action
performed within a database is called Process.

## Electronic health records EHRs

EHRs are built to go beyond standard clinical data collected in a provider’s office and
are inclusive of a broader view of a patient’s care. EHRs contain information from all
the clinicians involved in a patient’s care and all authorized clinicians involved in a
patient’s care can access the information to provide care to that patient.
EHRs also share information with other health care providers, such as laboratories
and specialists. EHRs follow patients – to the specialist, the hospital, the nursing
home, or even across the country.

### Contents


*  Identification data of registry of the patient
*  Administrative data concerning the healthcare
*  Health and social health documents
*  Patient summary or synthethic health profile
*  Citizen’s personal notebook
*  Statement of intent to donate organs and tissues


## EMRs VS EHRs

An EMR contains the standard medical and clinical data gathered in one provider’s
office. Electronic health records (EHRs) go beyond the data collected in the provider’s
office and include a more comprehensive patient history.
Unlike EMRs, EHRs also allow a patient’s health record to move with them to other
health care providers, specialists, hospitals, nursing homes, and even across states.

## Personal health records PHRs

A personal health record, or PHR, is an electronic application through which patients
can maintain and manage their health information (and that of others for whom they
are authorized) in a private, secure, and confidential environment.
PHRs contain the same types of information as EHRs—diagnoses, medications,
immunizations, family medical histories, and provider contact information.
PHRs can include information from a variety of sources including clinicians, home
monitoring devices, and patients themselves.


# Unified modeling language: UML

Models are used to:

1. Give a​ **visual representation** ​ of a system or a process
2. **Specify the architecture** ​or the behavior of a system
3. **Implement** ​a system
4. **Document** ​ the decisions taken during the implementation of a system
Generally, by modeling you can focus on a specified aspect of the system you are
trying to understand. A model can be expressed at different levels of detail.
There are 5 modeling principles
1. Observe the world
2. Choose the type of model
3. The model can describe different levels of abstraction of a system
4. The model must be connected to the reality
5. A complex system should be modeled by a set of interrelated but independent
models

## Object oriented programming

Object oriented programming is the creation of a system built by a set of objects
(abstraction of reality) interacting each other through exchanged messages.
There are 4 basic concepts:

1. Objects and classes
2. Inheritance
3. Encapsulation
4. Polymorphism

## Objects

An object is an entity or element of the real world that can be identified in a unique
way (e.g. customer, a product, a patient...).
Each object is composed by the set of their characteristic data and a set of methods
acting on those data for providing services to the rest of the system.
Each object is described by:
*  Attributes that define the characteristics
*  Methods (functions), that describe the behaviors


### Classes and objects

A class:
*  Is a template for objects
*  Defines object properties
*  Describes object behavior

Consequently, an object is a member or an “instance” of a class. An object has a state
in which all of its properties have values that you either explicitly define or that are
defined by default settings.
All the objects that share the same attributes and the same behaviors can be collected
in the same class. The methods are common for all the objects of a class. The data
types of attributes are common for all the objects of a class, while the attribute values
can be different for each object.
A class is responsible for the creation of new objects (i.e. class instances) having its
own OID (the concept of an object identifier (OID) as a means of uniquely identifying
a particular object).

### Inheritance

It is a property that allows to define a class (sub-class or child class) starting from
another class (super class or mother class). Between the classes Person and Employee
a relationship IS-A exists; it is a hierarchy of specialization - generalization.
The sub-class inherits the operations and attributes of the super class. Each sub class
can enrich the inherited methods and attributes with additional ones.

### Encapsulation

Encapsulation is the property of hiding/protect the internal behavior of a method.
Behavior encapsulation protects applications or other classes from seeing the internal
implementation of a behavior. Encapsulated attributes usually have behaviors that
provide clients some form of access to the attribute. Objects hide structure to the
external environment because to use an object we need to know attributes and
methods, but not its internal structure. Methods and attributes encapsulated into an
object are not directly accessible to clients of a class. Only the public interface of the
object is known (interfaces of methods). Attributes of an object can be manipulated
only by calls of methods.

Every class is defined in two ways: the first external (public) and the second internal
(private):

*  External Level or Public Interface: It specifies the messages (and arguments
associated to the messages) that can be sent to the objects of the class.

*  Internal or Private Level: It defines the object properties (attributes) and how
to manipulate them (methods)

### Polymorphism

Literally, it means the ability of assuming different shapes.
Polymorphism relates decoupling in terms of types. An object activates the correct
methods depending on the class type, when receives a message.
The classes TRIANGLE and EXAGON have the same superclass POLYGON. They reply
to the message of area calculation with different behaviors

## Benefits of the object oriented modeling

### Reusability

Object classes can be reused in different context. It is possible to specialize a class for
making available particular behaviors (new attributes and methods)

### Software robustness and maintenance

Changes in method body of a class don’t affect the users of that class. It is always clear
the responsibility of an object in a context and thus it is easy to understand who is
responsible for abnormal behaviors.

### Data integrity

Data can be manipulated only by specific method that have to respect “buisness
rules”.

### Control of complexity

Inheritance allows to separate a system in more simple blocks to facilitate the domain
understanding.

### Interoperability

OO programming languages allow the development of a software on heterogeneous
platforms. Communication and cooperation are performed by message exchanges.


# UML

UML is an object oriented modeling language. It is a semi-formal language (with
syntax and semantics) with graphical notation that allow to describe / model different
aspects of a system with an object oriented approach. UML is applicable to different
types of system (software and non- software). UML is also applicable to different types
of process “use-case driven”, architecture-centric”, iterative and incremental.

## 4 reasons why using UML


1. To ​ facilitate the visualization and the understanding ​of a system or process
  1. UML allows to have a global vision of the system in an effective and
concise way.
  2. UML uses an intuitive graphical notation to visualize actors
relationships between them.
  3.  UML facilites the communication between informatics working in
complex enviroments such as hospital​s.


2. To facilitate the specification of​ a system or process : ​ Specify​ means to build
precise and complete models.
  1.  UML allows to build precise models specifying the physical structure of
the system, its behavior, organization and implementation
  2.  UML allows to build models with different abstraction levels


3.  To​ facilitate the construction ​of a system or process:
  1.  UML can be directly connected to languages such as c++, Java etc...


4.  To ​ facilitate the documentation ​of a system or a process:
  1.  UML can document the architecture of a system, the requirements and
it can describe activities

## Uses of UML

UML common uses include:
*  Designing software
*  Communicating software or business processes
*  Capturing details about a system for requirements or analysis
*  Documenting an existing system, process, or organization
UML has been applied to countless domains, including:
*  Banking and investment sectors
*  Health care
*  Defense
*  Distributed computing
*  Embedded systems
*  Retail sales and supply


# UML syntax and diagrams

## Objects

## Structure objects


*  Class :​ description of a set of objects characterized by the same attributes,
methods and relationship
*  Interface ​: is a set of methods that specify a service of that class
*  Collaboration ​: interaction
*  Component ​: class that represents a physical part of a system
*  Node :​ class that represents a physical element existing during runtime. A node
has own memory and computational ability
*  Use Case ​: description of a series of actions that the system performs to reach
an end result, observable by a user of the system
*  Active classes ​: classes containing objects that allow control

## Behavioral objects


*  Interaction ​: behavior that includes messages exchanged by objects
*  State ​: is a behavior that specifies the sequence of states that an object get into

## Groups

**Packages:** ​are conceptual groups of elements (not physical)

## Annotations

**Notes:** ​ are comments within diagrams to describe specific parts or elements

## Relationships

**Dependence** ​: is a semantic relationship that makes that a change in an independent
class affects the dependent class (not the viceversa).

**Association:** ​is a structural relation among classes

**Generalization** ​: indicates relationships among classes and subclasses

**Realization** ​: is a semantic relationships between interfaces and components that
provide functions or services to the interfaces
