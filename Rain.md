##Rain

To make our mini game more interesting let’s add rain. To do this first create a 3D object sphere that is as big as a beach ball (Use the player model for size comparison). This will be our raindrop. 
<img width="600" alt="Screenshot 2024-11-08 at 6 49 19 PM" src="https://github.com/user-attachments/assets/5ec2e50a-7452-46cc-9fb7-1ae7da617bff">


Add detail by creating a material that is blue and mimics water to your liking and add it on top of our sphere. 

<img width="600" alt="Screenshot 2024-11-08 at 6 51 53 PM" src="https://github.com/user-attachments/assets/955aefe1-b4e3-45a0-9f1f-c53d063e2eb9">


Now drag the object into the prefab folder to create a variant. This is the object we will be working on.

<img width="791" alt="Screenshot 2024-11-08 at 7 08 36 PM" src="https://github.com/user-attachments/assets/12674d1d-8eb0-47b7-ba09-24f0f57f7680">


On this prefab add a new component and search "Rigidbody" and make sure to check the Gravity box.

<img width="255" alt="Screenshot 2024-11-08 at 7 11 35 PM" src="https://github.com/user-attachments/assets/414c2fa3-5bba-4d71-be1f-61db2c266f94">

Next we need to create rain spawners, similar to our enemy spawners, but in this case we want our rain to appear randomly from the sky. Create an empty object and name it “Rain Spawner.” Add a new component and create a new script with the same name.

<img width="1047" alt="Screenshot 2024-11-08 at 7 20 12 PM" src="https://github.com/user-attachments/assets/24aaf8e4-2786-42c5-972b-2aadd2b0f2ca">


We want our spawners to drop multiple raindrops on the stage and the rain to have a specific behavior. Each raindrop can be affected, or moved, by an enemy or player. Meaning the rain does not go through them. The movement of the enemies should not be affected by the rain. Unlike the enemy the player is affected and hindered by the rain. It’s important to note that while the player will be impacted by the rain drops, their bullets won’t collide with them. In other words, the bullets pass through them.

Next inside the scrip folder in your project create a new script called "Raindrop." This is where we will adjust the raindrops behavior. Click on the scrip to open it in your VS Code. 


