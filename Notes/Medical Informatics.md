---
title: Medical Informatics Notes


---
* 1 Data in Medicine
* 2 UML Diagrams
* 3 CUP in UML
* 4 DBMS
* 5 Standards in medical informatics
* 6 Clinical guidelines and protocols
* 7 Open Data
{:toc}
# Data in medicine

Medical informatics is the body of knowledge, methods, and theories that focus on the
effective use of Information and knowledge to improve the quality, the safety, and the
cost-effectiveness of patient care as well as the health of both individuals and
populations.
Medical informatics deals with many types of data:
● Numerical values
● Biosignals
● Bioimages
● Multilevel bioimages
● Biomovies
● Fusion of bioimages
● Plain text in natural language
● Structured text
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
● Personal data
● Historical data
● Admission data
● Anamnesis, medical history
● Physiological anamnesis
● Pathological anamnesis
● Past pathological anamnesis
● Physical examination


● Laboratory test
● Diagnosis
● Decision-therapy
An EMR is more beneficial than a paper records because it allows providers to:
+ Track data over time
+ Identify patients who are due for preventive visits and screenings
+ Monitor how patients measure up to certain parameters, such as vaccinations
and blood pressure readings
+ Improve overall quality of care in a practice

### Medical data summary

Medical data are used for mainly 4 reasons:

1. **Recording** ​aim:
    a. Historical record
    b. Legal record
2. **Communication** ​ aim: communication among providers
3. **Risk assessment** ​ aim:
    a. Anticipate future health problems
    b. Identify deviations from expected trends
4. **Research** ​ aim: support clinical research


Related to these reasons there are also 3 main arguments that emphasize the
importance of digitally collecting medical data:

**1. Pragmatic and logistical issues:**
    a. Timeliness of data accessibility
    b. Readiness of data
    c. Possibility to update data when new observations are made
**2. Avoid redundancy and inefficiency:**
    a. Avoid data duplication that may introduce errors
    b. Avoid sparse information
**3. Support data re-use** ​:
    a. Clinical and epidemiological research
    b. Data mining
    c. Input for decision support systems
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

```
● Identification data of registry of the patient
● Administrative data concerning the healthcare
● Health and social health documents
● Patient summary or synthethic health profile
● Citizen’s personal notebook
● Statement of intent to donate organs and tissues
```

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
● Attributes that define the characteristics
● Methods (functions), that describe the behaviors


### Classes and objects

A class:
● Is a template for objects
● Defines object properties
● Describes object behavior
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
implementation of a behavior.Encapsulated attributes usually have behaviors that
provide clients some form of access to the attribute. Objects hide structure to the
external environment because to use an object we need to know attributes and
methods, but not its internal structure. Methods and attributes encapsulated into an
object are not directly accessible to clients of a class. Only the public interface of the
object is known (interfaces of methods). Attributes of an object can be manipulated
only by calls of methods.
Every class is defined in two ways: the first external (public) and the second internal
(private):
● External Level or Public Interface: It specifies the messages (and arguments
associated to the messages) that can be sent to the objects of the class.


```
● Internal or Private Level: It defines the object properties (attributes) and how
to manipulate them (methods)
```
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

```
1) To ​ facilitate the visualization and the understanding ​of a system or process
a) UML allows to have a global vision of the system in an effective and
concise way.
b) UML uses an intuitive graphical notation to visualize actors
relationships between them.
c) UML facilites the communication between informatics working in
complex enviroments such as hospital​s.
2) To facilitate the specification of​ a system or process : ​ Specify​ means to build
precise and complete models.
a) UML allows to build precise models specifying the physical structure of
the system, its behavior, organization and implementation
b) UML allows to build models with different abstraction levels
3) To​ facilitate the construction ​of a system or process:
a) UML can be directly connected to languages such as c++, Java etc...
4) To ​ facilitate the documentation ​of a system or a process:
a) UML can document the architecture of a system, the requirements and
it can describe activities
```
## Uses of UML

UML common uses include:
● Designing software
● Communicating software or business processes
● Capturing details about a system for requirements or analysis
● Documenting an existing system, process, or organization
UML has been applied to countless domains, including:
● Banking and investment sectors
● Health care
● Defense
● Distributed computing
● Embedded systems
● Retail sales and supply


# UML syntax and diagrams

## Objects

## Structure objects

```
● Class :​ description of a set of objects characterized by the same attributes,
methods and relationship
● Interface ​: is a set of methods that specify a service of that class
● Collaboration ​: interaction
● Component ​: class that represents a physical part of a system
● Node :​ class that represents a physical element existing during runtime. A node
has own memory and computational ability
● Use Case ​: description of a series of actions that the system performs to reach
an end result, observable by a user of the system
● Active classes ​: classes containing objects that allow control
```
## Behavioral objects

```
● Interaction ​: behavior that includes messages exchanged by objects
● State ​: is a behavior that specifies the sequence of states that an object get into
```
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


## Diagram types

### Structure diagrams

### Behavior diagrams


# Use case diagram

Describes the static behavior of a system from the user point of view. Identify the
behavior of a system without entering in its details. Describes the functions (uses)
offered by the system. It is useful for identify the system requirements.
Use Case diagrams capture functional requirements for a system. They provide an
implementation-independent view of what a system is supposed to do and allow the
modeler to focus on user needs rather than realization details.
● A “​ **use case** ​” is the description of a series of action accessible for the user and
that lead to an end result which is observable
**● Actor** :​ initiates the use-cases and/or receives use-cases. It is an entity external
to the boundaries of the system that interacts with the system assuming a
specific role
**● Scenario** is defined as a sequence of steps describing an interaction between a
user and a system:
**○ Basic scenario** ​: usual path of steps
**○ Alternate scenarios** ​represent alternative paths for the use case

## Relationships among use cases

```
● Inclusion :​ When you have behavior that is similar across more than one use
case you can define that behavior as a use case, so you can reuse it avoiding
repetition. Instead of repeating this shared activity, it become a use case that is
included in the more complex ones. Similar to the sub-routine call in a
programming language
● Generalizations :​ When you have a use case similar to another but having
something more; the new use case inherits the behaviors of the parent use
case; the child use case is enriched by new scenarios. The «child» use case can:
○ Inherit all the attributes, the scenarios the extension points defined in
the «father» use case
○ Partecipate to all the relationships in which is involved the «father» use
case
○ Have new scenarios with respect to the «father» use case
● Extension :​ Similar to the Generalization but you wish to use the more
controlled form, declaring your extension points for the basic use case. It
represents the optional behaviour
```

# Activity diagram

The activity diagram describes the sequence of activities including conditional and
parallel behaviours. Conditional behaviour is represented as:
● branch (one input multiple outputs)
● merge (multiple inputs one output)
Parallel behaviour is represented as:
● fork (one input multiple outputs): indicates that all of the outputs are executed
in parallel as follows
○ Simultaneously
○ Sequentially
○ Interleaved
● join (multiple inputs one output): synchronizes all of the activities. The output
transaction is executed only when all the states of the input transactions
completed their activity
A SWIMLANE is a way to group activities executed by the same actor (responsible). It
is a way to represent responsabilities.
Guidelines:
● Give a logic order to the swimlanes
● Use a maximum of 5 swimlanes
● Use for linear processes
● Consider the swimareas for complex systems
An activity diagram is to use when is needed:
● To analyse a use case
● To understand a workflow
● To describe a complex algorithm
● To document multi-threads applications


