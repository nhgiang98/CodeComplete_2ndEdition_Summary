# CODE COMPLETE 2ND CONDITION
Source: [Code Complete 2nd Edition](http://aroma.vn/web/wp-content/uploads/2016/11/code-complete-2nd-edition-v413hav.pdf)

## Content and purpose 
* Containing the research and programming experience
* Create higher quality software
* Support to do your work more quickly
* How to avoid problems in the future
* Improve coding skill to increase performence

### Chapter 1: Welcome to Software Construction 
* The main activites in construction are:
	* Detailed design
	* Coding and Debugging
	* Integration
	* Developer testing (unit testing and integration testing) 
*The quality of the construction substantially affects the quality of the software. 

### Chapter 4: Key Construction Decisions 
* Every programming language has strengths and weaknesses. So should be choose and use a language that you've used before. It helps you will become more experienced and more productive.
* Choose the practices that are best suited to your project.
* Establish programming conventions before you begin programming.

### Chapter 10: General Issues in Using Variables
* Pay attention to declare variables: Use naming conventions, check variable name, turn off implicit declarations, set default value for variables.
* Minimize scope of each variables.
* Keep references to a variables close together. Keep it local to a routine or class. Avoid global data.
* Use each variable for one purpose.

### Chapter 11: The Power of Variable Names 
* Variable name should be readability.
* Variable name must be meaningful.
* Each variable name for one purpose, avoid using variables for specific purposes.
* Use variable naming conventions depends on the size of project types.
* Variables have naming corresponding with purposes. Ex: loop index, naming status, naming
* A good name tends to express the "what" more than "how".
* A variable name can contain the variable contents, the kind of data and the scope or visibility of the variable.
* Avoid using name with similar meanings such as "lineNumber" and "lineIndex".
* Avoid using name with different meanings but similar names.

### Chapter 12: Fundamental Data Types 
* Creating your own types makes your programs easier to modify and more self documenting
* Avoid initialize string to null, endless strings in C.

### Chapter 13: Unusual Data Types
* Unusual data types such as structure, pointer, global data …
* Avoid using global variables, can replace them with something better such as work with them through access routines.

### Chapter 15: Using Conditionals
#### a. `If` statements: 
* `If-then` statements:
	* Depending on the language we’re using. The simplest is the plain if or if then.
	* Write the nominal path through the code first; then write the unusual cases.
	* Make sure that you branch correctly on equality: Use `>` instead of  `>=` or `<` instead of `<=`.
	* Put the normal case after the if  rather than after the else.
	* Test the else clause for correctness

* `If-then-else` statements:
	* Simplify complicated conditionals expressions with calls to methods that return boolean values.
	* Put the most common cases first.
	* Make sure all cases are covered.

#### b. `Case` statements
* Some cases statements only work on data of certain types; do not create a "phony variable" to use a case statement.
* Use the default statement to detect legitimate defaults, or to detect errors and nothing else.

### Chapter 16: Controlling Loops 
#### a.Selecting the kind of loop
* Use `while` loop when you are not sure exactly how many times the loop to iterate.
* Keep `for` loop simple, consider `while` loop if you are explicitly changing the index value.

#### b.Controlling the Loops
* Put initialization code directly before the loop
* Use `while (true)` or `for (; ;)` to write an infinite loop.
* Do not change the index of a `for` loop to make it terminate. 
* Avoid using the loop index value after the loop; instead assign a final value to a variable at the appropriate point inside the loop.

### Chapter 17: Unusual Control Structures
#### a.Recursion
* Make sure the recursion stops: Handle the case when recursion stops.
* Consider to use recursion because it is very complicated.
* Use "new" key work to create objects on the heap for local variables 	in recursive functions.

#### b.`goto`
* Use `goto` to jump to a previously defined label.
* The `goto` statement is not recommended because it is very difficult to follow the work flow and makes the program difficult to understand and maintain.
* The try*finally construction can sometimes be used to perform the error cleanup that a goto sometimes performs. 
* A `goto` statement can always be written by another formal statement.

### Chapter 19: General Control Issue
#### a.Boolean Expressions
* Making boolean expression simple and readable.
* Comparing a character against `\0` instead of `0`.

#### b.Compound Statements (Blocks)
* Write pairs of braces together: Fill in the middle after you write both the opening and closing parts of a block.
* Use braces to clarify conditionals.

#### c.Null Statements
* Null statements are uncommon, so make them obvious, add comments to explain why one is used.  

#### d.Taming Dangerously Deep Nesting
* Simplify a nested if by retesting part of the condition.
* Simplify a nested if by using a break block, move some of the nested blocks into their own methods or use polymorphism.
* Convert a nested if to a set of if*then*else.
* Rewrite the code use a status variable.
* Use exceptions.

#### e.A Programming Foundation: Structure Programming 
* Structure programming is a simple idea that is still relevant: you can build any program out of a combination of sequences, selections and iterations.

### Chapter 20: The Software Quality Landscape
* Characteristics of Software Quality: Correctness, Usability, Efficiency, Reliability, Integrity, Adaptability, Accuracy,Robustness,
* Internal quality characteristics: Maintainability, Flexibility, Portability, Reusability, Readability, Testability, Understandability

### Chapter 21: Collaborative Construction
* Benefits of pair programming:
	* Improve code quality
	* It shortens schedule: Helping write code faster and fewer errors.
	* Connect people with a team.

* Key to improve with pair programming:
	* Support pair programming with coding standards.
	* Do not let pair programming turn into watching.
	* Do not force pair programming of the easy stuff.
	* Avoid pairing all newbies.
	* Rotate pairs and work assignments regularly.
	* Encourage pairs to match each other’s pace.
	* Do not force people who don’t like each other to pair.	

### Chapter 22: Developer Testing
* Tested after have finished the implementation function/class/method
* Defined test cases with work flow analysis
* Automated testing 

### Chapter 23: Debugging 
* Debugging is not way to improve quality. It is a way to diagnose defects. Debugging is a last way.
* Debugging is a method when we encountered errors. Understand the root cause before you fix the program.
* Should use debugging tools to software development.
* If your code has a bug, it’s your fault, do not relate to computer or compiler.
* After make a fix, check it again.

### Chapter 24: Refactoring  
* Reason to Refactor:
	* Code is duplicated, long, nested and poor cohesion, abstraction, encapsulation.
* Specific Refactoring: 
	* Never write document code or design ahead. 
* Data level refactoring: Rename a variable with a clearer or more informative name, Replace a magic number with a named constant, use a local variable for local purposes rather than a parameter
* Statement*Level refactoring: Use break or return instead of a loop control variable, decompose a boolean expression, create and use null objects instead of testing for null values
* Routine*Level refactoring: remove a parameter if a routine no longer uses a parameter, add a parameter when needed.
* Class implementing refactoring: include pulling up or pushing down data or methods; separating or combining classes with subclasses.
* Class interface refactoring: move a routine to another class; hide a delegate, replace inheritance with delegation,… 
* System level refactoring: create a definitive reference source for data you can not control; replace error code with exceptions or vice versa.
* Refactoring safely: 
	* Keep refactoring small; do refactoring on at a time; make frequently checkpoints.
	* Add test cases; use your compiler warning; review the changes. 
* Refactoring strategies:
	* Refactor when you add a routine, add a class, fix a defect,…
