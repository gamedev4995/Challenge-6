# Win and Lose Screens

As the last part of our mini game, we had to make a win/lose mechanic. For this we wanted an orange sphere to represent a win and a red cube to represent a loss.

We started off by creating each individual win/lose scene. When creating a new scene, we went to File > New Scene > Standard URP > Create.

We made sure to name our first scene, 'WinScreen' and proceeded to add a sphere.

<img width="292" alt="Screenshot 2024-11-07 205017" src="https://github.com/user-attachments/assets/0336bb41-2bf6-450f-9712-3c862717533b">

After adding the sphere, in our Materials folder in Assets, we created a new material and changed its base color to orange.

<img width="292" alt="Screenshot 2024-11-07 204224" src="https://github.com/user-attachments/assets/be53c9f3-c127-44ae-b3d3-5b23d5d4b657">

We then added a text from Game Object > 3D Object > Text and changed it to read "you win!", meaning you won the game. We also changed its color in the inspector window to a brighter one so it's noticeable and contrasts the lose scene.


<img width="300" alt="Screenshot 2024-11-08 at 10 27 22 PM" src="https://github.com/user-attachments/assets/640ca951-a153-403c-9c5c-ef2374d96853">


___Note:___ Be sure to position it on front of the Main Camera view.

<img width="310" alt="Screenshot 2024-11-07 205142" src="https://github.com/user-attachments/assets/812aaab5-f225-42e0-8b30-2dff84801773">

For the other scene, we named it 'LoseScreen' and proceeded to add a cube.

<img width="292" alt="Screenshot 2024-11-08 191408" src="https://github.com/user-attachments/assets/8cc2c6b0-234c-4f07-9979-d5c59587c8ed">

Then we took the same steps in creating a new material but this time we chose a red color.

<img width="310" alt="Screenshot 2024-11-07 205115" src="https://github.com/user-attachments/assets/b8688ca1-2a16-44b9-b423-e3a980bdc830">

For the text, we added a new text in Game Object > 3D Object > Text and changed it now to read "you lose!", meaning it's game over. Then changed its color in the inspector window to a darker one so it's noticeable and contrasts the win scene.

<img width="300" alt="Screenshot 2024-11-08 at 10 23 27 PM" src="https://github.com/user-attachments/assets/f9702dda-f3ca-4f85-813e-12de20e621ad">


Since we want our scenes to be included into the game once the player wins or loses, we added them by going to File > build settings and then dragging our lose and win scenes into the box.

<img width="637" alt="Screenshot 2024-11-08 at 5 43 27 PM" src="https://github.com/user-attachments/assets/6559246d-8d8c-44b2-9690-c41ca11b626b">

As a last step to our win/lose mechanic, we had to create a new script to establish the win/lose conditions.

First, we created an empty object (GameObject > Create Empty) and renamed it as 'GameMode'. Here, we added a new script called 'GameMode' (Add Component > New Script).

In this script, we used the following libraries and added the following code in the Start() function so that it calls for the CheckWinCondition() function.

<img width="500" alt="Screenshot 2024-11-08 130648" src="https://github.com/user-attachments/assets/2c80c82c-d635-4087-8d38-19926883c3fd">

## Win

We added the following winning function:

<img width="700" alt="Screenshot 2024-11-08 131018" src="https://github.com/user-attachments/assets/e34ae611-ede1-4a19-93af-6c7ae3dbb2e8">

## Lose

Then the following losing function:

<img width="600" alt="Screenshot 2024-11-08 131030" src="https://github.com/user-attachments/assets/0a77ff4c-6f59-462f-9130-47078a89f9ea">

___Note:___ The 'Lose Floor' layer refers to the layer belonging to the second hidden base floor mentioned in the Arena creation.

