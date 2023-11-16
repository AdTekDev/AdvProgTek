
# CHECKLIST: 

## Using Conditionals  

**if-then Statements**    
❑ Is the nominal path through the code clear?  
❑ Do if-then tests branch correctly on equality?  
❑ Is the else clause present and documented?  
❑ Is the else clause correct?  
❑ Are the if and else clauses used correctly—not reversed?  
❑ Does the normal case follow the if rather than the else?  

**if-then-else-if Chains**  
❑ Are complicated tests encapsulated in boolean function calls?  
❑ Are the most common cases tested first?  
❑ Are all cases covered?  
❑ Is the if-then-else-if chain the best implementation—better than a case statement?  

**case Statements**    
❑ Are cases ordered meaningfully?  
❑ Are the actions for each case simple—calling other routines if necessary?  
❑ Does the case statement test a real variable, not a phony one that’s made up solely to use and abuse the case statement?  
❑ Is the use of the default clause legitimate?  
❑ Is the default clause used to detect and report unexpected cases?  
❑ In C, C++, or Java, does the end of each case have a break?  


## Loops  

**Loop Selection and Creation**  
❑ Is a while loop used instead of a for loop, if appropriate?  
❑ Was the loop created from the inside out?  

**Entering the Loop**  
❑ Is the loop entered from the top?  
❑ Is initialization code directly before the loop?  
❑ If the loop is an infinite loop or an event loop, is it constructed cleanly rather than using a kludge such as for i = 1 to 9999?  
❑ If the loop is a C++, C, or Java for loop, is the loop header reserved for loopcontrol code?  

**Inside the Loop**  
❑ Does the loop use { and } or their equivalent to enclose the loop body and prevent problems arising from improper modifications?  
❑ Does the loop body have something in it? Is it nonempty?  
❑ Are housekeeping chores grouped, at either the beginning or the end of the loop?  
❑ Does the loop perform one and only one function, as a well-defined routine does?  
❑ Is the loop short enough to view all at once?  
❑ Is the loop nested to three levels or less?  
❑ Have long loop contents been moved into their own routine?  
❑ If the loop is long, is it especially clear?  

**Loop Indexes**  
❑ If the loop is a for loop, does the code inside it avoid monkeying with the loop index?  
❑ Is a variable used to save important loop-index values rather than using the loop index outside the loop?    
❑ Is the loop index an ordinal type or an enumerated type—not floatingpoint?  
❑ Does the loop index have a meaningful name?  
❑ Does the loop avoid index cross-talk?  

**Exiting the Loop**  
❑ Does the loop end under all possible conditions?  
❑ Does the loop use safety counters—if you’ve instituted a safety-counter standard?  
❑ Is the loop’s termination condition obvious?  
❑ If break or continue are used, are they correct?  

## Unusual Control Structures

**return**  
❑ Does each routine use return only when necessary?  
❑ Do returns enhance readability?  

**Recursion**  
❑ Does the recursive routine include code to stop the recursion?  
❑ Does the routine use a safety counter to guarantee that the routine stops?  
❑ Is recursion limited to one routine?  
❑ Is the routine’s depth of recursion within the limits imposed by the size of the program’s stack?  
❑ Is recursion the best way to implement the routine? Is it better than simple iteration?  

**goto**  
❑ Are gotos used only as a last resort, and then only to make code more readable and maintainable?  
❑ If a goto is used for the sake of efficiency, has the gain in efficiency been measured and documented?  
❑ Are gotos limited to one label per routine?  
❑ Do all gotos go forward, not backward?  
❑ Are all goto labels used?  

## Table-Driven Methods  
❑ Have you considered table-driven methods as an alternative to complicated logic?  
❑ Have you considered table-driven methods as an alternative to complicated inheritance structures?  
❑ Have you considered storing the table’s data externally and reading it at run time so that the data can be modified without changing code?  
❑ If the table cannot be accessed directly via a straightforward array index (as in the age example), have you put the access-key calculation into a routine rather than duplicating the index calculation in the code?  


