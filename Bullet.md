# Bullet Prefab

For the bullet, we first created a sphere (GameObject > 3D Object > Sphere) and scaled it down to a small size.

<img width="300" alt="Screenshot 2024-10-04 134242" src="https://github.com/user-attachments/assets/acaf376c-14b3-4ffa-83da-45480abd67a4">

Then we created a new material by right clicking > Create > Material in the assets area or by clicking the ‘+’ symbol > Material.

<img width="385" alt="Screenshot 2024-10-04 133959" src="https://github.com/user-attachments/assets/0f89feb3-595c-4d58-b969-8d4ed8ec6944">

In the inspector tab of the material, within 'Surface Inputs', we changed the 'Base Map' to our choice of color and added an emission for a glowing effect. 

<img width="300" alt="Screenshot 2024-10-04 134147" src="https://github.com/user-attachments/assets/f2be6b3f-7f4f-41d3-a2ce-977a74201218">

Then we dragged the material onto the sphere previously created. 

<img width="300" alt="Screenshot 2024-10-04 134252" src="https://github.com/user-attachments/assets/31d19f82-db86-46df-97ff-50adc5713589">

With the bullet’s look completed, we turned it into a prefab by dragging the object from the Hierarchy tab onto a prefab folder.

---

## Contact Damager

To start off with the bullet's scripts, we Add Component > New Script and named it Contact Damager. This script will ensure that when you hit an enemy, it takes away health each time a bullet hits them and ultimately causing them to be destroyed.

<img width="440" alt="Screenshot 2024-11-08 at 7 41 53 PM" src="https://github.com/user-attachments/assets/e2dc81eb-d507-4460-8f63-361d15ad779a"> 

___Note:___ Make sure to add a damage value in unity; we used 10.

---

## [other scripts]

We added two more scripts dedicated to the detection of walls for our game mechanics, one for the corner walls and the other for the regular walls.

For the corner walls we first added the following:

<img width="600" alt="Screenshot 2024-11-07 143626" src="https://github.com/user-attachments/assets/256dd357-9e4e-4862-a4e8-c333451c0448">

_Note:_ Make sure that the argument in NameToLayer is written the same as the layer previously created and added to the corner walls.

Additionally, we concluded the script by calling a function from a floor manager script mentioned later on.

<img width="400" alt="Screenshot 2024-11-08 162936" src="https://github.com/user-attachments/assets/54a80a32-549a-4347-b107-4571fc96f06a">

For the regular walls, the code is the same in exception to the NameToLayer argument.

<img width="600" alt="Screenshot 2024-11-07 143553" src="https://github.com/user-attachments/assets/f883131c-a5ca-4c3f-9f0b-213b464f468d">

Same as before, we concluded the script by calling another function from the floor manager script.

<img width="400" alt="Screenshot 2024-11-08 162914" src="https://github.com/user-attachments/assets/0054872d-485f-4034-b45d-edc7a4446916">

Then we tested:

![WallDetectVid-ezgif com-video-to-gif-converter (1)](https://github.com/user-attachments/assets/b52e43eb-069b-4c7b-ae66-77731c3007f5)