# Class diagram

## Essential elements

A class diagram describes the static architecture of a system using classes (types of
objects) and the various relationships existing among them. Essential Elements are:
● CLASS: describes a set of objects that have the same attributes, methods and
behaviors. It is composed by:
○ Name
○ Attributes: properties of the class. Their visibility can be pubilc, private,
protected or package
○ Methods: implement “procedures” and “functions”
● RELATIONSHIPS:
○ Associations: establishes a logical connection between classes.
Associations are also described by cardinalities: the cardinality
indicates the number of instances of a class that can be associated to
single instances of the other class. It should be indicated at both the
ends of the association; when it is not reported it does not mean that is
equal to 1
○ Subtypes

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

```
● Generalization :​ implement the IS-A ​ relationship. It connects a specialized
class (sublcass) to a general class (parent class). Subclasses inherits from
superclasses methods, attributes and relationships. Subclasses can have more
attributes and methods, more relationships and overloading of operators
● Aggregation :​ is a type of association that models a relationship among an
object and its parts. It models the relationship “​ Is a part of” (e.g. door is a part
of the car)
● Composition ​: is a strong type of aggregation which states that:
○ The aggregate is the only owner of its part
```

```
○ The part can belong to only one aggregate
○ The life of the part depends on the life of the aggregate
● Dependency ​: is the lightest relationship among classes. IT models the “ Use” ​
relationship.
```
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
● Objects
● Temporal sequences of exchanged messages
● There are not associations between objects
● The different objects are placed horizontally
Time is the vertical flow (life-line), the timescale is not important. It is important the
temporal sequence of the events but not the absolute distance between events or the
durations of events they are used to describe real-time systems.


An important part of sequence diagrams are the message exchanged between objects:
Major considerations:
● The strength of the sequence diagram is the simplicity and the immediate
visual interpretation.
● The meaning of the represented dynamics can be relative to objects of the
domain (conceptual) or of the system to be realized (implementation and
technical specifications).
● The sequence diagram is very important in the project documentation because
it shows the main control flow.
● The sequence diagram can be used to represent concurrent processes
There are other elements in a sequence diagrams:
**Frame** ​: is the graphical boundary of the sequence diagram and it’s optional
**Combined fragment** :​ is a part of the sequence diagram defined by an operator of the
interaction. The operators can be:
● Alt- alternative
● Break
● Opt-optional
● Neg- deny
● Loop- cycle


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
**● State** :​ specific situation in which an object is because it satisfies a specific
condition or it executes a specific activity or waits for an event
● **Transition** is the relationship between two state. It indicates that an object in
state  1  is doing some operations and when a specific event occurs (or specific
conditions are fulfilled) the object goes to the State 2
● **Event** ​ is an occurrence of a stimulus that triggers a state transition. The event
is an observable occurrence. There could be:
**○ Interaction** :​ call event (synchronous operation) or asynchronous
reception of a signal
**○ Time event
○ Change event**
Statecharts are used to represent classes and objects having a complex life cycle that
includes well defined steps.


### Example: ATM state machine

Design a state machine in UML to represent the function of an ATM machine
(Automated Teller Machine).
Identify the different working state of the system:
● Waiting
● Mainteinance
● ‘’out of order’’
● Interaction with the user during withdrawal


# The italian CUP

The Booking Service is a crucial help for patients and health institutions. It is aimed at
assuring an effective and efficient way to reserve medical examination decreasing the
waiting time for the patients.

## Motivations behid the CUP

**1. RISKS:** long​ waiting lists aggravate patients’ conditions and limit the possibility
    to access the required periodic controls
**2. RESOURCES:** ​Limited diagnostic and therapeutic resourses
**3. DISTRIBUTION:** ​Territorial dispersion of resources
**4. MANAGEMENT of MULTIPLE VISITS FOR EACH PATIENT
5. OPTIMIZATION IS NEEDED (USER CENTERED APPROACH):** ​The patient has
    to decide when and where depending on his/her needs
**6. FOLLOW-UP** :​ It is important to execute the new exam exactly in the same
    place in which the first was carried out in order to assure:
       a. Repeatability of the results
       b. Reliable longitudinal comparison
**7. STANDARD TERMINOLOGY** ​: It is necessary to use the same terms for
    prescriptions and diagnostic exams
**8. DIFFERENT CONSTRAINTS FOR DIFFERENT EXAMS** ​: It is needed to maintain
    the execution of the interventions similar in all the institutions to optimize the
    organization limiting the waste of time

## The booking service


## The phases of the booking


## Offer definition

The implementation of the booking service process is complex because it requires the
implementation of the architecture. We need to know all of the information of the
institutions included in the CUP:
● Creation of a central database including all of the information on available
resources, examinations, specific schedules
● Creation of a database for each institution that can be accessed by means of a
common central software
Each institution has to define the offer comprehending:
● Executable examinations
● Resources available with their maintainance period
So, for each examination the information will be:
Code Name Constraints Admin data Duration Working load
(daily, weekly,
monthly)
Logistics
availability
(frequency,
duration)
The offer will be modeled as:


## UML modeling guidelines

```
1) Identify the requirements: ​ Use case diagram
2) Specify the dynamic behaviour of the main use cases: activity, ​ sequence or
statechard diagram
3) Identify classes and relationships according to the model objective: class ​
diagram
```
## Model

### Use case diagram


### Activity diagram

##### ACTORS INVOLVED

● Patient
● Booking Service Operator
● Booking Service Software and DataBase
**ACTIVITIES**

1. Call the booking service
2. Check patient’s rights
3. Ask for examination
4. Check for examination code in the prescription
5. Enquery the SW about examination availability
6. Send the record set (date and place)
7. Choose an available date and place
8. Communicate it
9. Book the examination for the chosen date and place
10.Update the institute scheduling for the examination
11.Generate the reservation number
12.Communicate the reservation number


### Sequence diagram

#### With CUP

#### Without CUP


### Class diagram

**Person** ​: generalization of
● Technician
● Doctor
● Patient
● Call center operator


# 1  Database basics and Data Base Management

# Systems (DBMS)

## 1.1 Database definition and properties

A database is a collection of related data with an implicit meaning that:
● Is logically coherent
● Is designed, built and populated with a specific purpose and intended users
● Represents osme aspects of the real world (it’s a model!)
There are some definitions to keep in mind:
**1) Data item** ​: known fact that can be recorded or measured (value)
**2) Field:** Each​ value is formed of one or more parts and corresponds to a
particular field
**3) Record:** ​collection of related data values
**4) File:** ​ collection of records
**5) Database** ​: collection of related data with an implicit meaning


Example of database with related data:

## 1.2 Database approach vs File processing approach

### Database Approach

```
● A single repository of data is created once and can be accessed by various
users
● The system contains a complete definition or description of the database itself
(​ Self-contained nature ​)
● Indipendence between programs and data
● Provide a conceptual representation of data (​ Data abstraction ​)
● Provide different perspectives for different user (​ Multiple views ​)
```
### File processing

