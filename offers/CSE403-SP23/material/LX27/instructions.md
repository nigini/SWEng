# In-class exercise fault localization: Instructions

## High-level goal
The high-level goal of this exercise is to learn about systematic debugging and
software testing best practices that support effective debugging.

## Set up
1. Team up in groups of size 2.

2. **Assign yourself to the correct (in-class-5-fault-localization) group on Canvas.
   (You may work and submit alone, but you must still self-assign to a group on Canvas!)**

3. Make sure that you have
   [Apache Ant](http://ant.apache.org/),
   a [Java 17](https://www.oracle.com/java/technologies/downloads) JDK, and
   [git](https://git-scm.com/) installed.
The required software is already installed on attu.cs.washington.edu, if you
prefer to do the exercise there.

4. Clone the following git repository and read its `README.md` file:
[https://bitbucket.org/rjust/debugging](https://bitbucket.org/rjust/debugging)

5. Test your set up by running `ant clean test` in each of the bug directories
(i.e., in bug1, bug2, bug3). You should observe a test failure for each bug, but
you should be able to compile the code and run the tests.


## Instructions
1. **Bug1:** Run `ant clean test` in the `bug1` directory.

2. **Bug1:** For each of the following steps, note whether you can **directly**
     infer the buggy class(es), the buggy method(s), and the buggy statement(s) 
     (See Question 1 below):

    a. Inspect the test output only.

    b. Inspect the failing assertion.
    
    c. Inspect the method that is called from the failing assertion.

3. **Bug1:** Minimize the failing test: cut and paste the failing
   assertion(s) into a separate test method named `testFailing`; only remove
   the failing assertion(s) from the existing test method, but keep all passing
   assertions.

4. **Bug1:** Compare the visualizations of the Tarantula fault localization
   technique, [before](fl_output/bug1.non-min.html) and
   [after](fl_output/bug1.min.html) minimizing the failing test.

    **Note that you do not need to invoke Tarantula or any other tool for this step**;
    the visualizations are pre-computed for you! Also note that the outer ring in
    these visualizations represents the set of methods invoked by any of the tests;
    you can **mouse-over** on any element to see its corresponding method name and
    suspiciousness -- generally, green means not suspicious and red means very
    suspicious; you can **double-click** on any element to zoom in, e.g., to see
    suspiciousness at the line level. (See Question 1 below)

5. **Bug1:** Localize and fix the bug. If you get stuck, ask a staff member
   for help. (See Question 3 below)

6. **Bug1**: Use [this link](fl_output)
   to view the ranking files for each bug, and locate the buggy line in
   `bug<X>.ranking.txt`, where `<X>` is the bug number (i.e., `1` for Bug1).
   (See Question 4 below)

7. **Bug2:** Repeat steps 2, 5, and 6. (See Question 4 below)

8. **Bug3:** Repeat steps 2, 5, and 6. (See Question 4 below)


## Questions

1. **Bug1**: Were you able to directly infer (1) the buggy class(es), (2) the buggy method(s), 
and (3) the buggy statement(s) in the steps described above? For each, briefly
explain why or why not. 

2. **Bug1**: How did the output (visualization) of the Tarantula fault localization 
technique change after minimizing the failing test? Briefly explain why.

3. *Bug1*: What information helped you to ultimately localize and fix the bug?

4. **For each bug**, where does the buggy line appear in the
[`bug<X>.ranking.txt`](fl_output), where `<X>` is the bug number (i.e., `1` for Bug1)?
For each bug, briefly explain your observation.

5. **Compare all bugs**: Which was the easiest to localize, and which was the hardest
to localize? Briefly explain your reasoning.

6. Consider your observations and their implications: Provide two suggestions for
testing best practices that support effective debugging.

## Deliverables
A **plain-text file** including the following information:

+ a **list of all group members**,
+ your answers to the 6 questions above,
+ the minimized failing test method (i.e., `testFailing`) for bug1,
+ three patches (in [unified diff](https://en.wikipedia.org/wiki/Diff#Unified_format) format) for bug1, bug2, and bug3.


### Steps for turn-in

One team member should upload the deliverables to Canvas, via the [Canvas submission site](https://canvas.uw.edu/courses/1612319/assignments/8060491) for this course.
