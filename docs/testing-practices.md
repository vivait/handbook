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
Unit tests should be the most common type of tests in an application, these are tests which test the smallest unit of an application (such a method or a function). Unit tests run quickly this allows you to write as many of them as you need to cover all code flows and you should attempt to do this. 

We have tools to 
