---
status:
date: 
decision-makers: 
consulted: 
informed: 
---

# Proof of Concept program for ABC Limited's Complaint Management System

## Context and Problem Statement

This ADR will be documenting whatever decisions I make regarding the testing of my complaint management system proof of concept. Ideally the tests would need to be easy to make and would need to be able to test small parts of the system individually rather than the program as a whole. Testing smaller snippets of the program will allow for better bugfixing as the tests will be more focused on finidng specific issues with the program in each section, rather than doing a full runthrough of the program and potentially missing some bugs due to the length of each test as well as the tests being mostly surface level as they are meant to simulate how an end user would run through the program.
 
## Considered Options

* NUnit
* Selenium
* Playwright
* Manual

## Decision Outcome

I have decided to go with manual testing for the testing of my proof of concept as is seems to be the most efficient for use in my program. i believe it will be more effective than NUnut for me as i will be able to perform the tests myself faster than i would be able to create each init test, and although they could be less accurate than unit testing i will still be covering the same bases with both. Manual testing is much more effective for my project than using Selenium or Playwright as i need to be able to test each function of the website individually rather than doing a full user scenario run through of the program as while this would be useful for showinf how a user would encounter any issues, it would not cover  each component in nearly enough detail for it the be properly tested.

### Confirmation

## Pros and Cons of the Options
### NUnit
#### Pros

* tests will be more thorough than manual testing
* unit tests allow for better testing than end to end as it tests individual parts of the program

#### Cons

* Takes time to write out each unit test
* could end up more complex than manually doing the tests due to needing to be more precise when making the unit tests

### Selenium/ Playwright (Both have the same issue)
#### Pros

#### Cons

* Only allows for End to End testing - need smaller tests

### Manual
#### Pros

* easy to perform, only need the code and to know what youre testing for
* quick to perform, no need to write out each test and then wait for it to be completed, can just perform the tests immediately

#### Cons

* most likely will be less accurate than doing unit tests using NUnit
