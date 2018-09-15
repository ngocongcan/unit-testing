What is Unit testing?
====================

Unit testing is a software development process in which the smallest testable parts of an application, called units, are individually and independently scrutinized for proper operation. Unit testing can be done manually but is often automated.

Unit testing is a component of test-driven development (TDD), a pragmatic methodology that takes a meticulous approach to building a product by means of continual testing and revision. Test-driven development requires that developers first write failing unit tests. Then they write code and refactor the application until the test passes. TDD typically results in an explicit and predictable code base.

Unit testing involves only those characteristics that are vital to the performance of the unit under test. This encourages developers to modify the source code without immediate concerns about how such changes might affect the functioning of other units or the program as a whole. Once all of the units in a program have been found to be working in the most efficient and error-free manner possible, larger components of the program can be evaluated by means of integration testing.

Unit testing does have steep learning curve. The development team needs to learn what unit testing is, how to unit test, what to unit test and how to use automated software tools to facilitate the process on an on-going basis.  The great benefit to unit testing is that the earlier a problem is identified, the fewer compound errors occur. A compound error is one that doesn't seem to break anything at first, but eventually conflicts with something down the line and results in a problem.

This Google TechTalk provides an overview of unit testing.
<a href="http://www.youtube.com/watch?feature=player_embedded&v=wEhu57pih5w
" target="_blank"><img src="http://img.youtube.com/vi/wEhu57pih5w/0.jpg"
alt="wEhu57pih5w" width="240" height="180" border="10" /></a>


Why is Unit testing Important?
=============================
### 1. Makes the Process Agile

One of the main benefits of unit testing is that it makes the coding process more Agile. When you add more and more features to a software, you sometimes need to change old design and code. However, changing already-tested code is both risky and costly. If we have unit tests in place, then we can proceed for refactoring confidently.

Unit testing really goes hand-in-hand with agile programming of all flavors because it builds in tests that allow you to make changes more easily. In other words, unit tests facilitate safe refactoring.
### 2. Quality of Code

Unit testing improves the quality of the code. It identifies every defect that may have come up before code is sent further for integration testing. Writing tests before actual coding makes you think harder about the problem. It exposes the edge cases and makes you write better code.
### 3. Finds Software Bugs Early

Issues are found at an early stage. Since unit testing is carried out by developers who test individual code before integration, issues can be found very early and can be resolved then and there without impacting the other pieces of the code. This includes both bugs in the programmer’s implementation and flaws or missing parts of the specification for the unit.
### 4. Facilitates Changes and Simplifies Integration

Unit testing allows the programmer to refactor code or upgrade system libraries at a later date and make sure the module still works correctly. Unit tests detect changes that may break a design contract. They help with maintaining and changing the code.

Unit testing reduces defects in the newly developed features or reduces bugs when changing the existing functionality.

Unit testing verifies the accuracy of the each unit. Afterward, the units are integrated into an application by testing parts of the application via unit testing. Later testing of the application during the integration process is easier due to the verification of the individual units.
### 5. Provides Documentation

Unit testing provides documentation of the system. Developers looking to learn what functionality is provided by a unit and how to use it can look at the unit tests to gain a basic understanding of the unit’s interface (API).
### 6. Debugging Process

Unit testing helps simplify the debugging process. If a test fails, then only the latest changes made in the code need to be debugged.
### 7. Design

Writing the test first forces you to think through your design and what it must accomplish before you write the code. This not only keeps you focused; it makes you create better designs. Testing a piece of code forces you to define what that code is responsible for. If you can do this easily, that means the code’s responsibility is well-defined and therefore that it has high cohesion.
### 8. Reduce Costs

Since the bugs are found early, unit testing helps reduce the cost of bug fixes. Just imagine the cost of a bug found during the later stages of development, like during system testing or during acceptance testing. Of course, bugs detected earlier are easier to fix because bugs detected later are usually the result of many changes, and you don’t really know which one caused the bug.


When should I write unit tests?
===============================

![Product Life Cycle](/images/product-life-cycle-chart.jpeg)

*Image by Malakooti, B. (2013). Operations and Production Systems with Multiple Objectives. John Wiley & Sons. CC BY-SA 4.0*

### Stage 1: Introduction

If you’re in start up mode, doing proof of concepts, are writing tests really going to add value? Probably not. You probably haven’t even finalized core functionality at this point. So why test it?

There’s the argument that TDD makes sense and unit tests are good requirements to test against. But even here I’d say your requirements are probably changing too quickly.
### Stage 2: Growth

Okay. Enter testing. At this point the cost of code failure and potential problems begins to outweigh the cost of testing.

You should be developing a testing strategy at this point that includes other types of tests as well. This is when I think it makes sense to begin unit testing. You know what the core functionality is at this point, from here on out everything else is ramping up and adding features.
### Stage 3: Maturity

In this stage, the cost of test coverage is clearly less than the potential risk of downtime. Test the sh*t out of your software.
Stage 4: Decline

Writing new tests at this point is useless. It’s just a matter of time before the project you’re working on gets retired. Even maintaining tests is costly in this phase. You probably have a replacement piece of software in mind and a good chunk of the software has already been battle-hardened by users.

So if you have no major development planned, and a test or two fails as long as users aren’t complaining… who cares?

Ehhh you should. As the person charged with maintaining an old system, you need to care. At this point unit tests can act as kind of a canary in the coal mine. If a unit test is failing. You should at a minimum understand why it is failing. Tests don’t fail in isolation, something has changed to induce a failure. Investigate it.

References
==========
1. https://dzone.com/articles/top-8-benefits-of-unit-testing
2. https://medium.com/@JeffLombardJr/opinion-when-should-i-write-unit-tests-164b245bffbc
3. https://searchsoftwarequality.techtarget.com/definition/unit-testing
