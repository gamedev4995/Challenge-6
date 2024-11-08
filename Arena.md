## Base
For the mini game area, we first started off by making a template to later create the arena. 
This template/base can be done in multiple ways, but in our case, we first formed a large square with four semi-thin walls by using cubes (GameObject > Cube) and shaping them into rectangles.

[pic]

Then we took another cube, flattened it, and made it large enough to be placed beneath the four walls as a floor.

[pic]

Lastly, we duplicated that floor and positioned it at a lower height beneath it. This will serve as a trigger for a future purpose.

[pic]

## Arena
With this template we proceeded to begin creating the arena. 
_Note:_ the following models come from the Sci-fi Styled Modular Pack that is free to download from the asset store.

### Floor
Starting off with the floor, we grabbed the floor_5 model from the Sci-fi pack and scaled it roughly to the size we wanted.

[pic]

Then we added two things for future purposes:
-	Box Collider (Add Component > Physics > Box Collider)
  
-	[pic]
  
-	Layer (Inspector Tab > Layer (Default) > Add Layer)
  
-	[pic]
  
We then proceeded to duplicate this floor panel and placed them side by side until forming a 4x4 area (16 floors).

[pic]

### Walls:
Next, we placed a corner wall from our asset, placed it on one of the corners of the floor and scaled it to our preferred size.

[pic] 

_Note:_ For extra details, we created a new material, chose our preferred color, and dragged it onto the model.

Then, we took a wall prefab from our asset and scaled it about the size of our corner wall but made them thin enough to fit seven of them for each side of the floor.

[pic]

_Note:_ Be sure to also add box colliders for both the corner and regular walls as well as individual layers for each.

For easy management, we created an empty object, named it 'Wall 1' and dragged all the wall prefabs into it.

[pic]

With this, we duplicated that empty object called 'Wall 1' and proceeded to place down the rest of the walls.

[pic]

## Result:
[pic]

