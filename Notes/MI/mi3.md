---
layout: page
title: DBMS
---

# 1  Database basics and Data Base Management

# Systems (DBMS)

## 1.1 Database definition and properties

A database is a collection of related data with an implicit meaning that:
* Is logically coherent
* Is designed, built and populated with a specific purpose and intended users
* Represents some aspects of the real world (it’s a model!)

There are some definitions to keep in mind:

**1) Data item** ​: known fact that can be recorded or measured (value)
**2) Field:** Each​ value is formed of one or more parts and corresponds to a particular field

**3) Record:** ​collection of related data values

**4) File:** ​ collection of records

**5) Database** ​: collection of related data with an implicit meaning




## 1.2 Database approach vs File processing approach

### Database Approach


* A single repository of data is created once and can be accessed by various
users
* The system contains a complete definition or description of the database itself
(​ Self-contained nature ​)
* Indipendence between programs and data
* Provide a conceptual representation of data (​ Data abstraction ​)
* Provide different perspectives for different user (​ Multiple views ​)

### File processing

* Each user defines and implements the files needed for a specific application
(​ Redundancy ​)
* Data definition is part of the application program (​ Data definitions
embedded ​)
* The structure of the data files is embedded in the application program
(​ Dependency between programs and data ​)
* Data are represented by the memory occupation/record length
* Each different user needs a differen application (​ unique view ​)



Database |File processing
---------|---------------
Not redundant |Redundant
Self-contained nature |Data definitions embedded
Indipendence programs/data| Dependency programs/data
Data abstraction |Data instantiation
Multiple views |Unique views

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

1. They can handle huge amount of data (GB, TB)

2. They provide persistent storage for program objects and data structures.
Persistent data have extended lifetime that goes beyond the execution time of
the applications that use the database

3. They handle sharing of data and they can manage deltas of updates, also called
Concurrence control. In other words the software can control the
contemporary update by several users resolving occurring conflicts.

4. They control redundancy among data

5. They provide backup & recovery functions, which make the system reliable

6. They restrict unauthorized access providing security and authorization
subsystems that allows creating accounts and specifying their restrictions aka
privileges

7. They provide multiple interfaces. This is the way the database presents
multiple point of view: multiple users can access the database at the same
time. Every user will have a specific data view, specific language and specific
interface. There can be 6 different type of interface:
  1. Menu-based: list of options
  2. Graphical
  3. forms- based
  4. Natural language interfaces
  5. For parametric users
  6. DBA interfaces
  7. They represent complex relationships among data, the database should hence
represent all the possible relationships existing
  8. They enforce integrity constraints: in particular, data should be consistent and
constraints can be represented by relationships or unique values too.

## 1.5 DBMS Actors

There are 4 main classes of actors involved in DBMS softwares:

**1) DBA** ​: responsible of the management of the database

**2) DB Designer** ​: responsible of choosing the data to be saved in the database and
the appropriate structure to manage them

**3) End users** ​: classified in
  * Casual end users
  * Naive or parametric end users: users who mainly query and update the
database
  * Sophisticated end users: use the database but also understand the
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

  * **Logical data independence** :​ capacity to change the conceptual schema
without having to change external schemas or vice-versa.
  * **Physical data independence** :​ capacity to change the internal schema
without having to change the conceptual schemas


Is it also possible to define 2 limits of DBMS:

1. Costs
2. DBMS cannot be mixed-up

## 1.7 DBMS Languages

● Data Definition Language ( DDL ​ )​ Language for data defnition, the DDL is used
to specify conceptual schema for the database.
● Storage Definition Language (​ SDL ​) Language for data storage, the SDL defines
the internal schema (physical storage of the data).
● View Definition Language ( VDL ​ )​ Language for view defininition, the VDL
specifies user views and their mappings.

● Data Manipulation Language ( DML ​ )​ Language for data manipulation, the MDL
can be:
○ high-level non procedural (does not define how the result is obtained
but what is wanted)
○ low-level procedural (defines the procedure to obtain the result)

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
attributes PK of another relation R
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
2) Has all the attributes of both R1 and R

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
