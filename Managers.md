# Managers

Game managers help with the development of the game and keep track of its components.

---

## Enemy Manager

The enemy manager will keep track of the enemy list that appear in the arena. We created an empty object (GameObject > EmptyObject) and renamed it 'EnemyManager'. To this empty object, we added a new script by going to Add Component > New Script and named it 'EnemyManager' as well.

In the script we added these variables and libraries:

<img width="657" alt="Screenshot 2024-11-08 at 6 30 49 PM" src="https://github.com/user-attachments/assets/86ac78da-efeb-4a30-983c-eb80fdd69522">

We then added AddEnemy and RemoveEnemy so that it manages the enemy list.

<img width="297" alt="Screenshot 2024-11-08 at 6 36 02 PM" src="https://github.com/user-attachments/assets/ae3c7e93-1882-424e-86c6-895762c74c10">

To finish the script, we added an Awake so that it takes into consideration if there is a duplicated instance.

<img width="655" alt="Screenshot 2024-11-08 at 6 36 26 PM" src="https://github.com/user-attachments/assets/199a132e-5d0b-4e19-85c1-f29ff66a0e4f">

---

## Floor Manager
This manager will keep track of the floor list with each panel as well as their initialization and deletion.

We created an empty object (GameObject > Create Empty) and renamed it 'FloorManager' where we added a new script (Add Component > New Script) called 'floorManager'.

<img width="220" alt="Screenshot 2024-11-08 153755" src="https://github.com/user-attachments/assets/4ab2ba4b-e1a4-471a-bcfb-8aba40d75ca0">

In this script we added the following libraries and variables:

<img width="600" alt="Screenshot 2024-11-07 143836" src="https://github.com/user-attachments/assets/b34ef31c-5300-4fb7-bf1f-4fe6a4a23bd8">

Then we added the Singleton to prevent multiple instances of FloorManager.

<img width="500" alt="Screenshot 2024-11-07 144538" src="https://github.com/user-attachments/assets/2fd0db33-4fe6-41f6-b574-eef2fd5ded15">

To initialize the floor panels, we added the following code in the Start() function:

<img width="500" alt="Screenshot 2024-11-07 143921" src="https://github.com/user-attachments/assets/28845f29-2db1-4e72-b890-9b6e72f738ea">

Then comes the RemoveFloor() function to be able to remove each singular floor panel.

<img width="500" alt="Screenshot 2024-11-07 143940" src="https://github.com/user-attachments/assets/9902cf9e-88f8-4372-a9f9-9db00c720ca6">

Afterwards, we did a RemoveAllFloors() function to instantly remove all floors as part of a game mechanic.

<img width="500" alt="Screenshot 2024-11-07 144022" src="https://github.com/user-attachments/assets/1b7f6e66-cd88-464e-ad8a-306d9db53a79">

Lastly, we added a RemoveRandomFloor() function to randomize the removal of the floor panels.

<img width="600" alt="Screenshot 2024-11-08 154659" src="https://github.com/user-attachments/assets/13578bbb-c83f-4b3b-b9ef-86dfff8a665d">

___Note:___ These are the functions that are called in the wall detection scripts.

Back in Unity, be sure to drag the parent object containing the floor panels into the slot on the inspector tab.

<img width="290" alt="Screenshot 2024-11-08 161108" src="https://github.com/user-attachments/assets/b7a6d15c-ebdc-487b-9d2f-35e6e8197276">

### Result:

![floorManagerVid-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/2c40b4ce-8c22-46d0-b310-f8224797dbe8)

---

## Rain Manager


---

## Wave Manager

For the wave manager, we created another empty object by going to GameObject > Create Empty and renamed it as 'WaveManager' to which we added a new script to it calling it 'WaveManager' as well.

In the script, we used the following libraries and variables:

<img width="484" alt="Screenshot 2024-11-08 at 8 26 35 PM" src="https://github.com/user-attachments/assets/29dd7973-77bd-4663-b188-eafe9d6c7bf7">

Next we added Add and Remove wave so that it manages the wave list.

<img width="298" alt="Screenshot 2024-11-08 at 8 27 02 PM" src="https://github.com/user-attachments/assets/ca24294e-dadf-43c4-beb0-fa75729aab99">

To finish up, we added an Awake so that it takes into consideration if there is a duplicated instance.

<img width="482" alt="Screenshot 2024-11-08 at 8 27 56 PM" src="https://github.com/user-attachments/assets/9dbf283c-3447-4b4e-95df-f9576b8c365b">


---

## Score Manager

Score manager is simple enough. Just like the others, we created an empty object (GameObject > Create Empty) and renamed it as 'ScoreManager' in which we added a new script with the same name.

In the script, we used the following libraries and variable:

<img width="500" alt="Screenshot 2024-11-08 194122" src="https://github.com/user-attachments/assets/b71c06e3-419a-48fa-a3c8-94fd90bf7c0d">

Then we added the singleton to avoid the repetition of instances.

<img width="500" alt="Screenshot 2024-11-08 194131" src="https://github.com/user-attachments/assets/27d2670f-c42d-4697-a542-9a2f07e6254d">

In Unity, the score will be visible and automatically increment as each enemy is eliminated.

<img width="450" alt="Screenshot 2024-11-08 210218" src="https://github.com/user-attachments/assets/8297f29f-1f5a-43d3-9982-c9ba835ccb51">

