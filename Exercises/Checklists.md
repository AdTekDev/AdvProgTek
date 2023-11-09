
# CHECKLIST

## Naming Variables  

General Naming Considerations  
❑ Does the name fully and accurately describe what the variable represents?    
❑ Does the name refer to the real-world problem rather than to the programming-language solution?  
❑ Is the name long enough that you don’t have to puzzle it out?  
❑ Are computed-value qualifiers, if any, at the end of the name?  
❑ Does the name use Count or Index instead of Num?  


Naming Specific Kinds of Data  
❑ Are loop index names meaningful (something other than i, j, or k if the loop is more than one or two lines long or is nested)?  
❑ Have all “temporary” variables been renamed to something more meaningful?  
❑ Are boolean variables named so that their meanings when they’re true are clear?  
❑ Do enumerated-type names include a prefix or suffix that indicates the category—for example, Color_ for Color_Red, Color_Green, Color_Blue, and so on?  
❑ Are named constants named for the abstract entities they represent rather than the numbers they refer to?  


Naming Conventions  
❑ Does the convention distinguish among local, class, and global data?  
❑ Does the convention distinguish among type names, named constants, enumerated types, and variables?  
❑ Does the convention identify input-only parameters to routines in languages that don’t enforce them?   
❑ Is the convention as compatible as possible with standard conventions for the language?   
❑ Are names formatted for readability?


Short Names  
❑ Does the code use long names (unless it’s necessary to use short ones)?  
❑ Does the code avoid abbreviations that save only one character?  
❑ Are all words abbreviated consistently?  
❑ Are the names pronounceable?  
❑ Are names that could be misread or mispronounced avoided?  
❑ Are short names documented in translation tables?  


Common Naming Problems: Have You Avoided...  
❑ ...names that are misleading?  
❑ ...names with similar meanings?  
❑ ...names that are different by only one or two characters?  
❑ ...names that sound similar?  
❑ ...names that use numerals?  
❑ ...names intentionally misspelled to make them shorter?  
❑ ...names that are commonly misspelled in English?  
❑ ...names that conflict with standard library routine names or with predefined variable names?  
❑ ...totally arbitrary names?  
❑ ...hard-to-read characters?  


## Fundamental Data


Numbers in General  
❑ Does the code avoid magic numbers?     
❑ Does the code anticipate divide-by-zero errors?     
❑ Are type conversions obvious?     
❑ If variables with two different types are used in the same expression, will the expression be evaluated as you intend it to be?     
❑ Does the code avoid mixed-type comparisons?   
❑ Does the program compile with no warnings?   


Integers   
❑ Do expressions that use integer division work the way they’re meant to?   
❑ Do integer expressions avoid integer-overflow problems?   


Floating-Point Numbers  
❑ Does the code avoid additions and subtractions on numbers with greatly different magnitudes?   
❑ Does the code systematically prevent rounding errors?   
❑ Does the code avoid comparing floating-point numbers for equality?   


Characters and Strings  
❑ Does the code avoid magic characters and strings?   
❑ Are references to strings free of off-by-one errors?   
❑ Does C code treat string pointers and character arrays differently?   
❑ Does C code follow the convention of declaring strings to be length CONSTANT+1?   
❑ Does C code use arrays of characters rather than pointers, when appropriate?   
❑ Does C code initialize strings to NULLs to avoid endless strings?   
❑ Does C code use strncpy() rather than strcpy()?    And strncat() and strncmp()?   


Boolean Variables  
❑ Does the program use additional boolean variables to document conditional tests?   
❑ Does the program use additional boolean variables to simplify conditional tests?   


Enumerated Types  
❑ Does the program use enumerated types instead of named constants for their improved readability, reliability, and modifiability?   
❑ Does the program use enumerated types instead of boolean variables when a variable’s use cannot be completely captured with true and false?   
❑ Do tests using enumerated types test for invalid values?   
❑ Is the first entry in an enumerated type reserved for “invalid”?   


Named Constants  
❑ Does the program use named constants for data declarations and loop limits rather than magic numbers?   
❑ Have named constants been used consistently—not used as named constants in some places and as literals in others?   


Arrays  
❑ Are all array indexes within the bounds of the array?   
❑ Are array references free of off-by-one errors?   
❑ Are all subscripts on multidimensional arrays in the correct order?   
❑ In nested loops, is the correct variable used as the array subscript, avoiding loop-index cross-talk?   


Creating Types  
❑ Does the program use a different type for each kind of data that might change?   
❑ Are type names oriented toward the real-world entities the types represent
rather than toward programming-language types?   
❑ Are the type names descriptive enough to help document data declarations?   
❑ Have you avoided redefining predefined types?   
❑ Have you considered creating a new class rather than simply redefining a type?   