```
● Each user defines and implements the files needed for a specific application
(​ Redundancy ​)
● Data definition is part of the application program (​ Data definitions
embedded ​)
● The structure of the data files is embedded in the application program
(​ Dependency between programs and data ​)
● Data are represented by the memory occupation/record length
● Each different user needs a differen application (​ unique view ​)
```

```
Database File processing
Not redundant Redundant
Self-contained nature Data definitions embedded
Indipendence programs/data Dependency programs/data
Data abstraction Data instantiation
Multiple views Unique views
```
## 1.3 Schemas and Instances in databases

Databases can be described by 2 different modalities:
**● Database schema** ​: the description of the database that is specified during
database design and is not expected to change frequently ( **intensional** ​ **aspect** ​).
The schema can be seen as the skeleton of the database’ structure.
**● Database instance** ​: An instance of a database is composed by the data in a
database at a certain time point ( **occurrence** ​ or​ ​ **state** ​). This is reffered as
**estensional aspect** .​ The database is moreover defined as “​ **empty instance** ”​
when it’s created. Once populated, data are loaded in the database.

## 1.4 Data Base Management System

A DBMS is a collection of programs that enables the users to create and maintain a
database. The major functions of DBMS software are:
**1) Define the database** :​ it involves specifying the data types, structures and
constraints for the data to be stored in the database;
**2) Construct the database** ​: constructing is the process of storing the data itself
on some storage medium that is controlled by the DBMS;
**3) Manipulate the database** :​ functions like query the database to gather specific
data, update the database and generating reports from the data.
DBMS have multiple properties:
1) They can handle huge amount of data (GB, TB)
2) They provide persistent storage for program objects and data structures.
Persistent data have extended lifetime that goes beyond the execution time of
the applications that use the database


```
3) They handle sharing of data and they can manage deltas of updates, also called
Concurrence control. In other words the software can control the
contemporary update by several users resolving occurring conflicts.
4) They control redundancy among data
5) They provide backup & recovery functions, which make the system reliable
6) They restrict unauthorized access providing security and authorization
subsystems that allows creating accounts and specifying their restrictions aka
privileges
7) They provide multiple interfaces. This is the way the database presents
multiple point of view: multiple users can access the database at the same
time. Every user will have a specific data view, specific language and specific
interface. There can be 6 different type of interface:
a) Menu-based: list of options
b) Graphical
c) forms- based
d) Natural language interfaces
e) For parametric users
f) DBA interfaces
8) They represent complex relationships among data, the database should hence
represent all the possible relationships existing
9) They enforce integrity constraints: in particular, data should be consistent and
constraints can be represented by relationships or unique values too.
```
## 1.5 DBMS Actors

There are 4 main classes of actors involved in DBMS softwares:
**1) DBA** ​: responsible of the management of the database
**2) DB Designer** ​: responsible of choosing the data to be saved in the database and
the appropriate structure to manage them
**3) End users** ​: classified in
a) Casual end users
b) Naive or parametric end users: users who mainly query and update the
database
c) Sophisticated end users: use the database but also understand the
complex requirements behind
**4) System analysts and application programmers** ​: study the requirements of
the end users and develop specification transactions to meet such
requirements. They also implement the specifications
There is also another class of actors, who are “behind the scene”. They are
represented by DBMS/tools developers, operators and mainteinance personnel


## 1.6 DBMS architecture

A DBMS is implemented through a three-schema architecture, organised as follows:
**● Internal level** ​: internal schema that describes the physical storage structure of
the database. It includes the complete details of data storage and access paths
of the database.
**● Conceptual level** ​: it describes the structure of the whole database (hiding the
details of the physical storage)
**● External level** ​: it describes the database biew for a specific user group.
Thanks to this architecture, a DBMS provide different advantages:
**● Self-describing nature:** The​ Database is made self-describing by the use of a
catalog to store its schema. This catalog contains information such as the
structure of each file, the type and storage format of each data item, and
various contraints on the data. The information stored in the catalog is called
meta-data, it describes the structure of the primary database.
**● Data independence:** capacity to change the schema at one level of a database
system without having to change the schema at the other levels. Composed by
**○ Logical data independence** :​ capacity to change the conceptual schema
without having to change external schemas or vice-versa.
**○ Physical data independence** :​ capacity to change the internal schema
without having to change the conceptual schmas
**● Support of multiple user views
● Sharing of data and multi-user transaction processing
● The database provides a unified view on real world data once defined
● Centralized control on data
● Reducing redundancies and inconsistencies**
Is it also possible to define 2 limits of DBMS:
1) Costs
2) DBMS cannot be mixed-up

## 1.7 DBMS Languages

```
● Data Definition Language ( DDL ​ )​ Language for data defnition, the DDL is used
to specify conceptual schema for the database.
● Storage Definition Language (​ SDL ​) Language for data storage, the SDL defines
the internal schema (physical storage of the data).
● View Definition Language ( VDL ​ )​ Language for view defininition, the VDL
specifies user views and their mappings.
```

```
● Data Manipulation Language ( DML ​ )​ Language for data manipulation, the MDL
can be:
○ high-level non procedural (does not define how the result is obtained
but what is wanted)
○ low-level procedural (defines the procedure to obtain the result)
```
## 1.8 DBMS classifications

DBMS can be classified through 4 ways:
**● Data model:** a​ collection of concepts that can be used to describe the structure
of a database
○ Relational
○ Network
○ Hierarchical
○ Object oriented
**● Number of contemporary users** ​: single or multi
**● Number of sites where the database is distribuited:**
○ Centralized DBMS
○ Distribuited DBMS
○ Federated DBMS
**● Cost**


# 2 Relational models

The relational model represents data in a database as a collection of relations.
Relations are represented as tables where the columns are the attributes and the rows
are the tuples. The set of values that an attribute can assume is the “domain” of that
attribute. Values inside of the domain are atomic and they are specified by a format.

## 2.1 Properties

Relations have different properties:
1) There is no order among tables in a relational database
2) There cannot be 2 identical tuples in a relation (​ **non-redundancy** ​)
3) Attributes in a relation are not ordered
4) A relation is characterized by:
**a) Relation schema** ​: relation name and attributes (relation intension).
Relation schema is also expressed by the symbolic expression:
_R_ ( _A_ 1 , _A_ 2 , ..., _An_ ) where R is the relation (table) name and _dom_ ( _Ai_ ) is the
domain of the i-th attribute. N is the degree of the relation (number of
attributes). It is also possible to simply refer to a relation with the
following notation: _R_ ( _x_ ) where _X_ ={ _A_ 1 , _A_ 2 , ... , _An_ } is the attribute set
**b) Relation instance** ​: tuples containing actual data (relation extension)
With the same notation as the one for the relation schema, it’s possible to define the
database schema as an expansion of a relation schemas:
_R_ = { _R_ 1 ( _X_ 1 ), _R_ 2 ( _X_ 2 ), ..., _Rn_ ( _Xn_ )}
Where:
● R is the database name
● Ri is the table name
● Xi is the attribute set
So for example, the database of an hospital can be modelized as:
Hospital= {Patients(name, surname, tax ID,...), Operative Units(name,
location, director, ...),...}
Summarizing, a relation is defined as a set of tuples in which two tuples cannot be
identical (each tuple is unique). It means that there cannot be two or more tuples
with the same combination of values.


## 2.2 Keys

