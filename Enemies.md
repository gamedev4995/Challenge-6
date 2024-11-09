# Enemies 

To create our enemies, we simply duplicated our player character and removed the 'Player Input' component since these will be npc's (non playable characters). Since our enemies won't be shooting at the player in our game, we can go ahead and remove the empty object 'ShootPoint' as well.

To work with our character easily, we made it into a Prefab variant by dragging the object into out Prefab folder and named it Enemy Variant. Once inside the object, click Add Component > New Script and we're adding four new scripts: Enemy, Forward Movement, Life and Score on Death.

## Scripts 

### > Enemy

This script takes care of adding new enemies onto the arena once called or removing them once the player succesfully destroys them.

<img width="393" alt="Screenshot 2024-11-08 at 5 23 36 PM" src="https://github.com/user-attachments/assets/509e22a9-c958-43bb-ae01-9571477541dc">


### > Forward Movement

This script will handle the speed at which the enemies will be moving at around the arena.

<img width="454" alt="Screenshot 2024-11-08 at 5 29 11 PM" src="https://github.com/user-attachments/assets/d4502d24-ad70-40b3-9235-16cd96c787c3">


___Note___: Remember to set their speed in unity to your preference depending on how fast you want them to go.

<img width="270" alt="Screenshot 2024-11-08 at 10 10 07 PM" src="https://github.com/user-attachments/assets/43170abb-4326-4bb9-b04b-42f108812b9c">


### > Life

This script will handle the life of the enemy once the player shoots at it. It takes into account how much life each enemy has and once their life reaches 0, the enemy is finally destroyed.

<img width="306" alt="Screenshot 2024-11-08 at 5 26 41 PM" src="https://github.com/user-attachments/assets/f59c2cda-f754-4632-bff3-a44a1e07b646">

  
  
___Note___: Remember to set an amount for their life health in unity; the norm is 100.

<img width="266" alt="Screenshot 2024-11-08 at 10 10 44 PM" src="https://github.com/user-attachments/assets/e2571dc9-dee8-4ffb-a5be-0615662b2212">



### > Score On Death

This script will take care of giving the player their points for each enemy they destroy by checking their life.


<img width="377" alt="Screenshot 2024-11-08 at 10 15 31 PM" src="https://github.com/user-attachments/assets/5c43b62d-ea77-49e4-ada1-0287216ca249">


___Note___: Remember to set an amount of points in unity; we used 25 points per enemy.

<img width="269" alt="Screenshot 2024-11-08 at 10 09 35 PM" src="https://github.com/user-attachments/assets/3dcaa81c-7753-4083-bd5f-b46b9c811aec">


