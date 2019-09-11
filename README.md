

Assignment Description. Design a class called ComboLock that works like the 3-number combination lock in a gym locker. A combination lock is opened with a simple procedure: turn the lock’s dial to the right until you reach the ﬁrst number in the combination. Then turn the lock to the left until you reach the second number. Finally, turn to the right until the third number is reached. If the three numbers were correct, the lock will open.

A ComboLock object is constructed with three integers from 0-39 representing the combination needed to unlock the object. Create a new C++ program and make a class named ComboLock. Design the class to these speciﬁcations:

You will need three member variables to represent the three integers needed to open the lock. Choose an appropriate type and names for these variables. Make sure your member variables are private and NOT static.
Add a fourth member variable to represent the current position of the lock’s dial (the part that spins).
Add a constructor that takes three values for the lock’s combination and initializes the member variables accordingly. The dial position should start at 0. You may assume the combination numbers are always between 0 and 39.
Add an accessor method getDialPosition(), which returns the current dial position of the lock.
Add these methods to manipulate the lock:
void reset(): set the dial position back to 0 and start the unlocking procedure over again.
void turnLeft(int ticks): turn the dial to the left by the speciﬁed number of ticks from the current position. The ticks parameter is NOT the number you wish to turn to—it is how many positions to move from where you currently are. Example: if the current position is at 10, then turnLeft(10) would turn the dial to 20.
void turnRight(int ticks): likewise, turns the dial to the right by the speciﬁed number of ticks.
boolean open(): attempts to open the lock. If the user’s most recent turnRight, turnLeft, turnRight methods entered the correct three combination numbers, then the method returns true and resets the lock. Otherwise the method returns false and resets the lock.
This method is one of the harder parts of the lab. You will need to add member variables to the ComboLock class to help you with this method. You will need some way of remembering all three numbers that the user spun the lock to. You will also need to make sure the user spun the correct direction each time, not solely that they landed on the right number.
Finally, add documentation comments to each public method of your ComboLock class, as well as the class declaration itself. Include a one-sentence description of what the method does, plus entries for each method parameter, and a return entry if the method has a non-void return value.
Deliverables. Submit your .cpp source code ﬁle in a folder named assign3 in your csci133 folder. Make your compiled ﬁle named assign3. We will be building on this assignment for the next several weeks.
