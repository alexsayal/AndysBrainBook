.. _MRtrix_00_Diffusion_Overview:

==================================================
MRtrix Introduction: Overview of Diffusion Imaging
==================================================


.. note::

  This section is still under construction. Please check back soon!
  
---------------

Overview
****************

Until now, this book has touched on the most popular MRI technique: Functional Magnetic Resonance Imaging, or fMRI. These functional images, which measure signal generated by changes in blood flow, are often accompanied by structural images that are acquired using the same basic method: Different tissue types in the brain have different T1 and T2 **relaxation rates**, which are used to create images with contrast between the tissues. In T1, or anatomical scans, the white matter is lighter than the grey matter, which in turn is lighter than the cerebrospinal fluid; in T2, or functional scans, the relative intensities are flipped.

.. figure:: 00_T1_T2_Intensities.png

  Typical T1-weighted (anatomical) and T2-weighted (functional) images. Note how the relative intensities of the tissue types are inverted when going from T1-weighted imaging to T2-weighted imaging.
  
However, there are other types of images that can be acquired with an MRI scanner. In this module we will focus on **diffusion-weighted MRI**, or dMRI, which measures the relative diffusivity within different parts of the brain - in particular, within the white matter tracts.


The Structure of the White Matter
*********************************

Why does dMRI focus on the white matter tracts? Imagine peeling apart a stick of string cheese, and then imagine peeling apart a brain - just like the string cheese, the brain has preferred tear directions. These directions correspond to underlying white matter tracts, which are thick bundles of myelinated neurons that connect both nearby and distant parts of the brain. For example, the inferior longitudinal fasciculus connects the visual and temporal regions of the brain, while the uncinate fasciculus connects the temporal and inferior frontal parts of the brain. These tracts travel along all three dimensions of the brain, and they may run parallel to each other or cross one another.

.. figure:: 00_Tract_Examples.png

The white matter of the brain gets its name from its color; these neurons are highly myelinated, meaning they have a thick lipid coating that both insulates them and helps with the transmission of electrical impulses, just like an insulated electrical cable. The grey matter neurons, in contrast, are relatively unmyelinated, which allows for a higher density of neurons to be packed into a given area.

History of Diffusion
********************

While the composition of the brain tissues has been known for some time, imaging the diffusion of the white matter tracts is a new technique. To understand how the properties of the white matter were exploited for this purpose, we will briefly review of the history of diffusion and how scientists came to apply this concept to imaging the brain.

Brownian Motion
^^^^^^^^^^^^^^^

The first formal description of diffusion was made in 1827 by Robert Brown, a Scottish botanist. While looking at microscopic particles through a microscope, he noticed that the particles seemed to move randomly of their own accord - similar to how motes of dust, when observed moving through a shaft of light, appear to move in random patterns. Browning concluded that the movement was caused by smaller particles impinging upon the larger molecues seen through the microscope. When dye is dropped into water, for example, the random motion of the water molecules causes the dye to disperse at random until the water within the contained reaches a consistent hue. A more common, everyday example can be seen by pouring milk into coffee: Observe how the milk swirls and mixes with its surroundings, and you have an excellent demonstration of Brownian Motion.

The properties of the medium determine the speed of the Brownian Movement. For example, increasing the temperature of the surrounding water will cause the water molecules to move faster, and consequently make the particles move faster as well. If the viscosity of the medium is higher - for example, if we drop food dye into a bowl of honey - the molecules move slower, and the particles of the food dye will move slower. Decreasing the temperature and decreasing the viscosity, on the other hand, will have the opposite effects.

Lastly, and most relevant for our future tutorials on diffusion imaging, the Brownian Movement of both the particles and the molecules is determined by the size and shape of the container. Food dye dropped into a spherical bowl of water will diffuse randomly in all directions. Food dye dropped into a cylindrical beaker, on the other hand, will quickly diffuse along the length of the beaker; the particles will soon run into the walls of the container, and be forced to move either up or down. We call this type of container **anisotropic**, meaning that the dimensions of the container cause the particles to diffuse along a predominant axis. (If you have experience with fMRI, think of anisotropic voxels, which have one dimension that is longer than the others.)

.. note::

  For a video of Brownian Motion, click `here <https://www.youtube.com/watch?v=SB7GlVlm60g>`__.
