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
