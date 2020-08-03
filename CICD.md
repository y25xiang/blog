# CI/CD 

## Background
Currently I am doing a project which is in the testing phase. This is a blog that includes all the findings regarding CI/CD. 

## Regression Testing
Regression testing refers to testing used to ensure that a function previously worked is still working once new feature has been added. Manual regression testing is time-consuming, since the test will need to be tested for all the platforms and hardware you support.

Automated Tests is critical to ensure the software are fully tested. 

## Unit Testing 
**Definition** 
Isolated testing which only concerns with one feature. It does not care about the other systems which are related to the feature you are testing. 

**Downside**
* Don't test the contract. Assume the other components act a certain way to trigger the test. It does not test the fake input. 
* You need to create contract. If all the components are not in a separate modules, it would be difficult to test the code. 

## Integration Testing
**Definition**
We are concerning about multiple components in the system. When we are doing testing, we will test all the components together. 

**Downside**
* Expensive
  * Slower to run. You need to setup related components such as browser and database.
  * Brittle. As more components are introduced into the system, it will be more likely to get errors. 
  * Harder to write. 
* Cannot simulate errors 
  * If database is down, then your test needs to know how to handle that error. You need the ability fake errors. 
* Don't tell you where the problem is
  * If the error is in the middle of the process, the log is needed to help you find the error. 


## Unit Test for Node JS
 
### Test framework selection
Currently there are multiple test framework available for Javascript testing. One of the consideration of selecting the test framework is that it has the capability of doing both integration test and unit testing. We are trying to reduce the dependency. Based on this criteria, I find Jasmine, Mocha + Chai. 

We are trying to have as less as dependency. 

**Mocha + Chai**
Tests will have dependence. It does not clear the status. 

**Jasmine**


**Jest**
running slower than Mocha. Linear problem and Jest will reset the environment for each test. 
