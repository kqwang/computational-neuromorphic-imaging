[//]: # (Created by Kaiqiang Wang)

<a name="toc"></a>

# Resources for Computational Neuromorphic Imaging

Computational neuromorphic imaging (CNI) uses neuromorphic event cameras and related event-driven sensing hardware as optical measurement tools for quantitative physical inversion. Unlike generic event-based computer vision, which usually targets semantic tasks such as tracking, recognition, or SLAM, CNI focuses on recovering optical and physical quantities such as focus position, quantum resonance, molecular location, 3D structure, wavefront, phase, depth, flow, and surface profile from sparse asynchronous events.

Quick search by "Ctrl + F" with the following keywords:

*event camera, neuromorphic camera, computational imaging, optical inverse problem, event-based microscopy, event-based holography, wavefront sensing, quantum sensing, light-field microscopy, single-molecule localization microscopy*

****

## Table of contents:

- [Contributing](#contributing)
- [People and groups](#groups)
- [Companies, platforms, and sensors](#companies)
- [Workshops, courses, and tutorials](#workshops)
- [Software and tools](#software)
- [Research papers](#papers)
  - [Foundations and sensor models](#foundations-papers)
  - [Computational neuromorphic imaging paradigm](#paradigm-papers)
  - [Physical models and inverse problems](#inverse-papers)
  - [Event-count-based imaging](#count-papers)
    - [Autofocus](#count-autofocus-papers)
    - [Quantum sensing](#count-quantum-papers)
    - [Noise-enabled imaging](#count-noise-papers)
  - [Event-accumulation-based imaging](#accumulation-papers)
    - [Laser speckle analysis](#accumulation-speckle-papers)
    - [Single-molecule localization microscopy](#accumulation-smlm-papers)
    - [Light-field microscopy](#accumulation-lfm-papers)
    - [Structured light and surface metrology](#accumulation-surface-papers)
    - [Flow, Schlieren, and velocimetry](#accumulation-flow-papers)
    - [Neuromorphic holography](#accumulation-holography-papers)
  - [Raw-event and direct-event imaging](#raw-event-papers)
    - [White-light interferometry](#raw-wli-papers)
    - [Wavefront sensing](#raw-wavefront-papers)
    - [Polarization, spectral, and photometric imaging](#raw-spectral-papers)
    - [Surface profile and defect inspection](#raw-surface-papers)
    - [Higher-dimensional event imaging](#raw-highdim-papers)
  - [Hardware, multimodal sensing, and future directions](#future-papers)
- [Review / Tutorial papers](#review)
- [Books](#books)
- [Dissertations and thesis](#thesis)

****

<a name="contributing"></a>

# Contributing

***You are welcome to join as a contributor*** by adding or modifying relevant content via fork and pull request.

Please use the following guidelines:

- Edit the raw file with [Markdown Syntax](https://www.markdownguide.org/basic-syntax/).
- Avoid typos.
- Do not add what is already listed.
- Keep the format of new additions consistent with the existing entries.
- Note the order of new additions, usually chronological within each technical category.
- Prefer papers, datasets, tutorials, and groups that explicitly connect event-driven sensing to optical imaging, physical measurement, or inverse problems.

[Back to Top](#toc)

****

<a name="groups"></a>

# People and groups

(Initial list; in alphabetical order by group lead or first listed researcher when practical.)

## Asia

- [Edmund Y. Lam / Imaging Systems Laboratory](https://isl.eee.hku.hk/) (The University of Hong Kong). Keywords: computational imaging, neuromorphic imaging, event-based holography, quantum sensing, laser speckle imaging, wavefront sensing.
- [Lei Tian / Computational Imaging Systems Lab](https://www.bu.edu/eng/profile/lei-tian/) (Boston University). Keywords: computational microscopy, light-field microscopy, event-based microscopy.
- [Chetan Singh Thakur](https://eecs.iisc.ac.in/people/chetan-singh-thakur/) (Indian Institute of Science). Keywords: neuromorphic engineering, event-based sensing, neuromorphic localization microscopy.

## Americas

- [Laura Waller / Computational Imaging Lab](https://www.laurawaller.com/) (University of California, Berkeley). Keywords: computational imaging, event-camera image reconstruction, noise-enabled imaging.
- [Davide Scaramuzza / Robotics and Perception Group](https://rpg.ifi.uzh.ch/) (University of Zurich). Keywords: event-based vision, event-based reconstruction, event representations.
- [Adrian Stern](https://in.bgu.ac.il/en/engn/electrop/Pages/ResearchersAndResearchAreas.aspx) (Ben-Gurion University of the Negev). Keywords: 4D event imaging, computational optics, holography.

## Europe

- [Guillermo Gallego](https://sites.google.com/view/guillermogallego/research/event-based-vision?authuser=0) (Technische Universitat Berlin). Keywords: event-based vision, event representations, contrast maximization, structured light.
- [Suliana Manley / Laboratory of Experimental Biophysics](https://www.epfl.ch/labs/leb/) (EPFL). Keywords: microscopy, event-driven acquisition, single-molecule localization microscopy.

[Back to Top](#toc)

****

<a name="companies"></a>

# Companies, platforms, and sensors

Product availability and sensor generations change quickly; links should be verified before purchase or citation.

## Companies working on event-based vision

- [iniVation AG](https://inivation.com/): commercial event-based neuromorphic vision company spun out of the Institute of Neuroinformatics ecosystem.
- [iniLabs AG](https://inilabs.com/): neuromorphic technologies and research-oriented hardware/software support.
- [Prophesee](https://www.prophesee.ai/): event-based vision sensor and software company.
- [Sony Semiconductor Solutions](https://www.sony-semicon.com/en/products/is/industry/evs.html): image-sensor manufacturer developing event-based vision sensors with Prophesee.
- [Samsung](https://www.samsung.com/): developer of dynamic vision sensor prototypes and event-based vision technologies reported in the literature.
- [Insightness AG](http://www.insightness.com/): developer of Silicon Eye event-sensor technology; status and product availability should be verified.
- [CelePixel](https://www.celepixel.com/): developer of CeleX dynamic vision sensor platforms; status and product availability should be verified.
- [AIT Austrian Institute of Technology](https://www.ait.ac.at/en/research-fields/new-sensor-technologies/): optical sensor systems and industrial neuromorphic sensing applications.

[Back to Top](#toc)

****

<a name="workshops"></a>

# Workshops, courses, and tutorials

- [Optica Imaging Congress](https://www.optica.org/events/congress/imaging_and_applied_optics_congress/): includes topical meetings such as [Computational Optical Sensing and Imaging (COSI)](https://www.optica.org/events/congress/imaging_and_applied_optics_congress/program/computational_optical_sensing_and_imaging), Digital Holography and Three-Dimensional Imaging (DH), 3D Imaging, Imaging Systems, and related applied-optics programs.
- [CVPR Workshop on Event-based Vision](https://tub-rip.github.io/eventvision2025/): useful background for event-camera models, representations, algorithms, datasets, and challenges.
- [NEVI Workshop on Neuromorphic Event-Based Vision at ECCV 2024](https://research.universityofgalway.ie/en/activities/nevi-workshop-on-neuromorphic-event-based-vision-eccv-2024): related workshop on neuromorphic event-based vision, sensing, hardware, and bio-inspired AI.
- [OSA / Optica Imaging and Applied Optics Congress archive](https://optica-org-web-afd-f9abf4byhbacgfgk.z02.azurefd.net/optica/media/osa.media/meetings/archives/2018/2018_imaging_program.pdf?t=636663965651293431): historical source for COSI, DH, 3D imaging, wavefront sensing, spectral imaging, high-speed imaging, and computational microscopy sessions.
- [Event Vision School](https://edpr.iit.it/events/2026-evs): recurring educational content on event cameras and event-based vision.
- [Event-based Robot Vision at TU Berlin](https://sites.google.com/view/guillermogallego/teaching/event-based-robot-vision): course material by Guillermo Gallego.

[Back to Top](#toc)

****

<a name="software"></a>

# Software and tools

This section lists general-purpose event-camera tools that can support CNI experiments. Domain-specific code is linked next to the corresponding paper when available.

- [OpenEB](https://github.com/prophesee-ai/openeb): open-source event-based vision software from Prophesee.
- [jAER](http://jaerproject.org/): Java Address-Event Representation project for event processing.
- [AEDAT Tools](https://github.com/simbamford/AedatTools/): MATLAB and Python tools for working with AEDAT files.
- [Loris](https://github.com/neuromorphic-paris/loris): Python package for reading neuromorphic camera files.
- [Tonic](https://github.com/neuromorphs/tonic): event dataset and transformation library.
- [AEStream](https://github.com/norse/aestream/): streaming tools for address-event representations from iniVation and Prophesee cameras.

[Back to Top](#toc)

****

<a name="papers"></a>

# Research papers

<a name="foundations-papers"></a>

## Foundations and sensor models

- P. Lichtsteiner, C. Posch, and T. Delbruck, [A 128 x 128 120 dB 15 microsecond latency asynchronous temporal contrast vision sensor](https://doi.org/10.1109/JSSC.2007.914337), IEEE Journal of Solid-State Circuits, 2008.
- C. Posch, D. Matolin, and R. Wohlgenannt, [A QVGA 143 dB dynamic range frame-free PWM image sensor with lossless pixel-level video compression and time-domain CDS](https://doi.org/10.1109/JSSC.2010.2085952), IEEE Journal of Solid-State Circuits, 2011.
- C. Brandli et al., [A 240 x 180 130 dB 3 microsecond latency global shutter spatiotemporal vision sensor](https://doi.org/10.1109/JSSC.2014.2342715), IEEE Journal of Solid-State Circuits, 2014.
- X. Lagorce et al., [HOTS: A hierarchy of event-based time-surfaces for pattern recognition](https://doi.org/10.1109/TPAMI.2016.2574707), IEEE Transactions on Pattern Analysis and Machine Intelligence, 2017.
- S. Chen and M. Guo, [Live demonstration: CeleX-V: A 1M pixel multi-mode event-based sensor](https://doi.org/10.1109/CVPRW.2019.00214), CVPR Workshops, 2019.
- T. Huang et al., [1000x faster camera and machine vision with ordinary devices](https://doi.org/10.1016/j.eng.2022.01.012), Engineering, 2023.

[Back to Top](#toc)

<a name="paradigm-papers"></a>

## Computational neuromorphic imaging paradigm

This category is reserved for papers that explicitly define, name, or consolidate CNI as an optical physical-inversion paradigm.

[Back to Top](#toc)

<a name="inverse-papers"></a>

## Physical models and inverse problems

- A. Z. Zhu et al., [Unsupervised event-based learning of optical flow, depth, and egomotion](https://doi.org/10.1109/CVPR.2019.00108), CVPR, 2019.
- C. Scheerlinck et al., [Fast image reconstruction with an event camera](https://doi.org/10.1109/WACV45572.2020.9093366), WACV, 2020.
- H. Rebecq et al., [High speed and high dynamic range video with an event camera](https://doi.org/10.1109/TPAMI.2019.2963386), IEEE Transactions on Pattern Analysis and Machine Intelligence, 2021.
- P. Zhang et al., [Neuromorphic imaging with super-resolution](https://doi.org/10.1109/TCSVT.2024.3482436), IEEE Transactions on Circuits and Systems for Video Technology, 2024.
- P. Zhang, C. Wang, and E. Y. Lam, [Neuromorphic imaging and classification with graph learning](https://doi.org/10.1016/j.neucom.2023.127010), Neurocomputing, 2024.

[Back to Top](#toc)

<a name="count-papers"></a>

## Event-count-based imaging

<a name="count-autofocus-papers"></a>

### Autofocus

- S. Lin et al., [Autofocus for event cameras](https://doi.org/10.1109/CVPR52688.2022.01586), CVPR, 2022.
- Z. Ge et al., [Millisecond autofocusing microscopy using neuromorphic event sensing](https://doi.org/10.1016/j.optlaseng.2022.107247), Optics and Lasers in Engineering, 2023.
- H. Lou, M. Teng, Y. Yang, and B. Shi, [All-in-focus imaging from event focal stack](https://openaccess.thecvf.com/content/CVPR2023/html/Lou_All-in-Focus_Imaging_From_Event_Focal_Stack_CVPR_2023_paper.html), CVPR, 2023.
- Y. Bao et al., [Improving fast auto-focus with event polarity](https://doi.org/10.1364/OE.489717), Optics Express, 2023.
- X. Qu et al., [A robust autofocusing method for microscopic imaging based on an event camera](https://doi.org/10.1016/j.optlaseng.2024.108025), Optics and Lasers in Engineering, 2024.

<a name="count-quantum-papers"></a>

### Quantum sensing

- Z. Du et al., [Widefield diamond quantum sensing with neuromorphic vision sensors](https://doi.org/10.1002/advs.202304355), Advanced Science, 2024.
- C. Wang et al., [Intelligent quantum sensing with computational neuromorphic imaging](https://opg.optica.org/abstract.cfm?URI=COSI-2024-CM2B.1), Optica Imaging Congress, 2024.

<a name="count-noise-papers"></a>

### Noise-enabled imaging

- S. Zhu et al., [Harnessing noise for materials differentiation in computational neuromorphic imaging](https://doi.org/10.1109/OGC62429.2024.10738780), Optoelectronics Global Conference, 2024.
- R. Cao et al., [Noise2Image: noise-enabled static scene recovery for event cameras](https://doi.org/10.1364/OPTICA.538916), Optica, 2025.

[Back to Top](#toc)

<a name="accumulation-papers"></a>

## Event-accumulation-based imaging

<a name="accumulation-speckle-papers"></a>

### Laser speckle analysis

- Z. Ge, T. Zeng, and E. Y. Lam, [Lensless sensing using the event sensor](https://doi.org/10.1364/ISA.2021.ITu6B.5), OSA Imaging and Applied Optics Congress, 2021.
- Z. Ge et al., [Dynamic laser speckle analysis using the event sensor](https://doi.org/10.1364/AO.412601), Applied Optics, 2021.
- Z. Ge et al., [Event-based laser speckle correlation for micro motion estimation](https://doi.org/10.1364/OL.430419), Optics Letters, 2021.
- Z. Ge et al., [Lens-free motion analysis via neuromorphic laser speckle imaging](https://doi.org/10.1364/OE.444948), Optics Express, 2022.
- S. Zhu et al., [Efficient non-line-of-sight tracking with computational neuromorphic imaging](https://doi.org/10.1364/OL.530066), Optics Letters, 2024.
- Y. Cao, S. Zhu, and E. Y. Lam, [Neuromorphic dynamic speckle pattern synthesis for imaging through scattering media](https://doi.org/10.1117/12.3073637), Advanced Optical Imaging Technologies VIII, 2025.

<a name="accumulation-smlm-papers"></a>

### Single-molecule localization microscopy

- D. Mahecic et al., [Event-driven acquisition for content-enriched microscopy](https://doi.org/10.1038/s41592-022-01589-x), Nature Methods, 2022.
- R. Mangalwedhekar et al., [Achieving nanoscale precision using neuromorphic localization microscopy](https://doi.org/10.1038/s41565-022-01291-1), Nature Nanotechnology, 2023.
- C. Cabriel et al., [Event-based vision sensor for fast and dense single-molecule localization microscopy](https://doi.org/10.1038/s41566-023-01308-8), Nature Photonics, 2023.
- J. Basumatary et al., [Event-based single molecule localization microscopy for high spatio-temporal super-resolution imaging](https://doi.org/10.1101/2023.12.30.573392), bioRxiv, 2024.

<a name="accumulation-lfm-papers"></a>

### Light-field microscopy

- R. Guo et al., [EventLFM: Event camera integrated Fourier light field microscopy for ultrafast 3D imaging](https://doi.org/10.1038/s41377-024-01502-5), Light: Science and Applications, 2024.

<a name="accumulation-surface-papers"></a>

### Structured light and surface metrology

- C. Brandli et al., [Adaptive pulsed laser line extraction for terrain reconstruction using a dynamic vision sensor](https://doi.org/10.3389/fnins.2013.00275), Frontiers in Neuroscience, 2014.
- N. Matsuda, O. Cossairt, and M. Gupta, [MC3D: Motion contrast 3D scanning](https://doi.org/10.1109/ICCPHOT.2015.7168370), ICCP, 2015. [Project](http://compphotolab.northwestern.edu/project/mc3d-motion-contrast-3d-laser-scanner/)
- A. R. Mangalore, C. S. Seelamantula, and C. S. Thakur, [Neuromorphic fringe projection profilometry](https://doi.org/10.1109/LSP.2020.3016251), IEEE Signal Processing Letters, 2020. [Code](https://github.com/ashishrao7/NFPP)
- X. Huang, Y. Zhang, and Z. Xiong, [High-speed structured light based 3D scanning using an event camera](https://doi.org/10.1364/OE.437944), Optics Express, 2021.
- M. Muglikar, G. Gallego, and D. Scaramuzza, [ESL: Event-based structured light](https://doi.org/10.1109/3DV53792.2021.00124), 3DV, 2021. [Project and dataset](http://rpg.ifi.uzh.ch/esl.html), [Code](https://github.com/uzh-rpg/ESL)
- M. Muglikar, D. P. Moeys, and D. Scaramuzza, [Event guided depth sensing](https://doi.org/10.1109/3DV53792.2021.00048), 3DV, 2021.
- H. Wang et al., [Enhancing event-based structured light imaging with a single frame](https://doi.org/10.1109/MFI55806.2022.9913845), MFI, 2022.
- Y. Li et al., [Robust 3D measurement based on neuromorphic event-driven Fourier transform profilometry](https://doi.org/10.2139/ssrn.4204360), SSRN Electronic Journal, 2022.
- W. Morgenstern et al., [X-maps: Direct depth lookup for event-based structured light systems](https://openaccess.thecvf.com/content/CVPR2023W/EventVision/papers/Morgenstern_X-Maps_Direct_Depth_Lookup_for_Event-Based_Structured_Light_Systems_CVPRW_2023_paper.pdf), CVPR Workshops, 2023. [Project and code](https://fraunhoferhhi.github.io/X-maps/)

<a name="accumulation-flow-papers"></a>

### Flow, Schlieren, and velocimetry

- S. Shiba, F. Hamann, Y. Aoki, and G. Gallego, [Event-based background-oriented Schlieren](https://doi.org/10.1109/TPAMI.2023.3328188), IEEE Transactions on Pattern Analysis and Machine Intelligence, 2023. [Project and code](https://github.com/tub-rip/event_based_bos)
- L. Maya et al., [An evaluation of event-based cameras for particle image velocimetry](https://doi.org/10.1007/s00348-025-04127-5), Experiments in Fluids, 2025.

<a name="accumulation-holography-papers"></a>

### Neuromorphic holography

- Z. Ge et al., [Event-driven neuromorphic holography for dynamic particle imaging](https://doi.org/10.1364/OL.548088), Optics Letters, 2025.
- C. Wang et al., Motion-resolved event-based holography, Advanced Optical Imaging Technologies VIII, 2025.
- C. Wang et al., [Differentiable event-based holography](https://doi.org/10.1364/DH.2025.DTu2C.3), Optica Imaging Congress, 2025.
- I. Uchiyama et al., [Events meet phase-shifting digital holography: practical acquisition, theory, and algorithms](https://doi.org/10.1364/OE.584341), Optics Express, 2026.

[Back to Top](#toc)

<a name="raw-event-papers"></a>

## Raw-event and direct-event imaging

<a name="raw-wli-papers"></a>

### White-light interferometry

- C. Schober et al., [Event based coherence scanning interferometry](https://doi.org/10.1364/OL.437489), Optics Letters, 2021.

<a name="raw-wavefront-papers"></a>

### Wavefront sensing

- F. Kong et al., [Shack-Hartmann wavefront sensing using spatial-temporal data from an event-based image sensor](https://doi.org/10.1364/OE.409682), Optics Express, 2020.
- C. Wang et al., [Tracking the Shack-Hartmann spots using neuromorphic motion compensation](https://doi.org/10.1364/COSI.2023.CTu2B.5), Optica Imaging Congress, 2023.
- M. Grose, J. D. Schmidt, and K. Hirakawa, [Convolutional neural network for improved event-based Shack-Hartmann wavefront reconstruction](https://doi.org/10.1364/AO.520652), Applied Optics, 2024.
- C. Wang et al., [Angle-based neuromorphic wave normal sensing](https://doi.org/10.1002/lpor.202400647), Laser and Photonics Reviews, 2025.

<a name="raw-spectral-papers"></a>

### Polarization, spectral, and photometric imaging

- T. Takatani et al., [Event-based bispectral photometry using temporally modulated illumination](https://openaccess.thecvf.com/content/CVPR2021/papers/Takatani_Event-Based_Bispectral_Photometry_Using_Temporally_Modulated_Illumination_CVPR_2021_paper.pdf), CVPR, 2021. [Project](https://cigl.iit.tsukuba.ac.jp/portfolio/event-based-bispectral-photometry)
- H. Mei et al., [Deep polarization reconstruction with PDAVIS events](https://doi.org/10.1109/CVPR52729.2023.02121), CVPR, 2023. [Code](https://github.com/SensorsINI/e2p)
- M. Muglikar, L. Bauersfeld, D. P. Moeys, and D. Scaramuzza, [Event-based shape from polarization](https://openaccess.thecvf.com/content/CVPR2023/html/Muglikar_Event-Based_Shape_From_Polarization_CVPR_2023_paper.html), CVPR, 2023. [Project, code, and dataset](https://rpg.ifi.uzh.ch/esfp.html)

<a name="raw-surface-papers"></a>

### Surface profile and defect inspection

- Mangalore, A.R. et al, [Neuromorphic Fringe Projection Profilometry] (https://doi.org/10.1109/LSP.2020.3016251), IEEE Signal Processing Letters, 2020.
- S. Zhu et al., [Ultrafast dynamic defect inspection with computational neuromorphic imaging](https://doi.org/10.1002/advs.202510338), Advanced Science, 2025.

<a name="raw-highdim-papers"></a>

### Higher-dimensional event imaging

- R. Ilani and A. Stern, [4D event imaging with a single neuromorphic camera](https://doi.org/10.1117/1.APN.5.1.016001), Advanced Photonics Nexus, 2025.
- T. Tsuchida et al., [Coded-E2LF: Coded aperture light field imaging from events](https://doi.org/10.48550/arXiv.2602.22620), arXiv, 2026.
- Q. Zhou et al., [Event2Flow: Scalable imaging of peripheral and cerebral hemodynamics with event-based vision sensors](https://doi.org/10.64898/2026.02.17.706291), bioRxiv, 2026.

[Back to Top](#toc)

<a name="future-papers"></a>

## Hardware, multimodal sensing, and future directions

- S. Afshar et al., [Event-based processing of single photon avalanche diode sensors](https://doi.org/10.1109/JSEN.2020.2979761), IEEE Sensors Journal, 2020.
- M. Jaklin et al., [HDR 4T-APS pixel for event generation by frame differencing](https://doi.org/10.1109/MWSCAS47672.2021.9531723), MWSCAS, 2021.
- D. Yao et al., [Bayesian neuromorphic imaging for single-photon LiDAR](https://doi.org/10.1364/OE.525058), Optics Express, 2024.
- S. Esfahani, M. Cotrufo, and A. Alu, [Tailoring space-time nonlocality for event-based image processing metasurfaces](https://doi.org/10.1103/PhysRevLett.133.063801), Physical Review Letters, 2024.

[Back to Top](#toc)

****

<a name="review"></a>

# Review / Tutorial papers

## Event cameras and neuromorphic vision

- D. Kong and Z. Fang, Review of event-based vision sensors and their applications, Information and Control, 2021.
- G. Gallego et al., [Event-based vision: A survey](https://doi.org/10.1109/TPAMI.2020.3008413), IEEE Transactions on Pattern Analysis and Machine Intelligence, 2022.
- D. Cazzato and F. Bono, [An application-driven survey on event-based neuromorphic computer vision](https://doi.org/10.3390/info15080472), Information, 2024.
- H. AliAkbarpour et al., [Emerging trends and applications of neuromorphic dynamic vision sensors: A survey](https://doi.org/10.1109/SR.2024.3513952), IEEE Sensors Reviews, 2024.
- X. Zheng et al., Deep learning for event-based vision: A comprehensive survey and benchmarks, arXiv:2302.08890v3, 2024.
- B. Chakravarthi et al., [Recent event camera innovations: A survey](https://doi.org/10.1007/978-3-031-92460-6_21), ECCV Workshops, 2025.

## Application-adjacent reviews

- J. Huang et al., [Computational flow visualization to reveal hidden properties of complex flow with optical and computational methods](https://doi.org/10.1016/j.xcrp.2024.102282), Cell Reports Physical Science, 2024.

[Back to Top](#toc)

****

<a name="books"></a>

# Books

No dedicated CNI book is listed yet. Candidates on event-based sensing, neuromorphic engineering, computational imaging, optical inverse problems, or biomedical computational microscopy are welcome.

[Back to Top](#toc)

****

<a name="thesis"></a>

# Dissertations and thesis

- M. Mahowald, VLSI analogs of neuronal visual processing: a synthesis of form and function, Ph.D. thesis, California Institute of Technology, 1992.
- P. Lichtsteiner, [An AER temporal contrast vision sensor](https://www.research-collection.ethz.ch/handle/20.500.11850/149539), doctoral thesis, ETH Zurich, 2006.
- C. P. Brandli, [Event-Based Machine Vision](https://www.research-collection.ethz.ch/bitstreams/15b3c34e-bb2e-4e3f-b804-3353fb835fad/download), doctoral thesis, ETH Zurich, 2015.
- H. Rebecq, [Event Cameras: From SLAM to High Speed Video](https://rpg.ifi.uzh.ch/docs/PhD19_Rebecq.pdf), Ph.D. thesis, University of Zurich, 2019.
- C. Scheerlinck, [How to See with an Event Camera](https://openresearch-repository.anu.edu.au/items/7e2d4237-5e41-4f22-8b7f-171c1b07a4a4), Ph.D. thesis, Australian National University, 2021.
- L. Cordone, [Performance des reseaux de neurones a spikes sur des donnees evenementielles pour des applications automobiles embarquees](https://theses.hal.science/tel-04026653v1), Ph.D. thesis, Universite Cote d'Azur, 2022.
- Z. Ge, [Neuromorphic event sensing for laser speckle imaging and autofocusing microscopy](https://hub.hku.hk/handle/10722/318404), Ph.D. thesis, The University of Hong Kong, 2022.
- R. Cao, [Unknown Motion Calibration and Dynamic Imaging Reconstruction](https://escholarship.org/content/qt2xt6f11b/qt2xt6f11b_noSplash_06a2511dd7ab320755889fd55500602b.pdf), Ph.D. dissertation, University of California, Berkeley and University of California, San Francisco, 2024.
- P. Zhang, [Synergy of dynamic perception and static vision in neuromorphic imaging](https://hub.hku.hk/handle/10722/355614), Ph.D. thesis, The University of Hong Kong, 2024.

[Back to Top](#toc)
