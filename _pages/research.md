---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

A major theme of my research is developing both software and hardware for high-throughput computational 3D imaging techniques. My interests span the broadest, most inclusive interpretation of "3D", ranging from dense 3D tomography to sparse 3D topography, from the microscale to the mesoscale and macroscale. Some projects include:
- [High-speed volumetric imaging with 2π Fourier light field tomography](#high-speed-volumetric-imaging-with-2π-fourier-light-field-tomography)
- [High-throughput computational 3D imaging with camera arrays](#high-throughput-computational-3d-imaging-with-camera-arrays)
- [Optical coherence refraction tomography (OCRT)](#optical-coherence-refraction-tomography-ocrt)
- [Multiview imaging over extremely wide angular ranges](#multiview-imaging-over-extremely-wide-angular-ranges)
- [Diffraction tomography with a deep image prior](#diffraction-tomography-with-a-deep-image-prior)

## High-speed volumetric imaging with 2π Fourier light field tomography
We developed a Fourier light field system that can capture synchronized video from perspectives spanning 2pi steradians across 10s of cubic mms, enabling multimodal volumetric video at up to 120 fps.

Sample multi-view video acquisition of a *Drosophila* larva:
<center>
<video width="600" controls>
  <source src="/images/fruitfly_larva_multiview.mp4" type="video/mp4">
</video>
</center>
Sample tomographic video reconstruction of a freely swimming GFP-expressing zebrafish:
<center>
<video width="400" controls>
  <source src="/images/zebrafish_fluorescence.mp4" type="video/mp4">
</video>
</center>

Details coming soon!

## High-throughput computational 3D imaging with camera arrays
We present 3D-RAPID (<ins>3D</ins> <ins>R</ins>econstruction with an <ins>A</ins>rray-based <ins>P</ins>arallelized <ins>I</ins>maging <ins>D</ins>evice), a computational 3D imaging technique based on an array of 12-megapixel cameras capable of imaging at extremely high spatiotemporal throughts (>5 gigapixels/sec). 3D-RAPID features a spatiotemporally scalable, physics/self-supervised algorithm that enables simultaneous 3D reconstruction and stitching of arbitrarily many cameras across arbitrarily many temporal frames.
<center><img src="/images/3d-rapid.jpg" alt="3D-RAPID" width="900"/></center>

Our high spatiotemporal throughputs (>5 GP/sec) enable high-resolution 3D imaging of freely behaving organisms over wide FOVs (>130 cm<sup>2</sup>) at high speed (up to 230 fps):
<center>
<video width="700" controls>
  <source src="/images/zebrafish_60fps_tracked.mp4" type="video/mp4">
</video>
</center>
The left panel shows the zoomed-out view of the entire arena of freely swimming zebrafish; the right panels show the zoomed-in individually tracked zebrafish. The video alternates between photometric (RGB) and 3D height information.
<center>
<video width="700" controls>
  <source src="/images/S12_ants_230fps_compressed.mp4" type="video/mp4">
</video>
</center>
Freely moving harvester ants (left: photometric frame, right: 3D height map).

For more videos, see the supplementary materials of the accompanying publication below. See also [https://gigazoom.rc.duke.edu/](https://gigazoom.rc.duke.edu/) for interactive views of full video frames.

**Relevant publications**
- KC Zhou et al., [Parallelized computational 3D video microscopy of freely moving organisms at multiple gigapixels per second](https://www.nature.com/articles/s41566-023-01171-7), *Nature Photonics* (2023)

**Code**  
- [https://github.com/kevinczhou/3D-RAPID](https://github.com/kevinczhou/3D-RAPID)  

## Optical coherence refraction tomography (OCRT)
OCRT is a new computational 3D microscopy technique that incorporates extreme angular diversity to incoherently enhance resolution and reduce speckle of conventional OCT.

<center><img src="/images/OCRT_overview.jpg" alt="OCRT k-space synthesis" width="500"/></center>

OCRT registers multi-angle OCT images or volumes by solving an inverse refraction problem, a process that also computationally reconstructs a 3D refractive index map of the sample. The following videos demonstrate the marked improvement of 3D OCRT over conventional OCT volumetric data (zebrafish larva and mouse esophagus, respectively):

<center>
<video width="500" controls>
  <source src="/images/OCRT_example1.mp4" type="video/mp4">
</video>
<video width="500" controls>
  <source src="/images/OCRT_example2.mp4" type="video/mp4">
</video>
</center>

**Relevant publications**
- KC Zhou et al., [Computational 3D microscopy with optical coherence refraction tomography](https://doi.org/10.1364/OPTICA.454860), *Optica* 9, 593-601 (2022)
- KC Zhou et al., [Unified k-space theory of optical coherence tomography](https://www.osapublishing.org/aop/fulltext.cfm?uri=aop-13-2-462&id=452759), *Advances in Optics and Photonics* 13, 462-514 (2021)
- KC Zhou et al., [Spectroscopic optical coherence refraction tomography](https://www.osapublishing.org/ol/abstract.cfm?uri=ol-45-7-2091), *Optics Letters* 45, 2091-2094 (2020)
- KC Zhou et al., [Optical coherence refraction tomography](https://www.nature.com/articles/s41566-019-0508-1), *Nature Photonics* 13, 794–802 (2019)

**Code**
- [https://github.com/kevinczhou/3d-ocrt](https://github.com/kevinczhou/3d-ocrt)
- [https://github.com/kevinczhou/optical-coherence-refraction-tomography](https://github.com/kevinczhou/optical-coherence-refraction-tomography)


## Multiview imaging over extremely wide angular ranges
We introduce a class of techniques that can achieve multi-view imaging over extremely wide angular ranges (theoretically up to 4pi steradians) based on conic section mirrors (e.g., parabolic or ellipsoidal mirrors). Although traditionally such mirrors are known to exhibit off-axis aberrations and are thus more widely used for on-axis focusing or collimation, we show theoretically and practically that they are particularly well-suited for multi-view 3D imaging applications.

<center><img src="/images/parabolic_mirror.jpg" alt="multiangle imaging with parabolic mirror" width="800"/></center>
The above figure shows multi-view OCT imaging of a fruit fly head from up to ±75&deg;. The fruit fly images are color-coded by view angle, as denoted by the ray traces on the left. These images were used for 3D OCRT reconstructions.


**Relevant publications**
- KC Zhou et al., [Computational 3D microscopy with optical coherence refraction tomography](https://doi.org/10.1364/OPTICA.454860), *Optica* 9, 593-601 (2022)
- KC Zhou et al., [High-speed multi-view imaging approaching 4pi steradians using conic section mirrors: theoretical and practical considerations](https://www.osapublishing.org/josaa/abstract.cfm?uri=josaa-38-12-1810), *JOSA A* 38, 1810-1822 (2021)  

## Diffraction tomography with a deep image prior
Optical diffraction tomography is a coherent 3D imaging modality that reconstructs a 3D refractive index (RI) distribution based on multi-angle diffraction patterns. A well-known problem particularly when using low-NA objectives is the "missing cone" centered about the *k<sub>z</sub>* axis in the Fourier domain, which reduces the axial resolution. At the same time, however, low-NA objectives tend to have higher space-bandwidth products (SBPs), a property exploited in Fourier ptychography for 2D samples. 
<center><img src="/images/teaser.png" alt="deep prior diffraction tomography" width="600"/></center>  
To combat the missing cone problem, we reparameterized the 3D RI distribution as the output of an untrained CNN, and optimized its parameters instead of the 3D volume directly during the 3D reconstruction process. Interestingly, the inherent biases of the CNN structure, even without pretraining, are enough to fill in the missing cone!  



**Relevant publications**  
- KC Zhou & R Horstmeyer, [Diffraction tomography with a deep image prior](https://www.osapublishing.org/oe/abstract.cfm?uri=oe-28-9-12872), *Optics Express* 28, 12872-12896 (2020)  

**Code**  
- [https://github.com/kevinczhou/deep-prior-diffraction-tomography](https://github.com/kevinczhou/deep-prior-diffraction-tomography)
