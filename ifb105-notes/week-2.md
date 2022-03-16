---
description: >-
  Content here has been gathered from Week 2 tutorial, previous lectures and
  textbook content, feel free to add or mention any issues as more content
  becomes available too us :)
cover: >-
  https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2970&q=80
coverY: 0
---

# Week 2

### TLDR;

This week we cover the first 3 steps of CSDP:

| Step | Description                                                                             |
| ---- | --------------------------------------------------------------------------------------- |
| 1.   | Transform familiar information examples into elementary facts, and apply quality checks |
| 2.   | Draw the fact types, and apply a population check                                       |
| 3.   | Check for entity types that should be combined, and note any arithmetic derivations     |

## Week 2 Content:

### Elementary Facts

An elementary fact is a simple assertion, or atomic proposition, about the domain.\*

Examples of Elementary Facts are as follows:

* The **Patient** with surname ‘Lee’ has a **Temperature** of 37 Celsius.
* **Student** with the name 'Jane' was born in the **Year** '1990'.
* The **Athlete** with the name 'Jones EM' pole-vaults the **Height** of 400cm.

Elementary facts usually do not use logical connectives (e.g., not, and, or, if) or logical quantifiers (e.g., all, some).

Examples of incorrect Elementary Facts are as follows:

* Ann smokes **and** Bob smokes. - (Illegal, utilises logical conjunction).
* **All** people who smoke are cancer-prone. - (Illegal, utilises a logical quantifier).
* **If** Bob smokes **then** Bob is cancer-prone. - (Illegal, the statement is a conditional fact).

_\*Elementary facts are atomic. They cannot be split. A fact type represents one fact, regardless of its arity_

### Conceptual Modelling Method & Conceptual Schema Design Procedure (CSDP),

A **conceptual modelling method** comprises both a _modelling language_ and a _procedure_ describing how to use the language to build models.

A specification can be developed at the conceptual level using **Object-Role Modelling** (ORM).

The CSDP is performed in seven distinct steps:

| Step | Description                                                                 |
| ---- | --------------------------------------------------------------------------- |
| 1    | Transform familiar examples into elementary facts, and apply quality checks |
| 2    | Draw the fact types, and apply a population check                           |
| 3    | Check for entity types to be combined, and note any arithmetic derivations  |
| 4    | Add uniqueness constraints, and check the arity (length) of fact types      |
| 5    | Add mandatory role constraints, and check for logical derivations           |
| 6    | Add value, set-comparison and subtyping constraints                         |
| 7    | Add other constraints and perform final checks                              |

This week we only cover steps 1-3. If you would like to see an explanation of steps 4-7, please visit [Week 3](week-3.md).

### Basic Objects

Elementary facts assert that **objects** play roles. **Values** and **Entities** are basic objects.

#### Values:

A value is a constant that is self-identifying in the sense that when you see the constant written down in some context you always know what is being referred to. As a result, values can be referenced directly without identifying them with a description.

* E.g. character strings ('USA', 'Australia') and numbers (37, 5.38) are all values.

#### Entity:

An entity may be a tangible object (the City named ‘Brisbane’) or an abstract object (the Unit with code ‘IAB201’).

* E.g. - Australia has six states, "Australia" has nine letters.

### Entity Types and Reference Modes

