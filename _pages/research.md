---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

A major theme of my research is high-throughput computational 3D imaging techniques. Some projects include:
- [Computational 3D imaging with camera arrays](#computational-3d-imaging-with-camera-arrays)
- [Multiview imaging over extremely wide angular ranges](#multiview-imaging-over-extremely-wide-angular-ranges)
- [Optical coherence refraction tomography (OCRT)](#optical-coherence-refraction-tomography-ocrt)

## Computational 3D imaging with camera arrays
Coming soon!

## Multiview imaging over extremely wide angular ranges
We developed a class of techniques that can achieve multi-view imaging over extremely wide angular ranges (theoretically up to 4pi steradians) based on conic section mirrors (e.g., parabolic or ellipsoidal mirrors). Although traditionally such mirrors are known to exhibit off-axis aberrations and are thus more widely used for on-axis focusing or collimation, we show theoretically and practically that they are particularly well-suited for multi-view 3D imaging applications.

<center><img src="/images/parabolic_mirror.jpg" alt="multiangle imaging with parabolic mirror" width="800"/></center>
The above figure shows multi-view OCT imaging of a fruit fly head from up to ±75&deg;. The fruit fly images are color-coded by view angle, as denoted by the ray traces on the left. These images were used for 3D OCRT reconstructions (see below).


**Relevant publications**
- KC Zhou et al., [Computational 3D microscopy with optical coherence refraction tomography](https://doi.org/10.1364/OPTICA.454860), *Optica* 9, 593-601 (2022)
- KC Zhou et al., [High-speed multi-view imaging approaching 4pi steradians using conic section mirrors: theoretical and practical considerations](https://www.osapublishing.org/josaa/abstract.cfm?uri=josaa-38-12-1810), *JOSA A* 38, 1810-1822 (2021)  


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