In relational models is possible to identify:
**● Superkeys** ​: a subset of attributes in a relation that is unique for each tuple
(​ **superkey univocally identifies a tuple** ​)
**● Keys** ​: minimum superkey, i.e. a superkey for which it is not possible to identify
a subset of attributes satisfying the unicity property
For example:
{FirstName, LastName, BirthDate, BirthPlace, GP} -> SUPERKEY because it identifies
one single tuple
{FirstName, LastName, BirthDate, BirthPlace} -> KEY because it doesn’t identify one
single tuple
Among those keys, it has to be selected one key to identify the tuples in a relation,
which is called the ​ **Primary Key** ​ (highlighted by the “ % “ symbol). For example:
Hospital= {Patients(name, surname, tax ID,...), Operative Units(name,
location, director, ...),...}
Primary key for the relation “Operative Units” can be, for example a set of attributes
defined as such:
{name, OU_ID}
Doing so, the relation will be written as:
Operative Units { name%, location, director, OU_ID% }

## 2.3 Integrity constraints

The concept of integrity constraints derives from the observation that not all value
combinations are able to represent the information correctly. The introduction of
integrity constraints ensures that the information represented is correct.
There are 2 types of constraints:
● Intra relational constraints
○ Tuple contraints: constraints on the values of each tuple (NOT NULL,
valid interval,...) express conditions on the values of each tuple


```
independently from the others (es. grades at university exams in the
range [18, 30] and 30 cum laude); attribute NOT NULL.
○ Key constraints: no primary key value can be null.
● Inter relational constraints
○ Referential integrity constraint: used to mantain the consistency among
tuples of two relations. It’s based on the concept of “foreign key”. A set
of attributes FK in the relation R! Is foreign key of R1 if:
■ The attributes in FK have the same domain as the primary key
attributes PK of another relation R2
■ A value of FK in a tuple t1 of R1 either occurs as a value of PK in
some tuple t2 in R2 or is null ( t1[FK] = t2[PK])
```
## 2.4 NULL value

The NULL value have multiple meanings:

1. Not valid for the current instance (Husband surname for a male)
2. Valid but not yet existing (Husband surname for a non-married woman)
3. Existing but it cannot be saved (patient’s religion in some Countries cannot be
    stored to avoid discrimination)
4. Existing but unknown
5. Existing but not yet saved (patient’s history not collected yet)
6. Stored and then deleted (erroneous information)
7. Available but in an updating phase (patient’s therapy under modification)
8. Available but not reliable (a non final diagnosis)
9. Available but not valid (a blood parameter above the threshold of valid range)
10.Calculted from another NULL value (BMI if the weight is not present).


# 3 Relational Algebra

## 3.1 Definition

Relational algebra is a procedural language that specieifes the steps needed to obtain
a result. It defines a set of operations used to manipulate entire relations.

## 3.2 Select operation σ

Is used to select a specific subset of tuples in a relation. These tuples must satisfy a
selection condition. The result is a new relation with the same attributes as the
starting relation and only the selected tuples.
A select operation is written in this way:

_New Relation_ ←σ( _condition_ )( _Relation Name_ ) (^)
_Usually the condition is a comparison operation with constant values and Boolean
operators_

## Example

We want to select the Cardiology patients
The operation will be:

_New patient_ ←σ( _Operative Unit_ = " _Cardiology_ ")( _Patient_ ) (^)
Result will be a new relation with the same attributes and filled only with the tuples
satisfying the condition:


## 3.3 Project operation π

The project operation is used to select certain attributes from the table and discard
the other columns. The result is a new relation with the same tuples but different
attributes:

_New relation_ ←π( _attribute list_ )( _Relation name_ ) (^)

### Example

We want to select the Name, Surname, and date of Birth
The operation will be:

_New patient_ ←π( _Surname_ , _Name_ , _Birthdate_ )( _Patient_ ) (^)
Result will be a new relation with the same tuples but only the attributes listed in the
selection criterion:

## 3.4 Union operation

It operates over two relations (R1 and R2). The result is a relation that includes all the
tuples that are either in R1 or in R2, counted only once (duplicate tuples are
eliminated):

_New relation_ ← _R_ 1 ⋃ _R_ (^2)


The union operation is feasibile only when the two relations are “union compatible”.
It means that the two relations have the same number of attributes and each attribute
pair has the same domain.

## 3.5 Intersection operation

It operates over two relations and the result of this operation is a relation that
includes all the tuples that are both in R1 and in R2:

_New relation_ ← _R_ 1 ⋂ _R_ (^2)

## 3.6 Set difference operation

It operates over two relations and the result is a relation that includes all tuples that
are in R1 but NOT in R2:

_New relation_ ← _R_ 1 − _R_ (^2)
In this operation the order of the relations is relevat, it’s not commutative.

## 3.7 Cartesian product operation

It operates over two relations which don’t need to be union compatible. The result of
this operation is a relation that:
1) Combines all the tuples from R1 and R2 and
2) Has all the attributes of both R1 and R2

_New relation_ ← _R_ 1 _XR_ (^2)
The result per se does not have a real meaning but it is a matematical tool.

## 3.8 Join

It operates over two relations. The result of this operation is a relation that:
1) Combines related tuples from R1 and R2 into single tuples and
2) It is a cartesian product followed by a selection

_New relation_ ← _R_ 1 ⨝ (^) ( _condition_ ) _R_ 2 


### Example

We want to calculate the result of the Join operation between:
The operation will be:

_Pat_. _Dia_ ← _Patient_ ⨝ (^) ( _ID_ = _Pat_ − _ID_ ) _Diagnosis_ (^)
The new relation will be:
As we can see, the relation contain all tuples satisfying the condition. It is the same
result as the selection of the tuples where ID=PAT_ID after a cartesian product of
Patient and Diagnosis:

### Pat. Dia ←σ( ID = Pat − ID )( PatientXDiagnosis )


## 3.9 Natural join

It operates over two relations and the result is a relation that:
1) Combines related tuples from R1 and R2 into single tuples, but the set of
common attribute is unique
2) It is a cartesian product followed by a selection and a projection

_New relation_ ← _R_ 1 ⨝ _R_ (^2)

### Example

_Pat_. _Dia_ ← _Patient_ ⨝ _Diagnosis_ (^)
The new relation is the same as the one obtained in the previous join operation, but
the patient ID appear only once.
It is the same result as the selection of the tuples where ID=PAT_ID after a cartesina
product of Patient and Diagnosis and projecting all the attributes except Pat_ID (the
condition for the previous Join).


## 3.10 Rename operation

It operates over single relations and it allows giving new names to the attributes of a
relation. The result is a relation that has the same attributes as the original one but
with different names.

_New relation_ ←ρ( _renaming criteria_ )( _Relation Name_ ) (^)
_Where renaming criteria are in the form:
B_ 1 , _B_ 2 , ..., _Bn_ ← _A_ 1 , _A_ 2 , ..., _An_


# 4 Hierarchical and network data models

Representational data models are known also as “logical” data models because data in
the database are organized following a logical structure. In particular, in hirearchical
models data are organized in trees, while in network models, networks and graphs
are used.

## 4.1 Properties

