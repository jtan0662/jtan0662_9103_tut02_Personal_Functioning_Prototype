# jtan0662_9103_tut02_Personal_Functioning_Prototype
# **Individual Function**

## **Instructions on interaction**
Interaction here is controlling the elevator moving smoothly to each floor by press the number keys.

- Press 0 to reset the elevator to the ground floor.
- Press 1 to move the elevator to the 1st floor.
- Press 2 to move to the 2nd floor.
- Press 3 to move to the 3rd floor.

## **Thoughts and Inspiration**
My individual approach animated the group code by keyboard inputs for user interaction, I animated the parts of elevator while my other teammates worked on floors of clock, cat and peoples from audio, time-based and Perlin noise and randomness.

I decided to focus on the elevator interaction because it just felt like a natural fit for the modern building theme, which we adapted from Broadway Boogie Woogie. Elevators are such a part of daily life, and adding the button interaction really made sense—just like in real life, you press a floor button, and the elevator comes to you. This matched both our project’s style and my own approach to interactivity.

## **Technical Explanation**
For realizing harmonious elevator interaction, I first focused on setting up the correct dimensions and initial position. I adjusted the size of the elevator box to fit the height of each floor, and then set its starting position on the ground floor instead of in the middle of the canvas.
![Group elevator](picture/Group%20elevator.jpg)
![My elevator after adjust](picture/My%20elevator%20after%20adjust.png)

Afterwards, I clarified the Y coordinates for each floor. For example, the ground floor is at 780, and the third floor is at 120. These coordinates match the different heights that correspond to the number keys.

Then, I used the targetY variable to store the elevator’s target Y coordinate. When the user presses a number key, targetY updates to the corresponding floor’s Y coordinate. Then In the draw() function, I compare the elevator’s current position (elevatorY) with targetY. If elevatorY is less than targetY, that means the elevator needs to move down. I set the speed to 5, so it moves smoothly, mimicking the slow descent of a real elevator.
![Compare code](picture/Compare%20code.png)

At last, I set up keyPressed() to capture the user’s input. When they press a number key (0-3), targetY updates to the correct floor’s coordinate. This way, the elevator moves precisely to the chosen floor, creating an interactive experience for the user.
![Press code](picture/Press%20code.png)

After the main interaction part was done, I made sure all the color parameters were unified across the project. Some colors were already consistent in the group code, but I went through everything and matched the rest to their named variables to keep it all consistent.