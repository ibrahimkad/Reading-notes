# Error Handling & Debugging

**EXECUTION CONTEXTS**

_The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope._

**GLOBAL CONTEXT:**

_Code that is in the script, but not in a function. There is only one global context in any page._


**FUNCTION CONTEXT:**

_Code that is being run within a function. Each function has its own function context._

**GLOBAL SCOPE:**

_If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope._

**FUNCTION-LEVEL SCOPE:**

_When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope._


**Each time a script enters a new execution context, there are two phases of activity:**

1. PREPARE:
_The new scope is created_
_Variables, functions, and arguments are created_
_The value of the this keyword is determined_

2. EXECUTE:
_Now it can assign values to variables_
_Reference functions and run their code_
_Execute statements_

1. Syntax Error:
_This is caused by incorrect use of the rules of the language. It is often the result of a simple typo._

2. Reference Error:

_This is caused by a variable that is not declared or is out of scope._





_The console.log() method can write data from a script to the console. If you open console- l og. html, you will see that a note is written to the console when the page loads._

_JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error._

