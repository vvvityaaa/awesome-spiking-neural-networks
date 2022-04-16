# Awesome Spiking Neural Networks 
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![MIT License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

A curated list of materials for *Spiking Neural Networks*, 3rd generation of artificial neural networks.


![SNN Image](https://blogs.kcl.ac.uk/kclip/files/2019/08/prob_snn_KCLIP_0.jpg)

Fig 1. Left - standard ANN network. Right - Spiking neural network, taking spikes as an input and returning sequence of spikes [[1]](https://blogs.kcl.ac.uk/kclip/2019/08/16/compute-with-time-not-over-it-an-introduction-to-spiking-neural-networks/)

## Contents

- [Books](#books)
- [Papers](#papers)
- [Frameworks](#frameworks)
- [Repositories](#repositories)
- [Others](#others)

## Books :closed_book:
1. [Neuronal Dynamics](https://neuronaldynamics.epfl.ch/) - introduction to theoretical and computational neuroscience.
2. [Neuronal Dynamics - Lectures](https://www.youtube.com/channel/UClmOXGbekg0comtuh0d8Oaw/playlists) - youtube playlists of lectures, based on the book "Neuronal Dynamics".
3. [Dynamical Systems in Neuroscience](https://www.izhikevich.org/publications/dsn.pdf) - theoretical neuroscience with exercises and solutions.

## Papers :page_with_curl:
### Fundamental and overview papers
1. [Networks of Spiking Neurons: The Third Generation of Neural Network Models](https://igi-web.tugraz.at/PDF/85a.pdf), Maass W (1996) - pioneering work on spiking neural networks.
2. [On the computational power of circuits of spiking neurons](https://igi-web.tugraz.at/PDF/135.pdf), Maass W and Markram H (2004) - theoretical work, proving theorems about computational complexities of spiking networks.
3. [Deep Learning With Spiking Neurons: Opportunities and Challenges](https://www.frontiersin.org/articles/10.3389/fnins.2018.00774/full), Pfeiffer M and Pfeil T (2018) - overview paper of deep learning on neuromorphic hardware using biologically plausible spiking neurons.
4. [Deep learning in spiking neural networks](https://arxiv.org/pdf/1804.08150.pdf), Tavanaei et al. (2018) - overview paper of advancements in deep learning for spiking neural networks.
5. [Spiking Neural Networks and Online Learning: An Overview and Perspectives](https://arxiv.org/pdf/1908.08019.pdf), Lobo et al. (2019) - overview paper of application of spiking neural networks in the online learning domain.

### Applied papers
1. [STDP-based spiking deep convolutional neural networks for object recognition](https://arxiv.org/pdf/1611.01421.pdf), Kheradpisheh et al. (2017) - first paper proposing convolutional SNN architecture.
2. [A Brain-Inspired Decision-Making Spiking Neural Network and Its Application in Unmanned Aerial Vehicle](https://www.frontiersin.org/articles/10.3389/fnbot.2018.00056/full), Zhao et al. (2018) - using spiking neural networks for decision making for intelligent agents.
3. [Spiking Neural Networks applied to the classification of motor tasks in EEG signals](https://www.sciencedirect.com/science/article/abs/pii/S0893608019303193), Virgilio G. et al. (2020) - using spiking networks for recognition of motor imagery tasks from EEG signals.
4. [Combining SNN and ANN for enhanced image classification](https://arxiv.org/pdf/2102.10592.pdf), Muramatsu N and Yu HT(2021) - combining SNN and ANN to get a hybrid model with improved performance for image classification.
5. [One-shot learning with spiking neural networks](https://www.biorxiv.org/content/10.1101/2020.06.17.156513v1), Scherr et al. (2020) - investigation of one-shot learning paradigm in spiking neural networks using local synaptic plasticity in RSNNs.
6. [Visual Explanations from Spiking Neural Networks using Interspike Intervals](https://arxiv.org/abs/2103.14441), Kim Y and Panda P (2021) - building biologically plausible Spike Activation Maps (SAM) for spike visualization.

### ANN to SNN Conversion
1. [Fast-classifying, high-accuracy spiking deep networks through weight and threshold balancing](https://ieeexplore.ieee.org/document/7280696), Diehl et al. (2015) - defines algorithms for weight normalization for ann to snn conversion.
2. [Theory and Tools for the Conversion of Analog to Spiking Convolutional Neural Networks](https://arxiv.org/pdf/1612.04052.pdf), Ruckauer et al. (2016) - defines robust weight normalization and tools for converting different layers, like BatchNormalization, Maxpooling etc.
3. [Conversion  of  continuous-valued  deep  networks  to  efficientevent-driven  networks  for  image  classification](https://www.frontiersin.org/articles/10.3389/fnins.2017.00682/full), Rueckauer et al (2017) - spiking max-pooling and batch normalization.
4. [Enabling deep spiking neural networks with hybrid conversion and spike timing dependent backpropagation](https://arxiv.org/pdf/2005.01807.pdf), Rathi et al. (2020) - hybrid ann to snn conversion.
5. [Spiking-YOLO: Spiking Neural Network for Energy-Efficient Object Detection](https://arxiv.org/pdf/1903.06530.pdf), Kim et al. (2019) - converting famous yolo architecture to the spiking version.
6. [Spiking Deep Residual Network](https://arxiv.org/pdf/1805.01352.pdf), Hu et al. (2018) - converting ResNet to a spiking version.
7. [Optimal conversion of conventional artificial neural networks to spiking neural networks](https://openreview.net/pdf?id=FZ1oTwcXchK), Deng S and Gu S (2021) - more efficient approximation of loss function between ann and snn with weight transfer pipeline that combines threshold balance and soft-reset mechanisms.

### Learning methods for SNNs
1. [Spike timing dependent plasticity: a consequence of more fundamental learning rules](https://www.frontiersin.org/articles/10.3389/fncom.2010.00019/full), Shouval et al. (2010) - derivation of biological origin and plausibility of STDP.
2. [A History of Spike-Timing-Dependent Plasticity](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3187646/), Markram et al. (2011) - origins and history of STDP learning method.
3. [Training Deep Spiking Neural Networks Using Backpropagation](https://www.frontiersin.org/articles/10.3389/fnins.2016.00508/full), Lee et al. (2016) - treatment of membrane potentials as continuous signals and considering discontinuities as noise in backpropagation for SNN.
4. [Event-driven random backpropagation: Enabling neuromorphic deep learning machines](https://www.frontiersin.org/articles/10.3389/fnins.2017.00324/full), Neftci et al. (2017) - random backpropagation as solution for problem of discrete backpropagation on spikes.
5. [Surrogate gradient learning in spiking neural networks](https://arxiv.org/pdf/1901.09948.pdf), Neftci et al. (2019) - surrogate method, which enables discrete backpropagation learning.
6. [S4NN: temporal backpropagation for spiking neural networkswith one spike per neuron](https://arxiv.org/pdf/1910.09495.pdf), Kheradpisheh SR and Masquelier T (2020) - backpropagation learning method, based on rank-order temporal coding.
7. [Biologically inspired alternatives to backpropagation throughtime for learning in recurrent neural nets](https://arxiv.org/pdf/1901.09049.pdf), Bellec et al. (2019) - biologically plausible approximation of backpropagation through time.

### Neuron models
1. [A logical calculus of the ideas immanent in nervous activity](http://www.cse.chalmers.se/~coquand/AUTOMATA/mcp.pdf), McCulloch W and Pitts W (1943) - one of the first neuron models for computation, based on "all-or-none"-property of biological neurons.
2. [A quantitative description of membrane current and its application to conduction and excitation in nerve](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1392413/), Hodgkin A and Huxley A (1952) - introduction of Hodgkin-Huxley neuron model.
4. [Simple Model of Spiking Neurons](https://www.izhikevich.org/publications/spikes.pdf), Izhikevich E (2003) - introduces the mathematical model of a new type of neurons, so called, Izhikevich neurons.
5. [Resonate-and-fire neurons](https://www.izhikevich.org/publications/resfire.pdf), Izhikevich E (2001) - resonate-and-fire model with complex state variable.
6. [Which Model to Use for Cortical Spiking Neurons?](https://www.izhikevich.org/publications/whichmod.pdf), Izhikevich E (2004) - overview of computational efficiency and biological plausibility of different neuron models.
7. [Spike-frequency adaptation of a generalized leaky integrate-and-fire model neuron](https://www.cns.nyu.edu/wanglab/publications/pdf/liu2001.pdf), Liu YH and Wang XJ (2001) - paper on leaky integrate-and-fire neuron model.

### Neuromorphic hardware
1. [A Survey of Neuromorphic Computing and Neural Networks in Hardware](https://arxiv.org/pdf/1705.06963.pdf), Schuman et al. (2017) - broad discussion on major research topics on neuromorphic hardware.
2. [Towards spike-based machine intelligence with neuromorphic computing](https://www.nature.com/articles/s41586-019-1677-2) - Roy et al. (2019) - overview of the main research direction in neuromorphic hardware and discussion of open questions and challenges in neuromorphic computing.
3. [Neuromorphic silicon neuron circuits](https://www.frontiersin.org/articles/10.3389/fnins.2011.00073/full) - Indiveri et al. (2013) - overview of building blocks for neuromorphic circuits.
4. [Thermal-Aware Compilation of Spiking Neural Networks to Neuromorphic Hardware](https://arxiv.org/abs/2010.04773) - Titirsha T and Das A (2020) - novel technique for mapping of SNNs to neuromorphic hardware using a thermal model.

## Frameworks :computer:
1. [BindsNET](https://github.com/BindsNET/bindsnet) - Python framework for simulation of spiking neural networks using Pytorch.
2. [NEST](https://www.nest-simulator.org/) - spiking neural network simulator with focus on dynamics, size and structure of neural systems. Can be complemented by PyNN.
3. [PySNN](https://github.com/BasBuller/PySNN/tree/master/examples) - framework for spiking neural netorks built on top of Pytorch.
4. [PyNN](https://neuralensemble.org/PyNN/) - library for defining neural models independent of simulator specifics.
5. [NengoDL](https://www.nengo.ai/) - library for building, testing and deploying neural networks, especially spiking neural networks.
6. [Brian2](https://github.com/brian-team/brian2) - python simulator for spiking neural networks.
7. [Norse](https://github.com/electronicvisions/norse) - framework for spiking neural networks, which expands PyTorch with SNN primitives.

## Repositories :open_file_folder:
1. [snn-toolbox](https://github.com/NeuromorphicProcessorProject/snn_toolbox) - toolbox for conversion of ANNs into SNNs using weight normalization.
2. [BrainPy](https://github.com/PKU-NIP-Lab/BrainPy) - simulation toolbox for computational neuroscience research.
3. [spikeflow](https://github.com/colinator/spikeflow) - library for spiking neural networks on top of Tensorflow.
4. [hybrid-snn-conversion](https://github.com/nitin-rathi/hybrid-snn-conversion) - hybrid ann to snn conversion with spike-based backpropagation.
5. [SpikingJelly](https://github.com/fangwei123456/spikingjelly) - new simple SNN framework in Pytorch with easy SNN initialization and ANN2SNN conversion.

## Others :memo:
1. [Human Brain Project](https://www.humanbrainproject.eu/en/) - european project for research in neuroscience, computing and brain-related medicine.
2. [Spiking Neuron Simulation](https://github.com/kaizouman/tensorsandbox/blob/master/snn/simple_spiking_model.ipynb) - tutorial on a simple spiking neuron simulation using Tensorflow.
3. [LIF Simulation](https://github.com/kaizouman/tensorsandbox/blob/master/snn/leaky_integrate_fire.ipynb) - tutorial on the leaky-integrate-and-fire simulation using Tensorflow.
4. [McCulloch & Pitts Neural Net Simulator](https://justinmeiners.github.io/neural-nets-sim/) - visualized web simulator for McCulloch & Pitts NN model.
