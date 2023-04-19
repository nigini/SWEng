# Course project: Architecture and Design

## Overview

Solidify the software architecture and design of your product.

## Setup

Work with your project group to revise and extend your living document.

## Instructions

Add three new sections to your living document (Software architecture, Software
design, and Coding guidelines) and revise the process description section.
Additionally, _incorporate the feedback that you have already received_.

### 1. Software architecture (40%)

Provide an overview of your system. Specifically:

- Identify and describe the major software **components** and their
    functionality at a conceptual level.

- Specify the **interfaces** between components.

- Describe in detail what **data** your system stores, and how. If it uses a
    database, give the high level database schema. If not, describe how you are
    storing the data and its organization.

- If there are particular **assumptions** underpinning your chosen architecture,
    identify and describe them.

- **For each of two decisions pertaining to your software architecture**, identify and briefly describe an **alternative**.
    For each of the two alternatives, discuss its pros and cons compared to your choice.


### 2. Software design (30%)

Provide a detailed definition of each of the software components you identified
above.

- What **packages, classes, or other units of abstraction** form these
    components?

- What are the **responsibilities** of each of those parts of a component?

### 3. Coding guideline (10%)

For each programming language that you will use in the implementation of
your project, provide a link to a pre-existing coding style guideline
that the members of your project will follow. Do not try to make up your
own guidelines. Briefly state why you chose those guidelines and how you plan
to enforce them.


### 4. Process description (20%)

Expand your process description to address the following five topics:

#### i. Risk assessment

Identify the top five risks to successful completion of your project.

For each, give:

* Likelihood of occurring (high, medium, low);

* Impact if it occurs (high, medium, low);

* Evidence upon which you base your estimates, such as what information you have
  already gathered or what experiments you have done;

* Steps you are taking to reduce the likelihood or impact, and steps to permit
  better estimates;

* Plan for detecting the problem (trivial example: running automated tests to
  determine that a file format has changed);

* Mitigation plan should it occur.

Explicitly state how this has changed since you submitted your Requirements
document.

#### ii. Project schedule

Identify milestones (external and internal), define tasks along with effort
estimates (at granularity no coarser than 1-person-week units), and identify
dependences among them. (What has to be complete before you can begin
implementing component X? What has to be complete before you can start testing
component X? What has to be complete before you can run an entire (small) use
case?) This should reflect your actual plan of work, possibly including items
your team has already completed.

To build a schedule, start with your major milestones (tend to be noun-like) and
fill in the tasks (tend to start with a verb) that will allow you to achieve
them. A simple table is sufficient for this size of a project.


#### iii. Team structure

Make sure to update your team structure, if necessary, and provide more details
about team organization and team members' roles and responsibilities.


#### vi. Documentation plan

Outline a plan for developing documentation that you plan to deliver with the
system, e.g., user guides, admin guides, developer guides, man pages, help
menus, wikis, etc.


### 5. Submit 

Finally, export a PDF snapshot of your living document named **ProjectName-m4.pdf** 
and submit it to Canvas be deadline (*check calendar*).



## Clarifications

### What principles should our software architecture and design follow?

* Strive for modularity and testability.

* Use encapsulation.

* Keep related data and behavior in the same place.

* Emphasize cohesion, limit coupling, and do not pollute public interfaces.

* Emphasize separation of concerns: avoid "god classes" that do too much.

* Avoid overengineering and complexity: avoid insignificant or irrelevant
  classes that do too little.

* Make sure you can describe the purpose and functionality of each class
  concisely and clearly.

* Keep the data model decoupled from the UI (view).

* Allow for features to be developed in parallel as much as possible.



### Any other writing hints?

In evaluating your work, we will check whether your living document

(1) addresses all the necessary elements of defining the architecture and design of your system,

(2) provides reasonable justifications for decisions made,

(3) provides a reasonable schedule and set of tasks, and

(4) shows general improvements, in particular to the process section.


**Be brief.** Your living document should addressed the required points briefly and
clearly. The staff will deduct points for overly long, poorly organized, or
poorly explained documents.

Do not include **content-free filler** in your living document. This
includes anything that could appear in identical form in another group's
materials. For example, don't merely state as a risk, "we might fall behind
schedule" (another example is "we don’t know the tools"). What factors do you
think are most likely to cause schedule slippage for your project? Why do you
think those are the parts of the schedule with the greatest potential variance?
What have you done, or what do you plan to do, to learn more about how long
those particular tasks will really take?

Your living document should clearly describe (and possibly visualize) the system
architecture. For example, if you are using the Model-View-Controller
architecture, your living document should make this clear and provide references to the
design section, which in turn clearly describes which classes implement the
model, the view, and the controller of your system.

Avoid duplicated information and make good use of cross-references.
