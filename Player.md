# Player 

## Rigid Body

We first start off by adding a Rigidbody component to our character. The Rigidbody will allow physic properties to our character like gravity, collisions, and other physical interactions.

<img width="292" alt="Screenshot 2024-10-13 at 3 04 00 PM" src="https://github.com/user-attachments/assets/957304a5-aece-46ec-8364-926c5723a3c1">


## Capsule Collider

Next, we add a capsule collider to grasp the shape of our character. We adjusted the y-coordinate based on our character height and radius based on width.

<img width="293" alt="Screenshot 2024-10-13 at 3 08 23 PM" src="https://github.com/user-attachments/assets/a323a70f-b78b-44b9-844e-07bf9cac9b5d">


## Player Input 

Afterwards, to take in our player's input, we added the component 'Player Input'. We then hit Create Action > named it 'Movement' > Save.

<img width="293" alt="Screenshot 2024-10-13 at 3 13 05 PM" src="https://github.com/user-attachments/assets/da206ca3-884f-439f-a390-0cd11c3c6ac9">

## Script

For our player movement, we first added a new script where we would write the code. Clicking on the character, to the left where the 'Inspector' window appears, scroll all the way down and click Add Component > New Script, we named it "PlayerMove". Afterwards, we opened the new script and began coding our actions.

___Note___: Be sure to add the library InputSystem for your player's input!

<img width="400" alt="Screenshot 2024-10-13 at 3 26 39 PM" src="https://github.com/user-attachments/assets/1fd39414-92a2-4618-946f-246258be9f6a">



  ### > Horizontal & Vertical Movement 

In our Movement Input Actions (player input actions), we made sure to have our select keys (WASD or arrows) for each movement properly adjusted.

<img width="432" alt="Screenshot 2024-10-13 at 5 05 29 PM" src="https://github.com/user-attachments/assets/99083e36-3480-43ea-aed2-8267e836ff3c">

For our player's movement around the map, we created two variables: 'speed' and 'movementValue'.

<img width="512" alt="Screenshot 2024-10-13 at 3 27 52 PM" src="https://github.com/user-attachments/assets/2c74772d-116f-4dc8-befa-b841bc0d9512">

___Note:___ In Unity, be sure to add a desired value for speed.

<img width="350" alt="image" src="https://github.com/user-attachments/assets/f88cce76-e34d-41eb-a29f-8e1a6b889a07">

We then added our function OnMove to detect the player's movement if they're pressing any of the selected keys to move horizontally or vertically.

<img width="468" alt="Screenshot 2024-10-13 at 3 33 10 PM" src="https://github.com/user-attachments/assets/7181efc9-4545-47fc-8533-6b8423b720f3">

#### Result:

