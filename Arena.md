## Base
For the mini game area, we first started off by making a template to later create the arena. 
This template/base can be done in multiple ways, but in our case, we first formed a large square with four semi-thin walls by using cubes (GameObject > Cube) and shaping them into rectangles.

<img width="292" alt="Screenshot 2024-11-07 141509" src="https://github.com/user-attachments/assets/f836ae95-68ca-44e5-9c6c-08479f9a7002">

Then we took another cube, flattened it, and made it large enough to be placed beneath the four walls as a floor.

<img width="292" alt="Screenshot 2024-11-08 144655" src="https://github.com/user-attachments/assets/3008ef2f-f6fd-48bb-96fe-1d78f5010141">

Lastly, we duplicated that floor and positioned it at a lower height beneath it. This will serve as a trigger for a future purpose.

<img width="320" alt="Screenshot 2024-11-07 201944" src="https://github.com/user-attachments/assets/d0d8885e-ce60-49a7-a624-4f4929250c93">

For the trigger to work, we added a box collider (Add Component > Physics > Box Collider)

<img width="320" alt="Screenshot 2024-11-05 132207" src="https://github.com/user-attachments/assets/d532b58d-f705-495f-80f6-3f663a12d103">

Checked the 'Is Trigger' box

<img width="320" alt="Screenshot 2024-11-08 145159" src="https://github.com/user-attachments/assets/1b8ba85d-0e5b-4fbd-8d4b-76778a191012">

Added a layer (Inspector Tab > Layer (Default) > Add Layer)

<img width="320" alt="Screenshot 2024-11-08 150030" src="https://github.com/user-attachments/assets/954bee1d-9034-4c69-9c7d-2b8372df4e4c">

## Arena
With this template we proceeded to begin creating the arena. 
_Note:_ the following models come from the Sci-fi Styled Modular Pack that is free to download from the asset store.

### Floor
Starting off with the floor, we grabbed the floor_5 model from the Sci-fi pack and scaled it roughly to the size we wanted.

<img width="292" alt="Screenshot 2024-11-07 142630" src="https://github.com/user-attachments/assets/7f5449c4-27f2-45f2-946d-dfd9cb6cb82d">

_Note:_ Be sure to add a box collider and a layer as well.
  
We then proceeded to duplicate this floor panel and placed them side by side until forming a 4x4 area (16 floors).

<img width="292" alt="Screenshot 2024-11-07 142728" src="https://github.com/user-attachments/assets/f35c467b-6f85-404c-9b8a-86072d873610">

### Walls:
Next, we placed a corner wall from our asset (model: window_big_corner_plug), positioned it on one of the corners of the floor and scaled it to our preferred size.

<img width="292" alt="Screenshot 2024-11-07 142835" src="https://github.com/user-attachments/assets/e26e93d8-0ce6-4855-8da7-1b4325118647">

_Note:_ For extra details (optional), we created a new material, chose our preferred color, and dragged it onto the model.

Then, we took a wall model from our asset (model: wall_big_no_side_full_LOD0) and scaled it about the size of our corner wall but made them thin enough to fit seven of them for each side of the floor.

<img width="292" alt="Screenshot 2024-11-07 142940" src="https://github.com/user-attachments/assets/90fa771e-05c7-4fe8-b851-508ad182f57a">

_Note:_ Be sure to also add box colliders for both the corner and regular walls as well as individual layers for both.

Then we duplicate the wall for a total of seven walls.

<img width="292" alt="Screenshot 2024-11-07 143033" src="https://github.com/user-attachments/assets/286ae600-b527-4e13-89f1-b98490c16b37">

For easy management, we created an empty object, named it 'Wall 1' and dragged all the wall prefabs into it.

<img width="292" alt="Screenshot 2024-11-08 152410" src="https://github.com/user-attachments/assets/a13965f3-bed8-4785-b7b9-f7adf54cf7d3">

With this, we duplicated that empty object called 'Wall 1' and proceeded to place down the rest of the walls.

<img width="292" alt="Screenshot 2024-11-07 143117" src="https://github.com/user-attachments/assets/59c8f67a-5e21-41d8-ad4f-a52127735229">

## Result:

<img width="292" alt="Screenshot 2024-11-07 143140" src="https://github.com/user-attachments/assets/b4442b64-aa71-4f53-884d-8729fe309498">


