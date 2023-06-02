# In-class exercise: Advanced Code Analysis with Z3


## High-level goal
The high-level goal of this exercise is to learn about automated theorem provers (Z3 in
particular), and how they can be used to model programs, prove program properties, and generate test cases.


## Set up
1. Team up in groups of size 2.

2. **Assign yourself to the correct (in-class-6-z3) group on Canvas.
   (You may work and submit alone, but you must still self-assign to a group on Canvas!)**

3. Download and unzip the [`in-class-z3.zip`](in-class-z3.zip) archive.

4. Open the [Z3 web interface](https://www.philipzucker.com/z3-rise4fun/)
(or [this](https://microsoft.github.io/z3guide) or [this](https://compsys-tools.ens-lyon.fr/z3)) in your browser.
(Alternatively, download the latest [Z3 release](https://github.com/Z3Prover/z3/releases).)

5. Check out the [Z3 Tutorial](https://www.philipzucker.com/z3-rise4fun/guide.html) if you
   want more background. However, you should be able to do most of this exercise
   with targeted queries as opposed to reading the entirety of it.

6. Considering we are using 8-bit integers, you will likely want to check [this page](https://microsoft.github.io/z3guide/docs/theories/Bitvectors/) with the bit-vector operations.


## Instructions
The [`in-class-z3.zip`](in-class-z3.zip)
archive contains four folders (three pairs and one set of programs).
Each pair contains the original program, a mutated program, and z3
starter code for comparing the two. The set contains the original program, a
set of four mutants, and z3 starter code.

1. **Examine the original and mutated program in the `pair1` directory.**

    Are they equivalent? (See Question 1 below)

2. **Complete `Z3startercode.pair1.smt2` (see hints below!).**

    Your completed code should either prove equivalence of the two programs or
    generates a model (test case) that proves non-equivalence.

3. **Test your code by running it with Z3.**

    Run the `.smt2` file with Z3. You can copy the entire contents of the file
    into the web interface and run it there.

4. **Repeat steps 2 and 3 for the pair2 and pair3 directories.**

    Note that we are using width-8 `BitVec`s instead of the normal
    width-32 `BitVec`. This is for ease of reading/writing/reasoning: the
    principals we care about are the same, but are a little easier to
    grok at this lower precision. Also, recall the `BitVec` operators, such
    as `bvadd` and `bvsgt`, that replace Int operators, such as `+` and `>`.

5. **Familiarize yourself with [Z3 scopes](https://www.philipzucker.com/z3-rise4fun/guide.html).**

6. **Examine the four mutants in the set1 directory.**

7. **Use scopes to complete Z3startercode.set1.smt2.**

    Your completed code should, for each mutant, either prove equivalence or
    generates a model (test case) that proves non-equivalence.
    By using scopes you can leverage the fact that much of the execution is
    identical between the original program and the mutant programs.
    (See Question 2 and 3)

8. **Test your code by running it with Z3.**

## Questions
1. Which of the mutants in pair1, pair2, and pair3 are equivalent? Provide, for
each non-equivalent mutant, a test case that detects it.
The test case should be the output of the `(get-model)` instruction in your `smt2` code.

2. Which of the four mutants in set1 are equivalent? Provide, for each
non-equivalent mutant, a test case that detects it.

3. Briefly explain how scopes work in Z3 and when they are useful?

## Deliverables
A plain-text file with your answers to the questions above. Include in that file:

+ a **list of all group members**,
+ your final versions of the four `Z3startercode.<xyz>.smt2` templates.

### Steps for turn-in
One team member should upload the deliverables to Canvas, via the Canvas Assignment.

## Hints

**When modifying the `.smt2` templates, only modify what is between the following
two lines. Do not alter anything that is not
between the following two lines, including the lines themselves!**

```
;;;;;;;;;;;;;;;;; START STUDENT CODE ;;;;;;;;;;;;;;;
```

and

```
;;;;;;;;;;;;;;;;; END STUDENT CODE ;;;;;;;;;;;;;;;
```

These anchor lines are used for grading.


