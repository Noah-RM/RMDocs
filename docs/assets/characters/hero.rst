Character Design
################

Character Creator
*****************
* Build character according to references and ``script breakdown``

  * Load a base (usually CC4 Neutral Base) 
  * Use Morph Sliders for head/body sculpting
  * Make major changes to the skin by adjusting the Material Textures
  * Add features on the skin using the Appearence editor
  
.. attention::
    All Sliders/Morph Packages are under David's Reallusion Account. Please use David's
    Reallusion Account to be able to export to iClone or Third-Party programs.

Shoes
*****

* Add shoes .OBJ from clothes (If importing new shoes, it must first be imported on the avatar on which it was created.)

  * Create -> Accesory -> Choose the .OBJ 
  * Transfer Skin Weights, Select the "Shoes" profile
  * Conform (Under Modify panel) -> Calculate Collision (repeat as many times and needed)
  * Turn shoes into custom assets

.. important::
    At this point, get internal approval from Loukianos and/or Komiotis!

Exporting from CC
*****************

* Install `Unreal Engine Auto-Setup <https://www.reallusion.com/auto-setup/unreal-engine/default.html>`_
* Install `Blender Auto-Setup <https://github.com/soupday/cc_blender_tools/releases>`_

* In the Content panel, browse to Template -> Item(tab) -> Animation -> Pose -> Calibration -> _`Open A_UE4`

  * Alternatively, search in the Content tab for "Open A_UE4" or "UE4"

* Select the character and go to File -> Export -> FBX -> Clothed Character
* Export for Blender grooming and Wardrobe fitting, using the following settings:

  * Target Tool Preset -> Unreal
  * FBX Options -> Mesh + Motion
  * Texture Settings -> Embed Textures
  * Include Motion (tab)

    * Frame Rate -> 30fps 
    * Current Pose
    * **Uncheck** First Frame in Bind-Pose

* Send FBX to Clothes team
* Select character and export in iAvatar, using the following settings:

  * Max Texture Size: 4096 x 4096 
  * Texture Quality:

    * Set to Highest for Hero Characters
    * Set to High for Secondary Characters

* Upload CC Project & iAvatar files and update Animators

