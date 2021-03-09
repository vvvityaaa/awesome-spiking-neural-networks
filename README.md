# Awesome Spiking Neural Networks [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of materials for *Spiking Neural Networks*, 3rd generation of artificial neural networks.

## Contents

[Books](#books)
[Papers](#papers)
[Frameworks](#frameworks)
[Repositories](#repositories)
[Research groups](#research-groups)

## Books
1. [Neuronal Dynamics](https://neuronaldynamics.epfl.ch/) - introduction to theoretical and computational neuroscience.
2. [Neuronal Dynamics - Lectures](https://www.youtube.com/channel/UClmOXGbekg0comtuh0d8Oaw/playlists) - youtube playlists of lectures, based on the book "Neuronal Dynamics".
3. [Dynamical Systems in Neuroscience](https://www.izhikevich.org/publications/dsn.pdf) - theoretical neuroscience with exercises and solutions.

## Papers
### General papers
1. [Networks of Spiking Neurons: The Third Generation of Neural Network Models](https://igi-web.tugraz.at/PDF/85a.pdf), Maass W - pioneering work on spiking neural networks.
2. [On the computational power of circuits of spiking neurons](https://igi-web.tugraz.at/PDF/135.pdf), Maass W and Markram H - theoretical work, proving theorems about computational complexities of spiking networks.
3. [Deep Learning With Spiking Neurons: Opportunities and Challenges](https://www.frontiersin.org/articles/10.3389/fnins.2018.00774/full), Pfeiffer M and Pfeil T - overview paper of deep learning on neuromorphic hardware using biologically plausible spiking neurons.
4. 

### ANN to SNN Conversion
1. [Fast-classifying, high-accuracy spiking deep networks through weight and threshold balancing](https://ieeexplore.ieee.org/document/7280696), Diehl et al (2015) - defines algorithms for weight normalization for ann to snn conversion.
2. [Theory and Tools for the Conversion of Analog to Spiking Convolutional Neural Networks](https://arxiv.org/pdf/1612.04052.pdf), Ruckauer et al (2016) - defines robust weight normalization and tools for converting different layers, like BatchNormalization, Maxpooling etc.
3. [Conversion  of  continuous-valued  deep  networks  to  efficientevent-driven  networks  for  image  classification](https://www.frontiersin.org/articles/10.3389/fnins.2017.00682/full), Rueckauer et al (2017) - spiking max-pooling and batch normalization.
4. [Enabling deep spiking neural networks with hybrid conversion and spike timing dependent backpropagation](https://arxiv.org/pdf/2005.01807.pdf), Rathi et al - hybrid ann to snn conversion.

## Frameworks
1. [BindsNET](https://github.com/BindsNET/bindsnet) - Python framework for simulation of spiking neural networks using Pytorch.
2. [PySNN](https://github.com/BasBuller/PySNN/tree/master/examples) - framework for spiking neural netorks built on top of Pytorch.
3. [PyNN](https://neuralensemble.org/PyNN/) - library for defining neural models independent of simulator specifics.

## Repositories
1. [snn-toolbox](https://github.com/NeuromorphicProcessorProject/snn_toolbox) - toolbox for conversion of ANNs into SNNs using weight normalization.
2. [BrainPy](https://github.com/PKU-NIP-Lab/BrainPy) - simulation toolbox for computational neuroscience research.
3. [spikeflow](https://github.com/colinator/spikeflow) - library for spiking neural networks on top of Tensorflow.
4. [hybrid-snn-conversion](https://github.com/nitin-rathi/hybrid-snn-conversion) - hybrid ann to snn conversion with spike-based backpropagation.

## Research groups and projects
1. [Human Brain Project](https://www.humanbrainproject.eu/en/) - european project for research in neuroscience, computing and brain-related medicine.
2. [Robotics, Artificial Intelligence and Embedding Systems Chair](https://www.in.tum.de/i06/home/) - Technical University of Munich.
3. [Institue of Theoretical Computer Science](https://igi-web.tugraz.at/people/maass/) - Technical University of Graz.
4. [Institute of Neuroinformatics](https://www.ini.uzh.ch/en/institute.html) - University of Zurich.
5. [Chair of highly-parallel VLSI systems and neuromorphic microelectronics](https://tu-dresden.de/ing/elektrotechnik/iee/hpsn) - Technical University of Dresden.
6. [Neuroengineering student's group](https://neuroengineering.blog/) - student's of M.Sc. of Neuroengineering at the Technical University of Munich.
