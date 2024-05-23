## Testing
Software testing is the process of finding errors in a product, whether it be a mobile or web application. Errors include bugs in the code, missing requirements, glitches, and more. Software testing can also determine whether the outcome when engaging with the application differs from the expectation.

### Test driven development
- Test-Driven Development (TDD) is a methodology in software development that focuses on an iterative development cycle where the emphasis is placed on writing test cases before the actual feature or function is written. 
- TDD utilizes repetition of short development cycles. It combines building and testing. This process not only helps ensure correctness of the code -- but also helps to indirectly evolve the design and architecture of the project at hand
- It is an iterative approach combining programming, unit test creation, and refactoring.
- Benefits
  TDD encourages writing testable, loosely-coupled code that tends to be more modular. Since well-structured, modular code is easier to write, debug, understand, maintain, and reuse, TDD helps:
 - Reduce costs
 - Make refactoring and rewriting easier and faster ("make it work" with red and green stages, then refactor "to make it right")
 - Streamline project onboarding
 - Prevent bugs and coupling
 - Improve overall team collaboration
 - Increase confidence that the code works as expected
 - Improve code patterns
 - Eliminate fear of change

### Manual testing
- Manual testing is done in person, by clicking through the application or interacting with the software and APIs with the appropriate tooling. This is very expensive since it requires someone to setup an environment and execute the tests themselves, and it can be prone to human error as the tester might make typos or omit steps in the test script.
- Human testers execute tests on a software application to identify errors. The tester follows a predetermined set of test cases to ensure the application performs as expected. This is a labor-intensive process and can be slow.

## Automated Testing

- Automated tests, on the other hand, are performed by a machine that executes a test script that was written in advance. These tests can vary in complexity, from checking a single method in a class to making sure that performing a sequence of complex actions in the UI leads to the same results. It's much more robust and reliable than manual tests – but the quality of your automated tests depends on how well your test scripts have been written. 


## The Core Principles of Software Testing
- Testing is context-dependent: Different applications have different requirements and constraints, so your test should be tailored to the context.
- Absence of errors fallacy: The absence of errors does not guarantee the absence of defects in a software application. Software testing should be designed to cover identified and potential bugs.
- Early testing: This helps detect errors early, reducing the cost and effort required to fix them later.
- Pesticide paradox: Repeating the same tests multiple times can result in finding the same errors while missing new issues. Tests should be revised regularly to include new cases.
- Defect clustering: A small number of modules in a software application are often responsible for the majority of defects, so testing should focus on identifying and testing these thoroughly.
- Exhaustive tests are impossible: Due to the often limitless number of test scenarios, testing every combination of inputs and conditions is impossible.



## Different Types of Tests
 
### Unit tests
Unit tests are very low level and close to the source of an application. They consist in testing individual methods and functions of the classes, components, or modules used by your software. Unit tests are generally quite cheap to automate and can run very quickly by a continuous integration server.

### Integration tests
Integration tests verify that different modules or services used by your application work well together. For example, it can be testing the interaction with the database or making sure that microservices work together as expected. These types of tests are more expensive to run as they require multiple parts of the application to be up and running.


### End-to-end tests
End-to-end testing replicates a user behavior with the software in a complete application environment. It verifies that various user flows work as expected and can be as simple as loading a web page or logging in or much more complex scenarios verifying email notifications, online payments, etc...

End-to-end tests are very useful, but they're expensive to perform and can be hard to maintain when they're automated. It is recommended to have a few key end-to-end tests and rely more on lower level types of testing (unit and integration tests) to be able to quickly identify breaking changes.

### Functional tests
Functional tests focus on the business requirements of an application. They only verify the output of an action and do not check the intermediate states of the system when performing that action.

There is sometimes a confusion between integration tests and functional tests as they both require multiple components to interact with each other. The difference is that an integration test may simply verify that you can query the database while a functional test would expect to get a specific value from the database as defined by the product requirements.

### Acceptance testing
Acceptance tests are formal tests that verify if a system satisfies business requirements. They require the entire application to be running while testing and focus on replicating user behaviors. But they can also go further and measure the performance of the system and reject changes if certain goals are not met.

### Performance testing
Performance tests evaluate how a system performs under a particular workload. These tests help to measure the reliability, speed, scalability, and responsiveness of an application. For instance, a performance test can observe response times when executing a high number of requests, or determine how a system behaves with a significant amount of data. It can determine if an application meets performance requirements, locate bottlenecks, measure stability during peak traffic, and more. 

### Smoke testing
Smoke tests are basic tests that check the basic functionality of an application. They are meant to be quick to execute, and their goal is to give you the assurance that the major features of your system are working as expected.

Smoke tests can be useful right after a new build is made to decide whether or not you can run more expensive tests, or right after a deployment to make sure that they application is running properly in the newly deployed environment.


## Software Testing tools
- Selenium
- Ranorex
- Testpad
- Jest
- Cypress (end to end E2E test)
- Supertest

## Useful Repos
- http://github.com/EbookFoundation/free-programming-books
- http://github.com/sbilly/awesome-security
- http://github.com/Chalarangelo/30-seconds-of-code
- http://github.com/AllThingsSmitty/css-protips
- http://github.com/ryanmcdermott/clean-code-javascript
- http://github.com/vasanthk/how-web-works
- http://github.com/jwasham/coding-interview-university

[References]
- https://www.geeksforgeeks.org/types-software-testing/
- https://www.perfecto.io/resources/types-of-testing