# Testing practices

At Viva IT we use tests to help drive features toward a correct implementation, and also 
to ensure that features continue to work if the code is modified.

Implementing a good realible test suite has helped us to do the following:
* Automatic dependency updates.
* Continuous depoyment.
* Onboard staff who are new to programming into a safe environment.

A well tested system consists of the right blend of multiple different types of tests.

![From Wikimedia: https://commons.wikimedia.org/wiki/File:Testing_Pyramid.svg](https://upload.wikimedia.org/wikipedia/commons/6/64/Testing_Pyramid.svg)
*Image from Wikimedia: https://commons.wikimedia.org/wiki/File:Testing_Pyramid.svg*

In the following sections we'll explore each of the tests in the above image and their usages.

## Unit tests
Unit tests should be the most common type of tests in an application, these are tests which test the smallest part (or unit) of an application (such a class method or a function). Unit tests should be designed to run quickly. Doing so allows you to cover all code execution paths and to use a variety of different datasets.

At Viva IT we use the following tools to write unit tests:
- [PHPUnit](https://phpunit.de/). Used for unit testing PHP scripts.
- [Jest](https://jestjs.io/). Used for unit testing Javascript code, we also use it for React with [Enzyme](https://enzymejs.github.io/enzyme/).

### Mocking
TBD

## Integration tests

