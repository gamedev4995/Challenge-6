## Enemy Manager

## Floor Manager
This manager will keep track of the floor list with each panel as well as their initialization and deletion.

We created an empty object (GameObject > EmptyObject) and renamed it 'FloorManager' where we added a new script (Add Component > New Script) called 'floorManager'.

[pic]

In this script we added the following libraries and variables:

[pic]

Then we added the Singleton to prevent multiple instances of FloorManager.

[pic]

To initialize the floor panels, we added the following code in the Start() function:

[pic]

Then comes the RemoveFloor() function to be able to remove each singular floor panel.

[pic]

Afterwards, we did a RemoveAllFloors() function to instantly remove all floors as part of a game mechanic.

[pic]

_Note:_ These are the functions that are called in the wall detection scripts.

