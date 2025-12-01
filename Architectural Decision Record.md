---
status:
date: 
decision-makers: 
consulted: 
informed: 
---

# Proof of Concept program for ABC Limited's Complaint Management System

## Context and Problem Statement
This ADR is for the proof of concept i will be making of the Complaint Management System for ABC Limited. this system would be created for banking and telecom companies to allow their customers to easily log complaints they have with the company in a placer that said company can easily access and respont to them. I will be creating a proof of concept for this program, involving the user being able to acces the system and link their bank account to the CMS in order to ensure they are sending complaints to the right company, as well as giving users the ability to write upo whatever complaint they have or possibly choose from a selection of generic complaints if their issue is nothing too specific.

## Considered Options

* Onion Architecture
* Layered Architecture
* Monolithic Architecture
* Ntier Architecture

## Decision Outcome

I have chosen to utilise a Layered architecture for the CMS proof of concept because it is going to be much easier to find and fix bugs within the system than using a monolithic architecture due to each component of the system being seperated into its own layer. The layered architecture is also going to work better than the onion architecture due to the scale of the project, as it is only a proof of concept the layered architecture will be faster to implement and the simpler nature of a layered architecture is beneficial for a proof of concept. It works well for the CMS POC as i can seperate each component of the CMS into layers, such as the login and complaint logging, making it easy to see how it flows through each layer before being saved to the database.

### Consequences

* Good, simple nature benefits the smaller nature of a proof of concept
* Bad, while the layered architecture is scalable, it is less scalable than other architectures such as the onion

### Confirmation

I have chosen the Layered Architecture

## Pros and Cons of the Options

### Layered

#### Pros:
* Easy to bugfix due to code being better structured
* Somewhat Scalable
#### Cons:
* Built around the database so that will be harder to change out

### Onion

#### Pros:
* Easy to bugfix due to layered nature
* Very scalable due to each part being swappable
* Database can be swapped without causing problems
#### Cons:
* More difficult to use, especially at a small scale

### Monolith

#### Pros:
* Easy to make/ very simple
#### Cons:
* Not scalable
* No components can be swapped out
* Bugs are harder to locate due to everything being in one .exe

### Ntier

#### Pros:
* components are seperated into tiers making bugfixes easy
* scalable due to tiers being able to have layers 
#### Cons:
* built around the database

