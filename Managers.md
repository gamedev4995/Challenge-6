## Enemy Manager

## Floor Manager
This manager will keep track of the floor list with each panel as well as their initialization and deletion.

We created an empty object (GameObject > EmptyObject) and renamed it 'FloorManager' where we added a new script (Add Component > New Script) called 'floorManager'.

<img width="292" alt="Screenshot 2024-11-08 153755" src="https://github.com/user-attachments/assets/4ab2ba4b-e1a4-471a-bcfb-8aba40d75ca0">

In this script we added the following libraries and variables:

<img width="292" alt="Screenshot 2024-11-07 143836" src="https://github.com/user-attachments/assets/b34ef31c-5300-4fb7-bf1f-4fe6a4a23bd8">

Then we added the Singleton to prevent multiple instances of FloorManager.

<img width="292" alt="Screenshot 2024-11-07 144538" src="https://github.com/user-attachments/assets/2fd0db33-4fe6-41f6-b574-eef2fd5ded15">

To initialize the floor panels, we added the following code in the Start() function:

<img width="292" alt="Screenshot 2024-11-07 143921" src="https://github.com/user-attachments/assets/28845f29-2db1-4e72-b890-9b6e72f738ea">

Then comes the RemoveFloor() function to be able to remove each singular floor panel.

<img width="292" alt="Screenshot 2024-11-07 143940" src="https://github.com/user-attachments/assets/9902cf9e-88f8-4372-a9f9-9db00c720ca6">

Afterwards, we did a RemoveAllFloors() function to instantly remove all floors as part of a game mechanic.

<img width="292" alt="Screenshot 2024-11-07 144022" src="https://github.com/user-attachments/assets/1b7f6e66-cd88-464e-ad8a-306d9db53a79">

Lastly, we added a RemoveRandomFloor() function to randomize the removal of the floor panels.

<img width="292" alt="Screenshot 2024-11-08 154659" src="https://github.com/user-attachments/assets/13578bbb-c83f-4b3b-b9ef-86dfff8a665d">

_Note:_ These are the functions that are called in the wall detection scripts.

Result:
[gif]

