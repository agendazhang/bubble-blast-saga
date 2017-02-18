CS3217 Problem Set 5
==

**Name:** Mok Wei Xiong, Edmund

**Matric No:** A0093960X

**Tutor:** Delon Wong

### Rules of Your Game

Your answer here


### Problem 1: Cannon Direction

The user may use either a *Long Press* or *Pan Gesture* to select the cannon direction. Pressing anywhere on the game area (which is the entire screen) will activate the *Long Press* Gesture recognizer, and the cannon will immediately turn to face the direction of the user's finger. If that is not enough, the user can then pan around the screen with his finger, and the cannon will automatically follow the user's finger so that the user can define a more accurate direction to fire in. Once the user is satisfied with the cannon angle, he may simply release his finger from the screen and the bubble is fired at the direction his finger was last present at (before release).


### Problem 2: Upcoming Bubbles

As of now, my algorithm for deciding the colors of the next few bubbles is to just generate a random number and get the associated colored bubble according to that random number. Effectively, the upcoming bubbles will be randomly generated.

I am planning to display the current bubble, as well as the next upcoming bubble.

### Problem 3: Integration

#### How my design allowed the integration

My design for the Level Designer side and Game Engine side both use the same underlying BubbleGridModel / BubbleGridModelManager. As such, when the user presses the **START** button, I just need to segue from the Level Designer View Controller to the Game View Controller and in the process pass the same underlying BubbleGridModel from the LevelDesignerViewController to the GameViewController. As the GameViewController loads up, it will then load the model received by the LevelDesigner into the Game Engine, and then start the game engine, so that the bubbles in the bubble grid are in the game engine, and can be interacted with as physics objects and rendered on screen. 

In short, I only had to pass my model to my game view controller, and created another method to iterate through the model and each bubble in the bubble grid to the game engine.  

#### What are the alternative approaches?
1. 

#### Advantage vs alternative approaches
1. 


#### Disadvantage vs alternative approaches
1. 

### Problem 4.3

Your answer here


### Problem 7: Class Diagram

Please save your diagram as `class-diagram.png` in the root directory of the repository.

### Problem 8: Testing

Your answer here


### Problem 9: The Bells & Whistles

Your answer here


### Problem 10: Final Reflection

Your answer here
