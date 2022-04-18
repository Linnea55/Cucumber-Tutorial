# Background: Why use tests, and why have them automatated?

In DevOps, testing is crucial- we must be sure that what we have created does what we intended it to do. It's also beneficial to perform testing automatically rather than do it manually, since it's more efficient. Test automation enables software developers and comapanies to save time, money, effort, and helps deployment of applications with better quality.

# Background: What is Cucumber and why should it be used?

There are many different ways to perform tests automatically. However, sometimes it's convinient if the tests can be understood by a non-programmer, for instance your client or the CEO of your company. Cucumber helps us do this by creating behaviour around tests. The behaviour makes it easy to understand a specific feature of the code. Cucumber is an open source testing tool which supports `Behavior-driven development` (BDD) approach. In BDD, expected behaviours (examples) in the application is described in some ubiquitous language, and those examples are used for the automated tests. In Cucumber, those examples which illustrates software's behavior are called `Scenarios`, and we're going to describe it in `.feature` file. In order for Cucumber to execute a scenario we also need to create `Step definitions` which defines steps in a scenario. We'll come back to it later. 

# Setup a Gradle project

Let's start with making a folder where we can create our code with cucumber testing:

`mkdir cucumber-project`{{execute}}

And enter the new folder:

`cd cucumber-project`{{execute}}

In order to use Cucumber testing, you have to use a build tool, either Gradle or Maven. This tutorial uses Gradle. Let's start setting up a Gradle. We do this by running the following command:

`gradle init`{{execute}}

You have to choose some alternatives:

Let's create a application project `2`{{execute}} with implementation language java `3`{{execute}}, build script DSL Groovy `1`{{execute}} and test framework JUnit4 `1`{{execute}}. 

And set the project name `cucumber-project`{{execute}} and source package name `cucumber.project`{{execute}}.

Great! Gradle is now configured in the folder. You can verify this by doing `ls`{{execute}}, and you will see new gradle files in the directory. 


