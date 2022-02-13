# Test Automation Guide


# Table of Contents
1. [Overview](#overview)
2. [Test case](#test-case)
3. [Automated test](#automated-test)


## Overview
List the basics of test automation in general

Note: I have avoid using definitions. Will try to explain this in my own terms.

-------

## Test case

#### what is a test case?
- Verification of a certain functionality based on requirements (specifications) or acceptance criteria

#### What does it contain?
1. Pre-requisite
   1. Setup for the test (eg: data setup or mocking or clean up)
2. Actions
   1. Eg: Making Rest API request
3. Validations
   1. Eg: Validation of the Rest API response

--

#### Why do we need to build/run a test case?
- Make sures that the piece of functionality is built correctly

--

#### What is needed to build a test case?
- Based on requirements or acceptance criteria

--

#### How to execute a test case?
- Manual tests
  - Eg: UI or Rest API (using Postman or SoapUI)
- Automated tests
  - Built-in tools (such as Robot framework, cucumber, Soap UI, etc)
    - May need to build functionality on top of the framework

--

#### Who is responsible to create and execute tests?
- Development team (Dev, SDET or/and QA)
- Misc (UAT tests)

--

#### Bonus:
- Single test case should verify only one concept as a good practice

-----

## Automated test

#### Why would you want to automate test cases?
- Reduce manual test as the application grows
- Gives you faster feedback on application quality
- No user errors

--

#### What are the characteristics of an automated test?
- It should be fast
- Should be repeatable
- Should give consistent result on consecutive runs
- Independent
- Gives flexibility to run same test case with different dataset

--

#### What kind of tests can be automated?
- Unit test
- Functional tests (Acceptance test, BDD, integration (within the component))
- End-to-end (Eg: distributed)
- Performance Test
- Much more

--

#### How to build one?
- Leverage commonly used existing tools, libraries
    - Eg: Junit, Cucumber, Selenium, Rest API (Httpclient, Request)

--

#### Who can build it?
- Software Engineers
- SDET, SET, QA Automation Engineers
- QA (BDD or some tool that is user-friendly)

#### When not to automate?
- If it is low Return Of Investment (ROI)
    - Eg: One time project, POC, etc
