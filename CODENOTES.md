# What is scope?

Where do those variables live? In other words, where are they stored? And, most importantly, 
how does our program find them when it needs them?

### program undergoes three steps before it is executed.
1. Tokenizing/Lexing: Breaking up a string of characters.
2. Parsing: Taking a stream of tokens  and turning it into a tree of nested elements, which collectively represent 
the grammatical structure of the program. = **AST**
3. Code-Generation: the process of taking an AST and turning it into executable code.

_Any snippet of Javascript has to be compiled before it's executed._

## Understanding scope

1. Engine:responsible for start-to-finish compilation and execution of our JavaScript program.
2. Compiler: doing the work of parsing and code generation.
3. Scope: collects and maintains a list of all the declared identifiers (variables).

### var a = 2;.


Compiler:
1. see if variable a already exist for that particular scope.
2. produces code for the engine to later execute. for the a = 2 assignement.The code Engine runs will first ask Scope if there is a variable called a accessible in the current scope collection. 
If so, Engine uses that variable. If not, Engine looks elsewhere.

_ If the engine finds the variable it assigns the value 2, to it, if not an error occurs._

### Compiler speak

When Engine executes the code that Compiler produced for step (2), it has to look-up the variable a to see if it has been declared, 
and this look-up is consulting Scope. But the type of look-up Engine performs affects the outcome of the look-up.
In our case, it is said that Engine would be performing an "LHS" look-up for the variable a. 
The other type of look-up is called "RHS"
 "L" and "R" meaning: "Left-hand Side" and "Right-hand Side".Side of an assignment operation.

reference = right hand
declare = left hand = literal value 


# You Don't Know JS: Types & Grammar
### Chapter 1 : Types




