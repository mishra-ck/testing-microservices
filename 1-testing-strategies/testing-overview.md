Overview of testing
---
### What is a `Test Case` ?
A Test case is a set of inputs, execution conditions, and expected results developed for a particular objective,
Such as to exercise a program path or tp verify a cpmliance with specific requirement.

![image](https://github.com/mishra-ck/testing-microservices/blob/add-concepts/1-testing-strategies/Testing%20overview.png)

---
### Writing Automated Test Cases:
```
Automated test consists of 4 phases - 
1. Setup: Initialize the test fixture, which consists of System Under Test(SUT) and its dependencies, to desired initial state.
2. Execute: Invoke the SUT (ex: invoke method on class under test).
3. Verify: Make assertions about the invocation's outcome and the state of SUT.
4. Teardown:Clean up the test fixture if required (ex: case of DB test)
```
![image-2](https://github.com/mishra-ck/testing-microservices/blob/add-concepts/1-testing-strategies/Test%20Runner.png)

---
### There are two types of test doubles:

A test double is an Object that simulates the behaviour of the dependency.
1. Stub: A stub is a test double that returns value to the SUT. 
2. Mock: A mock is a test double that a test uses to verify that the SUT correctly invokes a depndency.

We can implement test double using Mockito, a popular mock framework for java.

---
### Different types of tests:

Automated tests are used to verfiy the functional aspect of the application, can be divided into 4 parts-

1. Unit Test: test smaller part of service, like class.
2. Integration Test: verify that a service can interact with infrastructure services such as database and others.
3. Component Test: acceptance tests for an individual service.
4. End-To-End Test: acceptance tests for entire application.

---
### Using Brian Marick's Test Quadrant to categorize tests:

The test quadrant categoirizes tests into 2 dimensions-

✅ Whether test is business facing or technolofy facing.

✅ Whether the goal of test is to support programming or critise the application.

![testing-quadrants](https://github.com/mishra-ck/testing-microservices/blob/add-concepts/1-testing-strategies/Testing-Quadrants.png)

Test quadrants defines four different types of tests :

1. Q1- Support programming/technology facing : unit and integration test
2. Q2- Support programming/business facing : component and end-to-end test
3. Q3- Critique application/business facing : usability and exploratory testing
4. Q4- Critique application/technology facing : non-functional performance test like performance tests

---
### Using Test Pyramid as a guide for testing efforts:

The idea of test pyramid is that as we move up the pyramid we should write less tests.
We should lot os unit tests and few end-to-end tests.

![test-pyramid](https://github.com/mishra-ck/testing-microservices/blob/add-concepts/1-testing-strategies/test-pyramid.png)


---
