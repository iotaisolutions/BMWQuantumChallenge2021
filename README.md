# hackathon-submission
IEEE SERVICES Hackathon 2021 Repository


# QKA for QNN   
## Exploring Quantum Kernel Alignment Runtime for optimizing Quantum Neural Network (processing images from **Surface Crack Detection** dataset)
[**IEEE SERVICES HACKATHON 2021**](https://github.com/IEEEServices/hackathon-2021#the-cloud-as-a-quantum-computing-accelerator)

**Members**: <!-- up to 6 members per term -->
- Anuj Mehrotra,@iotaisolutions, IOTAONEIQ Solutions Pvt. Ltd. (India)
- Vardaan Sahgal,@Vardaan Sahgal, University of Delhi (India), B.Sc. (Hons.) Physics
- Mitesh Adake, @Mitesh, Pune Institute of Computer Technology (India), Computer Engineering
- Vishal Sharathchandra Bajpe, @Vishal Bajpe, Sahyadri College of Engineering & Management (India), Mechanical Engineering
- Rajatav Dutta, @Rajatav Dutta, SAP Labs (India)
- Meghashrita Das, @Meghashrita Das,Indian institute of technology Kharagpur (India), Agricultural , Food and Financial engineering

**Quantum neural networks** are computational neural network models which are based on the principles of quantum mechanics and acts application-agnostic computational units that can be used for many different use cases : like Image Processing , Natural Language Processing, computer games, function approximation, handling big data, in modelling social networks, associative memory devices, and automated control systems etc.

In **Quantum Machine Learning (QML)**, Quantum kernels is the approach of exploiting group structure in data which helps to achieve quantum speedup ( but not mandatory). Quantum kernels can be optimized with a technique called kernel alignment.

Different quantum computing methods are used to encode classical data in a quantum-enhanced feature space. For computing quantum kernels, an algorithm called  Quantum kernel estimator (QKE) is  used which leverages quantum circuits for classical data and provides an efficient way to evaluate inner products between data in a quantum feature space.

Quantum Neural Networks (QNN) are parameterized quantum circuits which acts like linear methods in quantum feature space  and suitable case for using quantum kernels and in turn can be optimized using **Quantum Kernel Alignment (QKA)**. 

QKA is an iterative quantum-classical algorithm, in which quantum hardware is used to execute parametrized quantum circuits  for evaluating the quantum kernel matrices with QKE, while a classical optimizer tunes the parameters of those circuits to maximize the alignment. Iterative algorithms of this type can be slow due to latency between the quantum and classical calculations. 

Qiskit Runtime is a new architecture that can speed up iterative algorithms like QKA by co-locating classical computations with the quantum hardware executions.

In this project, in order to showcase an application of **Quantum Kernel Alignment Runtime** , QKA was used foroptimizing Quantum Neural Network, which processes images from **Surface Crack Detection** dataset (**Kaggle.com**) and can be scaled up & used as a module in **Automated Quality Management** in assembly line of Manufacturing Factory units (like of Automobile).

Below table covers Technology Ecosystem for implementing this project:

Programming Language| Classical (Deep) ML Framework| Quantum Compluting Development Platform | Simulator | Additional Module| Coding Collaboration Environment 
------------ | -------------| -------------| -------------| -------------|-------------
  Python 3.x >= 3.7  |  Pytorch 1.9 |  Qiskit 0.29 |  IBM QASM ( With Qiskit Runtime) & AER Simulator (for local) | QKA.PY from https://github.com/Qiskit-Partners/qiskit-runtime |Google Colab
                    
                     
                     
 **Note** : **kaggle.json** credential file is required to download **Surface Crack Detection** dataset from **Kaglge.com**
  
  # Methodology 
    
 In order to highlight the differentiating faetures, while implementing the **Quantum Kernel Alignment Runtime** a compartive study was performed across 3 methodologies (mentioned below) for same problem of processing images from **Surface Crack Detection** dataset (**Kaggle.com**), 
    
 1. **Classical Convolutional Neural Networks** ([Surface Crack-recognition with CNN & Pytorch](https://github.com/iotaisolutions/hackathon-submission/blob/main/code/Surface_Crack_recognition_with_CNN_%26_Pytorch.ipynb)) : Used complete dataset of 20k postive  & 20k negative images of 227 x 227 pixels along with pretrained model of resnet50.
 1. **Quantum Neural Networks** ([Surface Crack-recognition with QNN & Pytorch](https://github.com/iotaisolutions/hackathon-submission/blob/main/code/Surface_Crack_recognition_with_QNN_%26_Pytorch.ipynb)): Due to Quantum Computing resource restrictions and inline with QKA methodology, considered only 100 images of 7 x 7 pixels  
 1. **Quantum Kernel Alignment Runtime** for **Quantum Neural Networks** ( Surface Crack-recognition with QNN , QKA & Pytorch.ipynb): Due to Quantum Computing resource restrictions, considered only 100 images of 7 x 7 pixels 





