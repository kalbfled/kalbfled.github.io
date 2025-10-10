# Thoughts on Software Development

## Introduction

I used to think that software development is a creative endeavor.  After more than 10 years of writing code almost everyday--for work, for personal projects, and in multiple languages and paradigms--I have concluded that getting the desired outcome is less about creativity and more about following a reliable, coachable process to structure code is a way that is **easy to test, easy to understand, easy to maintain, easy to change, and hard to break**.

This is a living document to promulgate my prescriptions for such a process.  If I'm reviewing your pull request, I'm looking for things described herein.

## The Big Picture

Properly commented code that is easy to test probably meets the other criteria.  **The easiest unit of code to test is a function that takes inputs, returns outputs, and has zero side-effects other than logging.**  Raising an exception might also be acceptable.

Object-oriented programming (OOP) is antithetical to this maxim.  If there's no obvious concept of a world or global state in your application, and if a function called with the same inputs should always yield the same outputs, reconsider using OOP.

## Learn Haskell

When junior developers and interns ask me what they should do to become better coders, I response, "Learn Haskell."  Haskell is a popular pure functional programming language, and pure functional programming languages force developers to write code the way I think it should be written most of the time anyways.  **Learning Haskell will change how you write other languages by conditioning you to avoid side-effects and to focus on data types.**

[Learn You a Haskell for Great Good](http://learnyouahaskell.com/chapters) is an excellent resource.
