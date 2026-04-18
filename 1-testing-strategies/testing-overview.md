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