A hierarchical schema is composed by two elements:
1) Record types
2) Parent-Child Relationships (PCR) type: the cardinality is always 1:N
Among these,there are some additional definitions:
● Root: record type that is never child record type in any PCR type
● Other types:
○ Participate as child record type in only one PCR type
○ Participate as parent record type in N PCR type (0..N)
● Leaf: record type that never participates as parent record type in any PCR type
Furthermore, if a record type participates as parent in more than one PCR type, then
its child record types are ordered from the left to the right

## 4.2 Occurrence tree

Hierarchical data models are represented with occurrence tree:


For example in the example above the record type Patient_LastName_FirstName,
which takes “john Smith” value, is parent for the records at lower level such as
“diagnosis”, which takes “eye inflammation” or “headache” values and is the record
child. The relation among them is 1:2 because a single parent record is related to two
record child of type diagnosis.

## 4.3 implementation considerations

Structure of the Hierarchical model does not come from standards. Infact:
● The hierarchical data model does not have a standard language
● The DBMS that implement a hierarchical data model are based on lower-level
languages (IBM’s Information Management System, ‘60) That modify only
single records
● Only relations 1:N (duplications/redundancies)
● The access to data is quick only when the information can be reached with a
sequential strategy (following the tree)
○ Example:
■ Find the prescriptions of patient John Smith FAST
■ Retrieve the list of all the patients who had a certain prescription
SLOW first you have to reach the patient and then explore it (all
patients)

## 4.4 Network Data Model-basic structures

Network data models use:
● Records
○ Data are stored in records
○ Records are classified in record types
○ The record type describe the structure of a group of records that stores
the same kind of information
○ Each record has a name
○ Each data item (atribute) has a name and a type


● Sets
○ Is a 1:N relationship
○ Characterized by a name, an owner record type and a member record
type
○ Represented by an arrow
Some properties:
● CODASYL DBTG (COmputer DAta SYstem Language – Data Base Task Group
Comitee who defined the standards)
● Useful in the cases when there are different viewpoints:
○ Patient (interested in the healthcare operators that are involved as
careres)
○ Clinician (interested in all their patients)
○ Ward (interested in keeping track of the treatments of all the patients in
the ward)
○ Drug (interested in “knowing” which patients are treated with such
drug)
● None of these profiles is dominant


## 4.5 Weaknesses

A network database idea is more suitable to the conditions with multiple viewpoints.
However also the network databases have weaknesses:
As principle, at any stage they deal with all the data to be scanned by queries. This is
true also when all such queries belong to a specified application subset, where a large
part of the stored data will never be considered objects of any analysis.
An example is the administrative data: they will never be of interest in a clinical
query.
A second example is the full set of identification data, including those that may vary
over time, like the street address and the telephone number. Mainly these last data
are needed only for sending mails to the patient home.


# 5 Database design methodology

## 5.1 Database lifecycle and design methodology

The database lifecycle is a complex process, usually composed by the following main
phases:
1) Requirements collection and analysis
2) Conceptual database design
3) Choice of a DBMS
4) Logical database design
5) Physical database design
6) Database implementation
7) Use & maintenance

## 5.1.1 Requirements collection and analysis

In this phase the need is to collect knowledge of the needs, requirements,
expectations of the final users, details about the use and identification of the different
views on data. Moreover:
● Identification of homogeneous groups of users
● Review of the existing documentation related to the information and the
operations of the DB
● Analysis of the operative environment and the use of the data
● Analysis of questionnaires and interviews for priorities and expectations
At the end of this phase: collection of pieces of information which are not structured
and are often in natural language.
It is also needed to utilize process modeling tools, to have interaction with domain
experts and to identify use-cases.

## 5.1.2 Conceptual database design

This phase is independent from the DBMS that will be used, and it provides an high
level and abstract view of the reality. This phase is composed by
1) Conceptual design: from requirements to a conceptual schema. It leads to the
E-R model
2) Design of transactions
The Entity-Relationship (E-R) Data Model is a conceptual design of the database.
“Entity” is an independent object or entity of the real world. “Relationship” is an
association between more entities.


The relationship cardinality have to be specified for each entity participating in a
relationship. They describe the minimum and maximum occurrencies of each entity
istance in a relationship. They define how many times each entity istance can be
involved with other entities through the specified relationship.


In ER models is it also possible to have generalization. It relates one or more entities
with a single entity which includes them as specific cases. There are some properties
to consider; if E (parent) is generalization di E1, E2, ..., En (children):
● Any property of E is property of E1, E2, ..., En (including relationships)
● Any occurrence of E1, E2, ..., En is occurrence also of E
● Any property (attributes, relationship, other generalizations) of the parent are
inherited by the children entities and are not explicitly represented
There can be 2 types of generalizations:
1) Total: Each occurence of the parent entity is occurrence of at least one of the
child entities
2) Exlusive: Each occurrence of the parent entity is occurrenc of at most one of
the children entities

### 5.1.3 Choice of a DBMS

It includes:
● Choice of the representational data model:
○ Hierarchical
○ Network
○ Relational
○ Object Oriented
● Technology
○ Proprietary vs Open source
○ Compatibility with the general system specifications
○ Total size manageable
○ The type of physical storage strategy
○ Data model used by the DBMS
○ Interfaces available for users and designers
● Cost
○ Costs for purchese(Free vs license) and maintenance
○ Licensing schema (single, multiple, enterprise)
○ Training of personnels
● Other features (easy access control, versioning, etc)

### 5.1.4 Logical database design

This phase translates the abstract representation of the conceptual model in
specifications that can be implemented through a DBMS. The result is the logical
schema. It consists of 3 sub phases:


1. Translation from the conceptual schema to the logical schema using the DBMS
    data model
2. Adaptation of the logical schema to the characteristics of the specific DBMS
3. Logical schema optimization, called “Normalization”


### 5.1.5 Physical database design

Choice of the specific data storage structures and data access modalities to obtain an
efficient system. The coice depends on:
● Response time
● Memory occupation
● Average number of transactions per minute

### 5.1.6 Database implementation

The specific database languages are used to implement the database:
● DDL
● SDL
● DML
● VDL

### 5.1.7 Use&Maintenance

Aspects to consider:
● Everyday use by final users
● Database administrators are responsible for mainteinance
○ Change of the needs
○ More data
○ New users ecc..


# Standards in medical informatics

Interoperability is the ability of different systems to work cooperatively allowing
different users to share information and resources.
Standards are defined as a set of rules and definitions which specify how to carry out
a process or produce a product. Standards are created and used to make things or
processes work more easily and economically (or to work at all). They also permit two
or more disassociated people/parts to work in some cooperative way.
There are 4 methods to develop standards:

**1. Ad hoc** ​:
    a. A group of interested people and organizations agree on a standard
       specification
    b. These specifications are informal and are accepted as standards
       through mutual agreement of the participating groups (DICOM)
**2. De facto** ​: A single vendor controls a larghe enough portion of the market to
    make its product the market standard (microsoft windows)
**3. Government- mandate method** :​A government agency creates a standard
    and legislates its use (HCFA and UB-92 insurance-claim forms)
**4. Consensus method** ​: A group of volunteers representing interested parties
    work in an open process to create a standard (HL7)
The standard definition process ensures:
● AGREEMENT: Standards are created upon agreement because there was a
consensus among who participated to the working group
● DEMOCRACY: all the interested stakeholders can participate to the working
groups and make observations and suggestions
● TRANSPARENCY: standardization bodies make the process and the different
steps avaiable to the public who is interested
● VOLUNTARY: Norms are a reference that the interested stakeholders
voluntarily adopt.

