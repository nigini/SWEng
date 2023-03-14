# Course project: Requirements & Team Policies

## Overview
Establish a solid definition of your project from which to base a design and
implementation.  You will write a document that describes the goals of your
project, its functional and non-functional requirements, and the processes your
team will follow to implement it.  This is the first iteration of a living
document, and you'll be asked to update it during the development cycle.


## Setup

Work with your newly-assigned project teams.

Create a shared living document. (We recommend a Google doc, or a Markdown or
LaTex document in a shared repository.) The majority of your technical writing
will go in to this document, and when a milestone is due you will make a
snapshot (PDF) of this document and upload to Canvas.

## Instructions

Produce the first version of your living document with the following sections.

### 1. Team info & policies (10%)
Provide a concise summary of the project team and project artifacts. Specifically:

- List each team member and their role in the project.
- Link to each project relevant artifact such as your git repo (this can be empty for now).
- List communication channels/tools with corresponding use/communication
  policies (check main course page for communication channels and policies.)

### 2. Product description (20%)
Use the product description of the project proposal as a starting point. __Revise
it__ based on feedback you received so far, and incorporate it into this section.
Additionally, add the following to this section:

- 4+ major features you will implement.
- 2+ stretch goals you hope to implement.

The major features should constitute a minimal viable product (MVP).


### 3. Use Cases (Functional Requirements) (30%)
**Each team member** must come up with and describe **at least one use case** of
your product, following this template:

1. Actors
2. Triggers
3. Preconditions
4. Postconditions (success scenario)
5. List of steps (success scenario)
6. Extensions/variations of the success scenario
7. Exceptions: failure conditions and scenarios

(At the end of this step you will have at least one use case per team member.)


### 4. Non-functional Requirements (10%)
Describe at least three non-functional requirements, e.g., related to
scalability, usability, security and privacy, etc.


### 5. External Requirements (10%)
In addition to the requirements stated above, the course staff imposes the
following requirements on your product:

- The product must be robust against errors that can reasonably be expected to
    occur, such as invalid user input.
- The product must be installable by a user, or if the product is a web-based
    service, the server must have a public URL that others can use to access it.
    If the product is a stand-alone application, you are expected to provide a
    reasonable means for others to easily download, install, and run it.
- The software (all parts, including clients and servers) should be buildable
    from source by others. If your project is a web-based server, you will need
    to provide instructions for someone else setting up a new server. Your
    system should be well documented to enable new developers to make enhancements.
- The scope of the project must match the resources (number of team members)
    assigned.

Make sure that these requirements, if applicable to your product, are specialized 
to your project and included in your document—do not copy and paste these
requirements verbatim.  You may leave this as a separate section or fold its
items into the other requirements sections.


### 6. Team process description (20%)
Describe your quarter-long development process.

- Specify and **justify** the software toolset you will use.
- Define and **justify** each team member's role: why does your team need this
  role filled, and why is a specific team member suited for this role?
- Provide a schedule for each member (or sub-group) with at least four
    concrete milestones and deadlines for the quarter.
- Specify and explain at least three major risks that could prevent you from
    completing your project.
- Describe at what point in your process external feedback
  (i.e., feedback from outside your project group, including the project manager)
  will be most useful and how you will get that feedback.


__Export a PDF snapshot of your document named PorjectName-m2.pdf 
and submit it to Canvas by due date EOD (Check Calendar).__

(Yes, 12:00am of following day is a late submission :))

## Clarifications and FAQs

### How much should we say about the software toolset we will use?

What programming languages, data sources, project trackers, and other tools will
you use? What, if any, software components will you attempt to use "off the shelf"
versus implementing them from scratch? Explain why you chose these tools and
languages, as well as why they are suitable for your project.

It is OK to establish some of the answers during the requirements engineering
stage and others during the design stage. It is also OK of some of these change
as you continue working on the project.

### What is a team member "role"?

A role describes the part of the project (or a set of tasks) a team member is
responsible for. You can refine these roles as you continue to work on your
project and you are free to change them as you go forward. It is important,
however, to justify your current decisions.

Here are two examples for defining roles:

1. A typical web application project could have roles of: 2-3 backend engineers,
   1-2 frontend engineers, and 1-2 engineers in charge of UI  design (probably
   in addition to being frontend or backend engineers).

2. A data analysis project could have roles of: 1-2 people responsible for data
   collection and storage, 1-2 people responsible for data analysis and
   visualization, and 1-2 people responsible for infrastructure and automation.

### What if we want to commercialize our project idea?

Your group will collectively own its own work. If you think you may want to
commercialize your project, you may want to consult early with a legal source. A
resource on campus is [Comotion](https://comotion.uw.edu/).

### Any advice regarding writing?

Plausibility, thoughtfulness, and level of detail will largely determine the
score for this assignment. For example, generic or incomplete use cases often
lead to deductions. You should choose and clearly describe substantial use cases
that are important to the core functionality of your product. You should also
list a reasonable set of steps in the various scenarios that can occur in these
use cases. Make sure to not omit important steps or details. Make sure that the
state of the system at the end of any path through the use case matches what the
use case claimed is the final state.

Your documents must be clear and professional. This means they should be
concisely written, with proper spelling and grammar, clear wording, and
formatted with supporting structure to present your ideas clearly to the reader.

You are developing a living document, which means you should expect change
requests and iterations.

### Is there a minimum or maximum number of pages?

No, grading focuses on completeness and proper writing (clarity and
conciseness). As with all writing, technical or otherwise, you want to
completely address each thing that needs to be addressed (in this case,
requirements) while expressing it concisely and clearly enough to be
understandable and largely free of redundancy.
