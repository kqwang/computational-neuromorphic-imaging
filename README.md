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
    - [Neuromorphic holography](#accumulation-holography-papers)
  - [Raw-event and direct-event imaging](#raw-event-papers)
    - [White-light interferometry](#raw-wli-papers)
    - [Wavefront sensing](#raw-wavefront-papers)
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

- Edmund Y. Lam group (The University of Hong Kong). Keywords: computational imaging, neuromorphic imaging, event-based holography, quantum sensing, laser speckle imaging, wavefront sensing.
- Kaiqiang Wang group (Northwestern Polytechnical University). Keywords: computational imaging, optical metrology, neuromorphic imaging.
- Lei Tian group (Boston University). Keywords: computational microscopy, light-field microscopy, event-based microscopy.
- Chetan Singh Thakur group (Indian Institute of Science). Keywords: neuromorphic engineering, event-based sensing, neuromorphic localization microscopy.

## Americas

- Laura Waller group (University of California, Berkeley). Keywords: computational imaging, event-camera image reconstruction, noise-enabled imaging.
- Davide Scaramuzza group (University of Zurich / Robotics and Perception Group). Keywords: event-based vision, event-based reconstruction, event representations.
- Adrian Stern group (Ben-Gurion University of the Negev). Keywords: 4D event imaging, computational optics, holography.

## Europe

- Guillermo Gallego group (Technische Universitat Berlin). Keywords: event-based vision, event representations, contrast maximization, structured light.
- Suliana Manley group (EPFL). Keywords: microscopy, event-driven acquisition, single-molecule localization microscopy.

[Back to Top](#toc)

****

<a name="companies"></a>

# Companies, platforms, and sensors

This section tracks hardware routes that appear in CNI-related literature. Links and product details should be verified before new entries are added.

- DVS / Dynamic Vision Sensor: asynchronous temporal contrast sensing.
- ATIS / Asynchronous Time-based Image Sensor: event-triggered intensity measurement.
- DAVIS / Dynamic and Active-pixel Vision Sensor: hybrid event and active-pixel frame readout.
- CeleX series: multimode event-based vision sensors.
- Vidar series: high-speed event-like sensing from ordinary devices.
- SPAD-based event processing: photon-counting sensors with event-based processing.
- Frame-differencing CMOS sensors: event generation from high-speed frame differences.
- Metasurface event processors: optical-domain spatiotemporal differentiation and event-like processing.

[Back to Top](#toc)

****

<a name="workshops"></a>

# Workshops, courses, and tutorials

- Optica Imaging Congress: COSI, DH, ISA, 3D, and related topical meetings have hosted multiple CNI-related papers.
- CVPR / ICCV / ECCV event-based vision workshops: useful background for event-camera models, representations, and algorithms.
- OSA / Optica Imaging and Applied Optics Congress: historical venue for early event-sensor optical imaging demonstrations.

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

- K. Wang, S. Zhu, C. Wang, P. Zhang, Z. Ge, and E. Y. Lam, Computational Neuromorphic Imaging: From Bio-Inspired Events to Quantitative Optical Inversion, review manuscript in preparation.

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

- A. R. Mangalore, C. S. Seelamantula, and C. S. Thakur, [Neuromorphic fringe projection profilometry](https://doi.org/10.1109/LSP.2020.3016251), IEEE Signal Processing Letters, 2020.
- X. Huang, Y. Zhang, and Z. Xiong, [High-speed structured light based 3D scanning using an event camera](https://doi.org/10.1364/OE.437944), Optics Express, 2021.
- M. Muglikar, G. Gallego, and D. Scaramuzza, [ESL: Event-based structured light](https://doi.org/10.1109/3DV53792.2021.00124), 3DV, 2021.
- H. Wang et al., [Enhancing event-based structured light imaging with a single frame](https://doi.org/10.1109/MFI55806.2022.9913845), MFI, 2022.
- Y. Li et al., [Robust 3D measurement based on neuromorphic event-driven Fourier transform profilometry](https://doi.org/10.2139/ssrn.4204360), SSRN Electronic Journal, 2022.

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

<a name="raw-surface-papers"></a>

### Surface profile and defect inspection

- S. Zhu et al., [Efficient non-line-of-sight tracking with computational neuromorphic imaging](https://doi.org/10.1364/OL.530066), Optics Letters, 2024.
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

## Computational imaging and optical inverse problems

- J. N. Mait, G. W. Euliss, and R. A. Athale, [Computational imaging](https://doi.org/10.1364/AOP.10.000409), Advances in Optics and Photonics, 2018.
- G. Barbastathis, A. Ozcan, and G. Situ, [On the use of deep learning for computational imaging](https://doi.org/10.1364/OPTICA.6.000921), Optica, 2019.
- Z. Huang and L. Cao, [Quantitative phase imaging based on holography: trends and new perspectives](https://doi.org/10.1038/s41377-024-01453-x), Light: Science and Applications, 2024.
- X. Luo et al., [Revolutionizing optical imaging: computational imaging via deep learning](https://doi.org/10.3788/PI.2025.R03), Photonics Insights, 2025.
- F. Wang, J. W. Czarske, and G. Situ, [Deep learning for computational imaging: from data-driven to physics-enhanced approaches](https://doi.org/10.1117/1.AP.7.5.054002), Advanced Photonics, 2025.

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

[Back to Top](#toc)
