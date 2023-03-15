# Course project: Testing and Continuous Integration

## Overview

Flesh out the testing plan you laid out in your living document and
set up automated testing and continuous integration (CI) for your project.

## Set up

Work with your project group to (1) revise and extend your living document
and (2) set up continuous integration for your GitHub repository.

## Instructions

### 1. Add test-automation and CI to your test plan (50%)

Extend your test plan (which is a subsection of *Process description*) and
describe:

* Your test-automation infrastructure (e.g., JUnit, Mocha, Pytest, etc).

* A brief justification for why you chose that test-automation infrastructure.

* How to add a new test to the code base.

* Your CI service and how your project repository is linked to it.

* A brief justification for why you chose that CI service.

* A pros/cons matrix for at least three CI services that you considered.

* Which tests will be executed in a CI build.

* Which development actions trigger a CI build.


### 2. Set up your test-automation infrastructure and chosen CI service (50%)

You are not expected to provide an extensive test suite for your project at this
point. Rather, the goal is to have the test infrastructure and CI set up with a
few existing, example tests. (Your set up and the documented test-addition
process should allow a developer on the team to easily add and run a new test.)


### 3. Submit

Submit a PDF snapshot of your living document named **ProjectName-m5.pdf** to Canvas by due date (*Check Calendar!*).


## Clarifications

*What are some commonly used CI services?*

Here are four examples for commonly used CI services:

* [Travis](https://travis-ci.org)

* [CircleCI](https://circleci.com/)

* [GitHub Actions](https://docs.github.com/en/actions)

* [MS Azure pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/create-first-pipeline)

There are other options, so make sure to do sufficient research to make an
informed decision for your project.

*What do you mean by "the link between the CI service and our repo"?*

You should describe how the CI service is integrated into your repository and
how it is configured (e.g., how does the CI service access your repository and
how are the triggers that you identified configured?). Your description should
enable others to reproduce the steps that were required to set up CI for your
project and to configure the CI service.

*Any grading hints for this type of assignment?*

Part of your grade will come from the **plausibility and thoughtfulness of your
test plan**.

Further, you will be **graded on your actual CI setup** and your justifications
for choosing that CI service.

You are expected to **do some research to make an informed decision** when
picking a CI service and to **read documentation** to set up your testing and CI
infrastructure.