# HL7

Founded in 1987, Health Level Seven International (HL7) is a not-for-profit,
ANSI-accredited standards developing organization dedicated to providing a
comprehensive framework and related standards for the exchange, integration,
sharing, and retrieval of electronic health information that supports clinical practice
and the management, delivery and evaluation of health services. HL7's 2,300+
members include approximately  500  corporate members who represent more than
90% of the information systems vendors serving healthcare.


HL7 creates healthcare standards to enable interoperability of healthcare
information. In particular:
● Messages and documents move healthcare information in a standardized way
to the point of patient care.
● Standards assist in moving information within and beyond the four walls of
hospitals and clinics among all healthcare stakeholders.
● Standards assist in the sharing of public health information.
● Standards help enable the electronic health record and creation of a National
Health lnformation Network.
● HL7 assists in using genomic data in conjunction with other clinical
information
It’s important to highlight that HL7 does not create or provide any sort of software. It
does provide healthcare organizations with specifications for making their systems
interoperable. HL7 adopted strategies to develop specifications for making healthcare
systems interoperable. Among those, the most important are:
● Develop coherent , extendible standards and a format methodology.
● Collaborate with healthcare information users and other standards
development organizations.
● Promote the use of HL7 standards wortdwide.
● Educate the healthcare industry and policy makers.
● Enable domain experts from the healthcare industry to develop healthcare
information standards in their areas

## HL7 reference categories

HL7 standards are grouped into reference categories:
**1) Primary standards:** Primary​ standards are considered the most popular
standards integral for system integrations, inter-operability and compliance
**2) Foundational standards** ​: Foundational standards define the
fundamentaltools and building blocks used to build the standards, and the
technology infrastructure that implenters of HL7 standards must manage
**3) Clinical and administrative domains** :Messaging​ and document standards for
clinical specialties and groups are found in this section. These standards are
usually implemented once primary standards for the organization are in place
**4) EHR profiles:** These standards provide functional models and profiles that
enable the constructs for management of electronic health records
**5) Implementation Guides:** This​ section is for implementation guides and/or
support documents created to be used in conjunction with an existing
standard. All documents in this section serve as supplemental material for a
parent standard.
**6) Rules and references** :​ Technical specifications, programming structures and
guidelines for software and standards development


```
7) Education & Awareness: ​resources and tools to further supplement
understanding and adoption of HL7 standards
```
## HL7 communication workflow

1) The data exchange protocol is based onASCII-coded messages delimited by
“separators”;
2) Two actors (sender and receiver) communicate throgh the exchange of
bi-directional messages;
3) The message content is validated by a parser before the transmission: first, the
parser adds missing parts, then the message is transmitted;
4) The receiver decodes the message according to the protocol rules and
interprets the data type extracting all the relevant information from the
message;
5) Messages are independent from the system implementations
6) heterogeneous systems can communicate withouth knowing each other;
7) The receiver always sends an Acknowledge (ACK) message to confirm the
reception.
The HL7 vs communication workflow is activated by a trigger event: an explicit set of
conditions that initiate the transfer of information between system components (real
world event).
Examples: the placing of a laboratory order or drug order:


The Trigger Event may be caused by one of the following reasons:
● User Request Based (the trigger event that prompts a system to send all
accumulated data to a tracking system every  12  hours; a user pressing a
button in a user-interface)
● State Transition (the trigger for canceling a document)
● Interaction Based (the response to a query)

## Message structure

● Message:
○ Delimited ASCII text
○ Composed by one or more Segments
● Segment
○ Text line delimited by the carriage-return
○ Can be optional
○ Composed by one or more fields delimited by the pipe character “|”
● Fields:
○ Composed by data or strings separated by “^”
○ They can be empty
○ The NULL value is the empty string “”
Each message should contain the following segments:
1) Meassage header (MSH)
2) Event Type (EVN)
3) Patient Identification (PID)
4) Patient Visit (PV1)


Example:


# DICOM

DICOM - Digital lmaging and Communications in Medicine - is the international
standard for medicai images and related information (ISO 12052, 2006). lt defines the
formats for medical images that can be exchanged with the data and quality
necessary for clinical use. DICOM is implemented in almost every radiology,
cardiology imaging, and radiotherapy device (X-ray. CT, MRI, ultrasound, etc.), and
increasingly in devices in other medical domains such as ophthalmology and
dentistry. With tens of thousands of imaging devices in use, DICOM is one of the most
widely deployed healthcare messaging standards in the world. There are literally
billions of DICOM images currently in use for clinical care. Since its first publication
in 1993, DICOM has revolutionized the practice of radiology, allowing the replacement
of X-ray film with a fully digital workflow. Much as the Internet has become the
platform for new consumer informatian applications, DICOM has enabled advanced
medical imaging applications that have "changed the face of clinical medicine". From
the emergency department, to cardiac stress testing, to breast cancer detection.
DICOM is the standard that makes medicai imaging work- for doctors and for
patients.

## Aims

The DICOM model was developed to define the communication interface between a
PACS (Picture archiving and communication System) and a Hospital Information
System (HIS) or a Radiology Information System (RIS).
In this context, the communication was not only a point-to-point communication, but
also heterogeneous systems have to be connected, having different interfaces and
producing different data formats.
This standard is responsible for governing both the image format as well as the
various network protocols required for transmission of medical image information
generated during the many healthcare-related imaging “modalities”

## Architecture

DICOM currently defines an upper layer protocol (ULP) that is used over TCP/IP
(independent of the physical network), messages, services, information objects and an
association negotiation mechanism.
These definitions ensure that any two implementations of a compatible set of services
and information objects can effectively communicate.
Independence from the underlying network technology allows DICOM to be deployed
in many functional areas of application:


```
● a single site (Ethernet)
● between sites (VPNs, MANs)
● across dial-up or other remote access connections (such as by modem, ISDN or
DSL)
● via satellite (with optimized protocol stacks to account for increased latency)
```
## Services

DICOM standard is based on the concepts of:
● Service providers = Service Class Providers or SCP, e.g. a printer
● Service consumers = Service Class Users or SCU, e.g. an application requesting
the printing service
● Information objects that are acted upon by the providers and consumers, e.g.,
the bio-images
● Service-Object Pair (SOP) = The combination of a service class along with the
information object
○ SOPs form the foundation for DICOM-related compliance (or
“conformance”), and allow vendors to disclose what DICOM- related
capabilities their software and hardware support.
○ Each SOP class has a unique identification number issued by the DICOM
committee.

## Image format

The DICOM file contains patient identification information, study and series
information, information of the image acquisition, pixel data.
All this information is stored in the form of data sets. Data sets are a collection of data
objects attributes in the form of name/value representations. The attributes are
maintained/managed through a DICOM Dictionary.

## Conformance

DICOM adherence is described by vendors through a Conformance Statement
describes how their device or software supports the standard.
The information in the conformance statement include how the associations are
handled, the SOP classes that are supported, as well as other information such as
presentation contexts and communication profiles. Customers can use the
information contained in these documents to decide whether the vendor product can
successfully communicate with other DICOM-compliant devices or software within
their network.


