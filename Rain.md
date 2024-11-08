##Rain

To make our mini game more interesting let’s add rain. To do this first create a 3D object sphere that is as big as a beach ball (Use the player model for size comparison). This will be our raindrop. 
<img width="600" alt="Screenshot 2024-11-08 at 6 49 19 PM" src="https://github.com/user-attachments/assets/5ec2e50a-7452-46cc-9fb7-1ae7da617bff">


Add detail by creating a material that is blue and mimics water to your liking and add it on top of our sphere. Now drag the object into the prefab folder to create a variant. This is the object we will be working on.
<img width="600" alt="Screenshot 2024-11-08 at 6 51 53 PM" src="https://github.com/user-attachments/assets/955aefe1-b4e3-45a0-9f1f-c53d063e2eb9">

Next we need to create rain spawners, similar to our enemy spawners, but in this case we want our rain to appear randomly from the sky. Create an empty object and name it “Rain Spawner.” Add a new component and create a new script with the same name.


We want our spawners to drop multiple raindrops on the stage and the rain to have a specific behavior. Each raindrop can be affected, or moved, by an enemy or player. Meaning the rain does not go through them. The movement of the enemies should not be affected by the rain. Unlike the enemy the player is affected and hindered by the rain. It’s important to note that while the player will be impacted by the rain drops, their bullets won’t collide with them. In other words, the bullets pass through them.

