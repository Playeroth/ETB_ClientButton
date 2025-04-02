# ETB_ClientButton
A reusable source for Mod Developers of ETB (Escape The Backrooms) that wants a button to check if clients interacted with something without the need of everyone using the mod. This mod uses an ingame object with custom functions that will work across the network and able to trigger other things by Developer choices. 

this source is used in the mod "InsanityMod" for checking buttons across the map and then if conditions are met based on these interactions. 

# How To Use
![image](https://github.com/user-attachments/assets/d1c4e7b6-9d32-41eb-b793-aa5f98668e73)

----
- "Transform Relative to Owner" is used to set up position, scale and rotation to properly hide the radius of the original interactable.
----
- "ID" is used to identify which Interactable is available.  
----
- "Start Type" is used for when the object is created and what condition it will receive.  
![image](https://github.com/user-attachments/assets/44fff8c9-8910-474c-b989-2d8dced76304)
----
- "Use Type" is used upon interaction and what condition it will be set.  
![image](https://github.com/user-attachments/assets/1c130700-cd7d-4ce1-8b9c-04a09dbafbe4)
----
- "Is Comp Hidden" is mostly for debug purposes if you need to understand how it looks like.
----