# IHE

IHE is an initiative by healthcare professionals and industry to improve the way
computer systems in healthcare share information. IHE promotes the coordinated use
of established standards such as DICOM and HL7 to address specific clinical needs in
support of optimal patient care. Systems developed in accordance with IHE
communicate with one another better, are easier to implement, and enable care
providers to use information more effectively.
IHE is not a communication standard it has the aim to define how the available
standards have to be used in practice to implement system integration:
● To facilitate health information integration;
● To provide support functionalities for EHRs;
● To boost standard adoption;
● To promote the communication among vendors;
● To improve efficacy and efficiency in clinical practice;
● To improve ICT security and privacy;
IHE is organized by clinical and operational domains. In each domain users with
clinical and operational experience identify integration and information sharing
priorities and vendors develop consensus, standards-based solutions to address them.
Each domain includes :
● a technical committee, whose primary task is developing and documenting the
solutions (= integration profiles).
● a planning committee whose aim is long-term scope planning and organizing
deployment activities.
Each domain develops and maintains its own set of Technical Framework documents.

## Profiles

A profile is an abstract representation of the real world that defines the
implementaion specifications of one or more “use cases”:
● Communication processes
● Type of information exchanges
● Actions to be done when the information is received
Each profile is characterized by:
● ACTORS: healthcare information systems that mange the communication
activities (es. ADT, Order Placer, Order Filler, etc.);


● TRANSITIONS: standard-based information exchange among actors (ex. HL7).
Each transaction is characterized by the refernce standard and other
information.
In each profile, a table lists the actors and the transactions of the specific case.


# Evidence based medicine and protocols

**Evidence based medicine** integrate individual clinical expertise with the best
available external clinical evidence from systematic research.
**Protocols** ​ are a set of predefined actions that provide the best way to do something.
The combined use of those have as result a standardized and controlled medicine to
optimize the treatment of the patient. Expression of this medicine is represented by:
● Clinical practice guideline: document that contains recommendations or
strategies to assist healthcare practitioners and their patients in making
decisions about the management of healthcare for a specific clinical condition
or circumstance.
● Protocol: more prescriptive version of a guideline that contains a very explicit
set of instructions that should be followed. These precise instructions may
describe the procedure to be followed when investigating a particular set of
findings in a patient or the method to be followed in the management of a
given disease

## Clinical guidelines: sources and uses

Mainly AHRQ site which provides evidence-based guideline database or also NGC site.
Guidelines are based on evidence that is collected in the literature and in randomized
controlled trials. Another method used in literature are meta-analyses, a method that
pools the results from multiple similar experiments in the hope that the improved
power obtained from the combined data sets will identify statistically significant
patterns that cannot be identified within the smaller sample sizes of individual
studies.

## Computer-based guidelines design

The combined use of protocols and informatics lead to computer based protocols.
Actors involved in this type of protocols are:
● Clinicians
● Researchers
● Medical informaticians
● Patients
The medical guideline lifecycle is divided in 5 steps:
1) Conceptual modeling
2) Authoring process


```
a) Structured authoring of guidelines
b) Markup & adaptation of text guidelines
c) Testing & validation
3) Dissemination
4) Implementation
a) Adaptation to local preferences
b) Integration with operational system
5) Use & Update
```
## Design infrastructure for clinical guidelines

The design infrastructure for clinical guidelines is composed by 4 parts:

1. Preliminary consideration: investigation about adoption of a computerized
    guideline system. It is necessary to verify:
       a. Available instrumentations
       b. Health information systems in the ligh of embedded guidelines
2. Building yard
    a. Current version of guideline contents
       i. Text format or executable format
ii. Also guidelines in intermediate state (between text and
executable)
    b. Text fragmentation and framing
       i. Translation text exe
ii. Representation of the textual form of the protocol in a specific
language (UML – Unified Modelling Language)
iii. XML format can be used
    c. Tools for dictionaries
       i. Standardized medical terms
ii. Do not need concept “translation”
    d. Risk analysis
       i. Minimize recovery time
ii. Analyze all the possible risk situations
    e. E-mail
       i. Communication systems to reach medical expertises (cooperative
          systems)
    f. Programming languages
       i. Guidelines implementation
ii. Examples: Arden Syntax, Protegè
3. Delivery bus
    a. Access list
       i. System protection
ii. Different responsibilities user’s view
iii. Electronic sign, audit trail, timestamps, ...
iv. Specific set of actions/operations/views for each kind of user
    b. Emergency


```
i. Guideline path can change in the case of emergency (inclusion
criteria in normal situation or in the case of natural disaster)
ii. In the emergency case also the access politics can change
c. Followed guideline path tracking
i. Tracking system (action, time, data, ...)
ii. Used for medical intervention evaluation and for outcome
measure
d. Execution engine
i. The implemented guideline is executed through the execution
engine
e. Parameters calculation
f. Software tool (storage and recovery)
i. Save/recover a certain guidelines in the system
ii. Recall and execute
g. preceding version of guideline contents
i. In a certain time frame a certain version of the guideline is used
you have several patients treated in that particular way
h. preceding version of software application
i. Problem of version updating
ii. Not all the old features are supported/compatible with the new
version
i. software tools for validation
i. Needed in every system
ii. More important in the medical field (every error is paid by the
patient)
```
## Computer-based guidelines systems implementation

The fundamental role of a protocol is to ensure a task is carried out in a defined and
repeatable way. Protocols find wide application in healthcare. Protocols have been
shown to improve the process of delivering care.
For what concerns care pathways:
● They are a structured multidisciplinary plan of care
● They translate guidelines or evidence into local structures
● They have timeframes or criteria that guide progression between stages
● They detail the steps in a course of treatment or care in a plan, pathway,
algorithm, guideline or protocol
● They standardize care for a particular clinical problem, procedure or episode
of healthcare in a specific population
Protocol refinement can be modelized by the three-loop model. This model describes
the way in which protocols can be used to manage individual patients in a uniform
way and use the result of treatment to grow clinical knowledge


Computer-based protocols can be classified in:
**● Passive protocol systems** :​ provide clinicians with access up-to-date guidelines
and provide access to best-practice documentation.
**● Active protocol systems** :​ they help applying guidelines in the management of
patients, guiding the actions of clinicians. Thanks to them, clinical activities
can be supported or even automated. Active protocol systems must be
integrated into the wider organizational information system. For these
systems, communication interfaces are needed to allow the sharing of
information between active protocol systems and other clinical systems.
Protocol-driven information systems can integrate into many different clinical
systems, with cumulative benefit. They can, for example, guide record keeping,
prompt alert generation, trigger automated order entry systems and
appointment scheduling and provide a mechanism for variance capture.

## Languages and implementation tools

**Arden Syntax** – Developed originally by the American Society for Testing and
Materials (ASTM), recognized standard for representing clinical and scientific
knowledge in an executable format. It is a part of the HL7 (Health Level 7) standard
set, Medical Logic Modules or MLMs no underlying ontology. This means that sharing
MLMs depends on making sure that variables have the same meaning when used in
different systems. Features:
● Implementation of medical knowledge bases
● Alarms and alerts generation
● Diagnosis interpretation
● Clinical studies screening


● Message delivery management
Files created with this syntax are composed by 3 modules:

