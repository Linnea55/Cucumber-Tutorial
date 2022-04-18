# Background: Why Use Tests, and Why Have Them Automated?

In DevOps, testing is crucial- we must be sure that the program we have created does what we intended it to do. It's also beneficial to perform testing automatically rather than doing it manually, since it's more efficient. Test automation enables software developers and companies to save time, money, effort, and helps to have applications with better quality.

# Background: What Is Cucumber and Why Should It Be Used?

There are many different ways to perform tests automatically. However, sometimes it's convenient if the tests can be understood by a non-programmer, for instance your client or the CEO of your company, or by a person that understands a different programming language. Cucumber helps us do this by creating behavior around tests. The behavior makes it easy to understand a specific feature of the code, even if it's read by a non-technical person. Cucumber is an open source testing tool which supports `Behavior-driven development` (BDD) approach. In BDD, expected behaviors (examples) in the application are described in some ubiquitous language, and those examples are used for the automated tests. In Cucumber, those examples which illustrate software's behavior are called `Scenarios`, and we're going to describe it in `.feature` file. In order for Cucumber to execute a scenario we also need to create `Step definitions` which define steps in a scenario. We'll come back to it later. To summarize: Cucumber's BDD approach works well for better collaboration between different teams in development, and customers. This is largely thanks to the behavior scenarios which can be written and understood by anyone with plain language.

# Setup a Gradle Project

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


