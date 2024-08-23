Transfer Groom between characters
#################################

Blender
~~~~~~~

* Import the character to which the hair should be transferred (using the `CC/iClone Pipeline plugin <https://github.com/soupday/cc_blender_tools/releases>`_ or File -> Import -> FBX)
* Choose all Curves objects from the old character
* Hold ``Shift`` + Drag & Drop all Curves objects under the new character's ``CC_Base_Body`` heirarchy
* Delete all the old character's elements:

  * Right Click the old character's name (with a sideways 'Y' icon)
  * Click ``Select Heirarchy``, then delete

.. attention::
   If everything was done correctly, the hair should **disappear** at first!

* For each Curves object:

  * Select it 
  * Under the properties panel, open the Curves tab (3 green lines)
  * Set "Surface" as ``CC_Base_Body``
  * Confirm UV Map is set to ``Channel0``, if not, set it as such
  * Choose the "Modifiers" tab (Wrench icon)
  * Choose the "Interpolate Hair Curves" modifier

    * Set Surface as ``CC_Base_Body``
    * Confirm "UV Map" is set to ``Channel0``
    * **Uncheck** "Surface Rest Position"
    * **Uncheck** "Follow Surface Normals"

  * Select "CC_Base_Body"

    * Check "Add Rest Position" in Data Tab (Green upside-down Triangle)

Fix for Height Differences
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::
   If you notice the hair being lower on the head and less dense than it was before transfer, follow these steps!


* Follow the steps in the previous section
* Select all Curves object
* Go to Sculpt Mode
* To the right of the "Sculpt Mode" dropdown, go to Curves -> "Snap to Deformed Surface"
* The hair should be in the correct position

  
