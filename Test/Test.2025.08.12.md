
# AdvProg - Test 12/08/2025


## Problem - Puppy Simulator
Using the State pattern, create a puppy simulator program that has two basic functions: to feed or play with the puppy.   
The puppy will react differently to these functions based on which state it is currently in.   
The puppy has three possible states: asleep, eating, or playing.  

Use the following state diagram to decide how the puppy reacts to each function in each state:  
<img width="827" height="481" alt="image" src="https://github.com/user-attachments/assets/bc9a269f-8dd5-4685-9b63-6e0a1a659438" />

• The puppy simulator should begin in the asleep state.  
• When the puppy is asleep, the only way to wake it up is to feed it. It will come running when it hears its food bowl being filled.  
• When the puppy is eating, it can continue to eat until it’s so full that it will fall back asleep (after ~2 or 3 times), or if you can distract it with a ball, then it will play with you.  
• When the puppy is playing, you can continue playing with it until it gets so tired that it falls   asleep again (~2 or 3 times).
• You should not be able to play with puppy when it is asleep (it should continue sleeping) and you should not be able to feed the puppy when it is playing (it should ignore the food).  

Use the following UML diagram to create your puppy simulator (in python):  
<img width="2817" height="1086" alt="image" src="https://github.com/user-attachments/assets/73e86324-a837-4f5f-b1be-fc695eaaf1c3" />

**Classes:**

1. (3 points) Puppy – the object that the user interacts with.  
a. Attributes: _state, _feeds, _plays – add properties for feed and plays.  
b. __init__(self) / Puppy() – initializes the state to the asleep state, and then initializes the number of feeds and plays.  
c. properties for feed and plays.  
d. change_state(new_state) – updates the puppy’s state to the new state.  
e. throw_ball() – calls the play method for whichever state the puppy is in.  
f. give_food() – calls the feed method for whichever state the puppy is in.  
g. inc_feeds() – increments the number of times the puppy has been fed in a row.  
h. inc_plays() – increments the number of times the puppy has played in a row.  
i. reset() – reinitializes the feeds and plays attributes.  

2. (1 point)  PuppyState – interface  
a. feed(puppy) – abstract (no code)  
b. play(puppy) – abstract (no code)  

3. (3 points)  The Three Concrete States: StateAsleep, StatePlay, StateEat –  
a. feed(puppy) – use the state diagram to implement the puppy’s reaction to feeding according to which state class you’re writing. Returns a string describing the puppy’s reaction.  
b. play(puppy) – use the state diagram to implement the puppy’s reaction to playing according to which state class you’re writing. Returns a string describing the puppy’s reaction.



5. (2 points)  Main – construct a puppy object and then display a menu that allows the user to play with or feed the puppy. Display the puppy’s reaction to the user’s choice. Repeat until the user chooses to quit.
  
**Demo** (1 point)   


## **Submission Requirements:**
Link:  https://mlearning.hoasen.edu.vn/mod/assign/view.php?id=1175654  

**Submit 3 parts:**
1. 3-5 screenshots demonstrating the application execution.
2. 3-5 Image(s) of code implementing the chosen classes.
3. containing the C++ files.
