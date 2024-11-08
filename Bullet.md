## Bullet Prefab

## Scripts
[other scripts]

We added two more scripts dedicated to the detection of walls for our game mechanics, one for the corner walls and the other for the regular walls.

For the corner walls we first added the following:

[pic]

_Note:_ Make sure that the argument in NameToLayer is written the same as the layer previously created and added to the corner walls.

Then we tested:

[gif]

Additionally, we concluded the script by calling a function from a floor manager script mentioned later on.

[pic]

For the regular walls, the code is the same in exception to the NameToLayer argument.

[pic]

Then we tested:

[gif]

Same as before, we concluded the script by calling another function from the floor manager script.

[pic]

