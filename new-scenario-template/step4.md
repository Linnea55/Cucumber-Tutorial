# Scenarios - Create Prime.feature

It's finally time to make our Cucumber testing file. It should be in the resources directory. Let's enter that directory:

`cd`{{execute}}

`cd cucumber-project/src/test/resources`{{execute}}

A Cucumber testing file has the extension `.feature`. We create such a file in the resources directory:

`touch Prime.feature`{{execute}}

`.feature` files are written in the `Gherkin language`; a readable way of writing tests. The Gherkin language has some
special keywords. First we must write `Feature:` followed by some text. The text should describe what feature of our code we want to test and hence we write `Prime game play`.
The next keyword is `Scenario:`, which should be followed by a text that describes the scenario we want to test. In our case, we want to provide two scenarios; one when the number
we play with is a prime and one when it's not. For the scenarios we will use the keywords `Given`, `When`, and `Then`, which is followed by a precondition, some action, and some outcome that can be tested is achieved respectively.

<pre class="file" data-filename="./cucumber-project/src/test/resources/Prime.feature" data-target="replace">
Feature: Prime game play

  Scenario: Play prime to get prime
    Given Create a Prime game play
    When I play with number 5
    Then The result is Prime

  Scenario: Play prime to get noPrime
    Given Create a Prime game play
    When I play with number 10
    Then The result is NoPrime
</pre>

The lines which start with keywords such as `Given`,`When`, and `Then` are called `steps` which are required to be defined in another file. This is done in the next step. 

