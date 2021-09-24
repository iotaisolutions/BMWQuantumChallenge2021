# Quantum computing: BMW Group “Quantum Computing Challenge” in collaboration with AWS to crowd-source innovation.
BMW Quantum Computing Challenge 2021 Repository


# Quantum Defect Analyser 
## Quantum Neural Network Solution for Automated Quality Asessment (processing images from **Surface Crack Detection** dataset)
[**BMW Quantum Challenge 2021**](https://www.press.bmwgroup.com/global/article/detail/T0337884EN/quantum-computing:-bmw-group-launches-%E2%80%9Cquantum-computing-challenge%E2%80%9D-in-collaboration-with-aws-to-crowd-source-innovation?language=enr)

**Members**: <!-- up to 6 members per term -->
- **Anuj Mehrotra**, @iotaisolutions, IOTAONEIQ Solutions Pvt. Ltd. (India) | IBM Qiskit Advocate
- **Vardaan Sahgal**, @Varary73, Netaji Subhas University of Technology (India), M.Sc. Physics
- **Meghashrita Das**, @Meghashrita Das, Indian Institute of Technology Kharagpur (India), B.Tech in Agricultural and Food engineering and M.Tech spl in Financial engineering
- **Amaury de Miguel**, @AmauryDM, ISEP Engineering School (France), Data Analysis and Machine Learning | Sorbonne Université Pierre et Marie Curie, M.Sc. Physics | IBM Qiskit Advocate

**Quantum neural networks** are computational neural network models which are based on the principles of quantum mechanics and acts application-agnostic computational units that can be used for many different use cases : like Image Processing , Natural Language Processing, computer games, function approximation, handling big data, in modelling social networks, associative memory devices, and automated control systems etc.

In **Quantum Machine Learning (QML)**, Quantum kernels is the approach of exploiting group structure in data which helps to achieve quantum speedup ( but not mandatory). Quantum kernels can be optimized with a technique called kernel alignment.

Different quantum computing methods are used to encode classical data in a quantum-enhanced feature space. For computing quantum kernels, an algorithm called  Quantum kernel estimator (QKE) is  used which leverages quantum circuits for classical data and provides an efficient way to evaluate inner products between data in a quantum feature space.

Quantum Neural Networks (QNN) are parameterized quantum circuits which acts like linear methods in quantum feature space  and suitable case for using quantum kernels and in turn can be optimized using **Quantum Kernel Alignment (QKA)**. 

QKA is an iterative quantum-classical algorithm, in which quantum hardware is used to execute parametrized quantum circuits  for evaluating the quantum kernel matrices with QKE, while a classical optimizer tunes the parameters of those circuits to maximize the alignment. Iterative algorithms of this type can be slow due to latency between the quantum and classical calculations. 


In this project, in order to showcase an application of **Quantum Kernel Alignment ** , QKA was used foroptimizing Quantum Neural Network, which processes images from **Surface Crack Detection** dataset (**Kaggle.com**) and can be scaled up & used as a module in **Automated Quality Management** in assembly line of Manufacturing Factory units (like of Automobile).

  
# Technology stack
Below table covers Technology Stack for implementing this project:

Programming Language| Classical (Deep) ML Framework| Quantum Compluting Development Platform | Simulator | Additional Module| Coding Collaboration Environment 
------------ | -------------| -------------| -------------| -------------|-------------
  ![Python](https://img.shields.io/badge/python%203.x%20>=%203.7-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  |  ![PyTorch](https://img.shields.io/badge/PyTorch%201.9-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white) |  ![Qiskit](https://img.shields.io/badge/Qiskit%200.29-%236929C4.svg?style=for-the-badge&logo=Qiskit&logoColor=white) |  IBM QASM & AER Simulator (for local) | Qiskit Quantum Machine Learning Application Module | [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Naereen/badges)
                    
                     
                     
 **Note** : **kaggle.json** credential file is required to download **Surface Crack Detection** dataset from **Kaglge.com**

 # Design decisions and architecture
 
 In order to highlight the differentiating faetures, while implementing the **Quantum Kernel Alignment** a compartive study was performed across 3 methodologies (mentioned below) for same problem of processing images from **Surface Crack Detection** dataset (**Kaggle.com**), 
    
 1. **Classical Convolutional Neural Networks** ([Surface Crack-recognition with CNN & Pytorch](https://github.com/iotaisolutions/BMWQunatumChallenge2021/blob/main/code/Surface_Crack_recognition_with_CNN_%26_Pytorch_Reduced_Sample_Size.ipynb)) : From original dataset of 20k positive & negative images, only used a sample subset of 1000 postive  & negative images of 227 x 227 pixels along with pretrained model of resnet50.
 2. **Quantum Neural Networks** ([Surface Crack-recognition with QNN & Pytorch](https://github.com/iotaisolutions/BMWQuantumChallenge2021/blob/main/code/Surface_Crack_recognition_with_QNN_%26_Pytorch_Reduced_Sample_Size.ipynb)): From original dataset of 20k positive & negative images, only used a sample subset of 1000 postive  & negative images of 227 x 227 pixels, with two convolution layer and fully connected layer apart from Hybrid layer.
 3. **Quantum Kernel Alignment** for **Quantum Neural Networks** ( [Surface Crack-recognition with QKA,QNN & Pytorch](https://github.com/iotaisolutions/BMWQunatumChallenge2021/blob/main/code/Surface_Crack_recognition_with_QNN_%26_Pytorch_Reduced_Sample_Size.ipynb)): Due to Quantum Computing resource restrictions, considered only 1000 images of 8 x 8 pixels, with single convolution layer and fully connected layer apart from Hybrid layer. 

# [Project Report](https://github.com/iotaisolutions/hackathon-submission/blob/main/Reports/QISKIT%20RUNTIME%20APPLICATIONS%20IN%20SURFACE%20CRACK%20DETECTION.pdf) :
## The report contextualizes the project and summarizes the software design process covering below mentioned aspects: 

1. Motivation
2. Innovation
3. Applicability
4. Role of Qiskit Runtime
5. Technology stack, design decisions, and architecture.
6. Future applications





