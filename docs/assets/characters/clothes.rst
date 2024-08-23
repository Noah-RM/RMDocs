Clothing Design
###############

* Create and fit character clothes according to references and the script breakdown

  * Load Character FBX 

    * **Uncheck** Joint Animation to keep the static pose! 

  * The Character must be in the "Open A_UE4" pose
  * Create clothes and simulate the cloth to fit it to the character
  * For every Fabric type for the created clothes:

    * Name: XX 
    * Set "Material" to PBR
    * Set "Texture Mapping" to repeat
    * Basic Parameters:

      * Texture (color/map)

        * Change texture settings (if necessary)
    
      * Normal Map (map)

        * change intensity to ``25`` or greater (until it is noticeable)

      * Reflection

        * Roughness: 

          * Intensity (default) 
          * **Use this map only if you need certain parts to be reflective!**

            * Select desired "Intensity", from ``0`` to ``100`` (0 = full reflectivity, 100 = maximum roughness)
            * Select desired "Reflection Intensity", from ``0`` to ``100`` (controls overall brightness/opacity of reflection)
            * Select desired "Metalness", **either** ``0`` *or* ``100`` (0 = non-metallic, 100 = maximum metalness)

              * Author's note: In the PBR system, metallics are not an either/or, they vary inbetween 0 and 100 depending on the kind of metal and other factors.
  
