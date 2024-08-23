Groom Design
############


Blender
*******

Setup
=====


* Import character FBX (using the `CC/iClone Pipeline plugin <https://github.com/soupday/cc_blender_tools/releases>`_ or File -> Import -> FBX)
* Import headgear as an FBX (if needed)
* Select cc_base_body 
* Add (``Shift + A``) Curve -> Empty Hair

* In the properties panel, go to the Render Tab (Camera Icon):

  * Set the Render Engine to Cycles, if it isn't already
  * Under the Curves -> Viewport Display section:

    * Switch it from ``Strand`` to ``Strip``
    * Increase "Additional Subdivion" to ``3``

Sculpting
=========

* Go to Sculpt Mode
* Add Curves using Density with the following options:

  * Distance Min: ``1m``  
  * Count Max: ``10``
  * Increase Curve Shape -> Points for longer hair (up to ``15`` for long hair)

* Comb the curves with the Comb tool set in Projected
* Add Hair in sections, starting low and moving up towards the forehead

* Go to Object Mode
* Add Blender hair assets. Added assets are different for each hair style. Set Hair Curve Profile and Interpolate Hair Curves should always be added.

  * Set Hair Curve Profile is used as is for hair and Radius increases up to ``0.015`` for beards. 
  * Interpolate Hair Curves must be bound on the same surface the parent curves are bound on
  * Distance to guides should be around ``1`` and Density ``30`` to ``40``
  
* For characters wearing veils, after the hair is complete, the curves are combed closer to the head unitl no hair comes out of the cloth (save on a different file)

Export to Alembic File
======================

* Install `Blender Groom Exporter Add-On <https://turbocheke.gumroad.com/l/Groomexporter>`_

* Select all curve objects except for the mustache and click "Button Export" to save as an alembic (.abc)

  * In the pop-up, name it and set scale to ``1``, then save

* Select the moustache curve object and click ``Button Export`` and set scale to ``1``
* Upload and update Animators

 