![ezgif com-crop](https://github.com/user-attachments/assets/d9cc9c3c-6f78-49de-b2a6-3f65643dbc38)

---
  
  ### > Shoot

For the character to shoot the bullets, we first had to create an empty object (GameObject > empty) which we referred to as ShootPoint, positioned it where we would want the bullets to come out of and then moved the object onto the hierarchy of the asset.

<img width="600" alt="Screenshot 2024-10-04 140608" src="https://github.com/user-attachments/assets/f022df58-7cca-44ba-ac3b-b7dc88f62510">

Back in with the movement script:

We added two public variables, one called 'prefab' and the other 'shootPoint'.

<img width="600" alt="Screenshot 2024-10-13 222847" src="https://github.com/user-attachments/assets/4616655a-5eb5-46b6-ada4-48356d7add1b">

Continuing, we added the following OnFire function, based on the Fire action already established by Unity, that creates an instance/copy of the bullet prefab and positions it where the shooting point object is located once the left mouse button is pressed.

<img width="700" alt="Screenshot 2024-10-12 213631" src="https://github.com/user-attachments/assets/278a7512-6149-45f2-ae55-c195d39de72b">

Lastly, in Unity, drag the bullet prefab and the shootPoint empty onto their respective variables.

<img width="350" alt="Screenshot 2024-10-04 161206" src="https://github.com/user-attachments/assets/09a3b2d7-8a1d-45f6-ba20-fd0acf25a3e8">

#### Result:

![OnFireVid-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/f340f864-159e-43c1-99d6-667010abeeff)

---

  ### > Jump 
  
In the player input actions, we added a new action by pressing on the '+' next to "Actions" to which we named "Jump".

<img width="400" alt="Screenshot 2024-10-12 214242" src="https://github.com/user-attachments/assets/1d55efc5-1711-4b21-8f84-b02d36c7a692">

___Note:___ Player input actions refers to the following asset located in the assets folder:

<img width="150" alt="Screenshot 2024-10-13 221515" src="https://github.com/user-attachments/assets/eb5e2479-a524-43df-b6dc-dec5f2ab8c21">

Then, in the binding properties, next to "Path" we assigned the spacebar of the keyboard. This can be done by typing "spacebar" in the search bar or by pressing "listen" button and tapping the spacebar.

<img width="550" alt="Screenshot 2024-10-12 214500" src="https://github.com/user-attachments/assets/516e10de-fb6d-4917-b6b0-9f3d285c7dd8">

Back in our movement script "PlayerMove", we added a new public variable called 'jumpForce'.

<img width="600" alt="Screenshot 2024-10-12 220509" src="https://github.com/user-attachments/assets/9978e12f-f7a7-469f-b31b-762737fecdb4">

___Note:___ Value can be changed for preference.

Lastly, we added the following OnJump function, based on the Jump action we added, to allow the player to jump:

<img width="600" alt="Screenshot 2024-10-12 221303" src="https://github.com/user-attachments/assets/1f0b8f94-8c33-4c0d-81e7-46efc73835f4">

#### Result:

![OnJumpVid-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/116087e7-6317-419d-8073-17d4ae8111d2)

---

  ### > Look
For the player to look around, we started off by adding two variables, once public called 'rotationSpeed' and a private one called 'lookValue'.

<img width="600" alt="Screenshot 2024-10-12 220221" src="https://github.com/user-attachments/assets/652ef5ad-d44e-4241-a473-13aae004e5eb">

___Note:___ In Unity, be sure to add a desired value for rotation speed.

Then, we added the following OnLook function, based on the Look action already established by Unity:

<img width="550" alt="Screenshot 2024-10-12 221608" src="https://github.com/user-attachments/assets/9f5203a6-2ef0-4cc5-acf9-601d391218d7">

Lastly, with the lookValue, we can apply the rotation in the Update() with the following code:

<img width="650" alt="Screenshot 2024-10-12 221826" src="https://github.com/user-attachments/assets/f49f9ebc-0049-49ee-9d66-1d0495fb859b">


#### Result:

![OnLookVid-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/ba801ab6-6eac-47af-9dcd-4e1e8cc0a5bf)

---

  ### > Fast Horizontal & Vertical Movement
  To make our character move fast, as in sprint, first we have to create a new public variable called 'sprintSpeed', which we can set to 0, and a private bool 'isSprinting', which needs to be initialized to 'false'.
  
<img width="600" alt="Screenshot 2024-10-13 at 8 28 13 PM" src="https://github.com/user-attachments/assets/0d2b84a7-ec97-476d-9fe8-6ebbed6b1186">

In the Movement(Input actions) menu create a new action called "Run." Using the plus sign next to the new action created select "add binding." In the path field select the right and left shift key.

  <img width="570" alt="Screenshot 2024-10-13 at 10 41 14 PM" src="https://github.com/user-attachments/assets/2f04bc9c-84b8-453e-958a-9474c48c4603">

  Go back to the code and create a new function called OnRun. This will detect wether the keys we selected are being pressed by the user. Create an if statement that verifies if the user is pressing shift. If true, then set isSprinting to true.
  
  <img width="600" alt="Screenshot 2024-10-13 at 10 38 03 PM" src="https://github.com/user-attachments/assets/e86f5c35-5856-4775-bf60-7005d4d6caee">

  Next we need to adjust the OnMove function. Inside the function add an if/else statement that checks the boolean 'isSprinting'. If 'true' the 'movementValue' will be multiplied by the sprintSpeed. Otherwise the 'movementValue' is multiplied by the regular player speed. Finally set isSprinting to false again. 
  
  <img width="500" alt="Screenshot 2024-10-13 at 8 34 18 PM" src="https://github.com/user-attachments/assets/ca056b1b-6e32-4459-9d1d-52dca1789f81">


  #### Result:

![OnRunVid](https://github.com/user-attachments/assets/e97d6601-ddfd-4886-aa17-4d11f77d616d)


---

## Final Result

![AllActionsVid-ezgif com-optimize](https://github.com/user-attachments/assets/34165bc6-97e5-4502-8188-26dd9904ec7b)




