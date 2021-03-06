How to use the toolbox for Non-Rigid Structure from Motion.

Creating the data
#################

The toolbox comes with a tool to create automatic Animation objects:

.. code-block:: matlab

  anim=generateToyAnimation(3.2)

3D reconstruction
#################

3D reconstruction only works for orthographic camerasso far.

.. code-block:: matlab

  anim = computeNrsfm( method, W )

where method is one of the followg:
  * 1: Torresani (PAMI 08)
  * 2: Xiao, Kanade (IJCV 06)
  * 3: MSFM Rabaud, Belongie (CVPR 08). This method is not yet delivered with this toolbox for performance issues (available at your own risks).
  * 4: CSFM Rabaud, Belongie (CVPR 09)
