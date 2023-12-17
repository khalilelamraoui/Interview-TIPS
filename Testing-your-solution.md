## Introduction
In this reading, you will learn about how you can build testing into your take-home assignments and a coding interview, you’ll also explore the practice of writing unit tests.

Testing is a key part of software development. Ideally, the scope of your tests is comprehensive; however, there are always external considerations that can affect this ideal outcome.

## Take-home assignement
If you have been allowed to take some code home, you may have time to implement more comprehensive tests. 
*There are many types of tests that you can choose to run. For example:*
- Integration tests: These test how various components of an application interact with one another. An integration test will not be in-depth because the external dependencies will be simulated rather than using actual instances. Further, unit tests assess individual lines of code, while integration tests take more of a global approach. 

- Functional tests: This is an automated test that proves that a system operates as expected. This test is concerned with the capabilities of the system. 

- Regression tests: This is to test that a change does not cause an error in the existing code. It ensures that when a system change is made, it does not affect its operations.

## Coding interview
Unit testing is an approach that confirms your code is working as expected. While many tests are written before code goes into production, you will not have an opportunity to write all these when engaging in a coding interview.
***Considerations when writing tests:***
- Readability: Make the tests readable for other developers. This habit should be internalized regardless of whether you work in a team. Tests with a clear purpose identify problems should they arise. They also signpost what a section of code is supposed to achieve. This has the added effect of increasing maintainability. 

- Clear outcomes: Your tests should, whenever possible, be deterministic. This is to say that the result should always be the same regardless of the conditions. A deterministic test will always fail when buggy code is written. Tests dependent on a combination of different conditions can be challenging to debug. 

- Automation: Tests should always have the potential to be automated so that they can be run quickly whenever a change has been made to code. This is a cornerstone of CI/CD (Continuous Integration/ Continuous Development).

***Putting unit tests into practice:***
- *The defining solutions reading outlines the steps needed to make a number-guessing game. Below is a screenshot of the pseudocode used to develop a viable solution.*
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/rItkZaeATwW-ReWm9GruLQ_458d2d352ee74d6c8194a05e98010fe1_Testing-your-solution-image-1-1-.png?expiry=1702944000000&hmac=IS4XHn_LMnEZIXNyOkr9xCi6XtaZVIp9N45JEOsgOHw"/>

- *Taking this example, imagine that there are only a few minutes left in the allotted time, what would you focus on?*
<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/VVz3akZpRpObPW0e8tPr5A_6c3dcfd48fe94e898699fad4ad572ee1_Testing-your-solution-image-2-2-.png?expiry=1702944000000&hmac=llpkmGvf9twmM5MXSGehbUTjGfoUjTXz9VDp9l4WsLU"/>

## Conclusion
In this reading, you learned to integrate testing into take-home assignments and coding interviews, emphasizing the importance of code assessment. Recognize that writing unit tests, often overlooked in favor of implementation time, is a crucial practice. Incorporating unit tests into your coding routine not only adds credibility but also positions you as a strong candidate, especially in time-sensitive scenarios like coding interviews.
