# ETB_ClientButton
A reusable source for Mod Developers of ETB (Escape The Backrooms) that wants a button to check if clients interacted with something without the need of everyone using the mod. This mod uses an ingame object with custom functions that will work across the network and able to trigger other things by Developer choices. 

this source is used in the mod "InsanityMod" for checking buttons across the map and then if conditions are met based on these interactions. 

# How To Use
![image](https://github.com/user-attachments/assets/cb4040ec-3745-413b-91a9-e7c9136c6db8)

"Actor Attached" is an actor that you may want to attach for localtransforms to work, such as attaching this Interactable into another ingame button but overwrite its interaction.
"ID" can be used to identify which Interactable is available.
"Is Enabled" can be toggled to OFF if you want players to interact but nothing happens, blocking further execution.
"Is Use Once" can be toggled so only one use is considered, future interactions will be disconsidered and not block interaction.
"Visible Static Mesh" can be used to set one key one value for adding meshes and material, mostly for debug as setting Material wont work for Clients without the mod, setting mesh does work.
