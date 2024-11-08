## Bullet Prefab

## Scripts
[other scripts]

We added two more scripts dedicated to the detection of walls for our game mechanics, one for the corner walls and the other for the regular walls.

For the corner walls we first added the following:

<img width="500" alt="Screenshot 2024-11-07 143626" src="https://github.com/user-attachments/assets/256dd357-9e4e-4862-a4e8-c333451c0448">

_Note:_ Make sure that the argument in NameToLayer is written the same as the layer previously created and added to the corner walls.

Additionally, we concluded the script by calling a function from a floor manager script mentioned later on.

<img width="500" alt="Screenshot 2024-11-08 162936" src="https://github.com/user-attachments/assets/54a80a32-549a-4347-b107-4571fc96f06a">

For the regular walls, the code is the same in exception to the NameToLayer argument.

<img width="500" alt="Screenshot 2024-11-07 143553" src="https://github.com/user-attachments/assets/f883131c-a5ca-4c3f-9f0b-213b464f468d">

Same as before, we concluded the script by calling another function from the floor manager script.

<img width="400" alt="Screenshot 2024-11-08 162914" src="https://github.com/user-attachments/assets/0054872d-485f-4034-b45d-edc7a4446916">

Then we tested:

[gif]



