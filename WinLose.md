## Win and Lose Screens
As the last part of our mini game, we had to make a win/lose mechanic. For this we wanted an orange sphere to represent a win and a red cube to represent a loss.

We started off by creating each individual win/lose scene. When creating a new scene, we went to File > New Scene > Standard URP > Create.

We made sure to name our first scene, 'WinScreen' and proceeded to add a sphere.

[pic]

After adding the sphere, in our Materials folder in Assets, we created a new material and changed its base color to orange.

[pic]

_Note:_ Be sure to position it on front of the Main Camera view.

[pic]

For the other scene, we named it 'LoseScreen' and proceeded to add a cube.

[pic]

Then we took the same steps in creating a new material but this time we chose a red color.

[pic]

After creating each scene, [menu part goes here...]

As a last step to our win/lose mechanic, we had to create a new script to establish the win/lose conditions.

First, we created an empty object (GameObject > EmptyObject) and renamed it as ‘GameMode’. Here, we added a new script called ‘GameMode’ (Add Component > New Script).

[pic]

In this script, we used the following libraries and added the following code in the Start() function so that it calls for the CheckWinCondition() function.

[pic]

Then we added each win/lose function. The winning function is the following:

[pic]

The losing function is the following:

[pic]

Result:

[gif]