1. Maintenance: file identification
2. Library: file content description
3. Knowledge: decision rules and actions
**PROforma** - ​ is designed to emphasize safe and robust guideline creation captures
both procedural and declarative aspects of a protocol into a set of tasks.
Distinguishing features of PROforma are the simplicity and intuitiveness of the
underlying task model
**Protégé** – is a widely used open source tool that allows a user to build a protocol,
guided by an ontology. Once constructed, the protocol is translated into a
machine-readable form. It comprehends:
● A suite of models and software components assists in writing guideline-based
applications
● A simple graphical interface to allow people to author a protocol
**Guideline Interchange Format (GLIF)** ​–is designed as an interchange format that
supports the sharing of guidelines among different institutions and software systems.
Based on Arden Syntax, its aim is to be a tool for guideline implementation in
different/shared informative systems (integration)

## System implementation tools

### Gem

Gudeline elements model, based on XML and developed by the Yale university. Its aim
is to create a model for guideline documents. It facilitates the translation thank to the
use of structured format.


### GLARE

GuideLine Acquisition, Representation & Execution, it’s a guideline implementation
system which aim is to support of the decision making process. Its major feature is the
“what if” service in which alternative choices are developed and virtually followed to
evaluate possible time, costs and resources. Its architecture is based on 3 layers:

1. System layer (interface): data acquisition and guideline execution
2. XML layer
3. Database Layer: data repository


# Open Data

Open data refers to the possibility of sharing data among users without particular
restrictions, the final goal is in improving services to the citizens and increase
capacity of research.
Encouraging and supporting data sharing is important for many reasons:

1. To reproduce research
2. Increase data reliability: improve quality of research and trust among
    researchers
3. Observational evidence base for clinics
4. Save economical resources
5. To make public assets available to the public
6. To allow others (scientists and non-scientists alike) to use existent data to
    answer new questions
7. To advance research and innovation
There is the need to define two type of data:
**● Personal Data** ​: any information concerning natural persons that are or can be
identified also by way of other items of information
**● Sensitive Data** ​: a personal data requiring special precautions on account of its
nature. A sensitive data is any data that can disclose a person's racial origin or
ethnicity, religious or other beliefs, political opinions, membership of parties,
trade unions and/or associations, health, or sex life. Management of these
data, in Italy, is under the supervision of The Italian Data Protection Authority
(DPA) (Garante per la protezione dei dati personali)

## Legal issues

Recently DPA published the general rules and authorizations for the use of personal
data for scientific research: Autorizzazione n.9/2016: Autorizzazione generale al
trattamento dei dati personali effettuato per scopi di ricerca scientifica del  15 
dicembre 2016.
In general, the secondary use of clinical and physiological data is allowed, without
further authorization for statistical and research purposes given that the data are
properly anonymized.
Personal data can be sent to:
● EU member states: no specific limitations on data flows to or through these
countries
● non-EU contries: a personal data can be transferred if


○ Any of the conditions the DP Code is fullfilled
○ The transfer is authorized by the DPA on the basis of adequate safe
guards for the data subject’s rights
Apart from the above cases, no personal data may be transferred if the legal system of
the country the data is bound for or in transit through does not afford an adequate
protection level to individuals.

## Assess quality of data

Actual possibility of accessing data and reuse them for different purposes. Effective
open data strictly depend on:

1. Quality data collection
2. Validation
3. Evaluation and certification methods
4. Standards
In Italy, the Agenzia per l’Italia Digitale, assumes the **Berners-Lee  5  star** model for
quality assessment:
Best quality data correspond to LOD (Linked Open Data). This means linking and
sharing not only data, but also the resources, like ontologies, knowledge bases or
datasets. RDF (resource description Framework) links between data items from
different data sources to provide context.
Data quality is also regulated by the ​ **ISO/IECFDIS-25012 (data quality model)** ​ which:
● Define and evaluate requirements in the production, acquisition and
integrations of data
● Identify the criteria for quality assurance of the data


● Evaluating data compliance with national laws and or existing requirements
In the contest of data reuse for health research, quality of Open Data should also refer
to amount of erroneous or missing data and to completeness of related information,
such as details on the measure protocols, links to complementary data, etc. which are
needed for result interpretation.

## Open data in Regione Lombardia for Public

## Administrations

The objective is to make available to everyone the Region’s information assets, such
that large amount of information of public interest can be used by anyone to create
new services, perform studies and create applications.
This is the added value of open data: starting from the data that has been made
available, it is possible to create innovative services for the Region, favouring not only
transparency, but also participation and the collaboration between instituitions and
the private sector. Example of app created:

## Open data for Research

### Further information: ​Horizon 2020

Features of sharing data in research activiy:
+ To reproduce or to verify research
+ To make the results of publicly funded research available to the public
+ To enable others to ask new questions of extant data
+ To advance the state of research and innovation
+ To save economical resources
Modern research builds on extensive scientific dialogue and advances by improving
earlier work. The europe  2020  strategy for a smart, sustainable and inclusive


economy underlines the central role of knowledge and innovation in generating
growth.
Broader access to scientific publications and data therefore helps to:
● **Build on previous research results** ​ (improved quality of results)
● **Encourage collaboration** ​ and avoid duplication of effort (greater efficiency)
● **Speed up innovation** ​ (faster progress to market means faster growth)
● **Involve citizens and society** (improved transparency and LEGITIMACY of the
scientific process)


# Open data in Genomics

Genomics is a Big Data science and is going to produce more and more data.
The human genome project (HGP) led to the problem of sharing human genomics
data. Firstly, a joint policy from the National Genome research Institute and the
Department of Energy in 1991 released a public version of data generated by the HGP.
To protect participant’s privacy, all recognizable information had been removed
(de-identification of data). In 2004, however, it was demonstrated that a single
individual can be identified by means of less than one hundred single nucleotide
polymorphisms.
In 2006, the NIH established the Database of Genotypes and Phenotypes. It is a
controlled access database in which individual genetic data are retrivable only with
approval from a Data Access Committe.
Further restriction were applied because in  2008  it was demonstrated that single
individuals could be identified in aggregated data sets.

## Three examples of web-based personal genomic data

## sharing projects

## Consent Research

System through which users can donate their data to databases that remove
identifiying details. It then assign an identification number to all of the data from
each user and deliver the de-identified data to researchers, who must agree to broad
conditions designed to prevent harm to the data contributors. Moreover, data donors
must undergo a detailed informed consent process, including, for instance, watching
a six-and-a-half minute video that cannot be fast-forwarded.

## Free the Data

Project initiated by a consortium of organizations, managed by Genetic Alliance
which is a non-profit health advocacy organization.

## Genomes unzipped

Project in which its member publicly publish their own genomic data believing that
“doing good science means releasing complete data for others to investigate”.


Another example is given by the Personal Genome Project (PGP, 8/4/2017). It is a long
term, large cohort study which aims to sequence and publicize the complete genomes
and medical records of 100k volunteers, in order to enable research into personal
genomics and personalized medicine.

## Risks of Data Sharing

```
● Misuse of the data
○ Accreditation
○ Project approval
○ Data accessible but not downloadable
● Researchers may lack the expertise, resources or incentives to share their data
● Data often do not exist in transferable forms.
● Some data are not sharable for ethical or epistemological reasons
```
