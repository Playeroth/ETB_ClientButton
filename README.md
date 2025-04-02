A reusable source for Mod Developers of ETB (Escape The Backrooms) that wants a button to check if clients interacted with something without the need of everyone using the mod. This mod uses an ingame object with custom functions that will work across the network and able to trigger other things by Developer choices. 

this source is used in the mod "InsanityMod" for checking buttons across the map and then if conditions are met based on these interactions. 

# How To Use
![image](https://github.com/user-attachments/assets/d1c4e7b6-9d32-41eb-b793-aa5f98668e73)

- "Transform Relative to Owner" is used to set up position, scale and rotation to properly hide the radius of the original interactable.
----
- "ID" is used to identify which Interactable is available.  
----
- "Start Type" is used for when the object is created and what condition it will receive.  
![image](https://github.com/user-attachments/assets/66eb054c-7860-44f1-9935-0679650787d1)
----
- "Use Type" is used upon interaction and what condition it will be set.  
![image](https://github.com/user-attachments/assets/117ad7a0-9295-4e68-91d7-3b603a6d9eb9)  
- CanCheckAndInteract = A normal function, will check the interaction of this custom interactable.
- NoCheckNorInteract = Wont check neither interact, nothing.
- NoCheckButInteract = Wont check but players can interact, usefull to block players from opening doors or interacting with something if its not ready to.
----
- "Is Comp Hidden" is mostly for debug purposes if you need to understand how it looks like.  
----
![image](https://github.com/user-attachments/assets/1346b8dc-1757-4812-adc2-b1207f7eab9c)  
Sets whether is enabled or not.

## Events 
![image](https://github.com/user-attachments/assets/a3a6d0d2-2404-41ed-bdeb-1b8ee11aa076)  
You can set up Events upon creation. The Event above is called when interaction has executed.  

![image](https://github.com/user-attachments/assets/6eabb202-eb46-4927-b0a9-0cddf639c4de)  
The Event above is called when component is destroyed, destroying also the Latch. It might be not as usefull as the interaction event.

# Examples
![image](https://github.com/user-attachments/assets/8de8c95d-9874-480c-bf62-134d3ef09c63)  
this is an example that is used in "InsanityMod" that checks if all Levers is executed.

# Behind the scenes
It spawns a Latch object of the game. It checks whether or not the latch float value has changed. the game has a value if its moving or not, so i found about that and now use it as a form of interaction check that works for clients without the mod. 
![image](https://github.com/user-attachments/assets/59babf68-95b2-411e-86a9-f2cf20b59679)
