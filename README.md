
# AT2 Phase-Field Fracture Simulation (FEniCS)

This repository provides a simple and modular implementation of the **AT2 phase-field fracture model** using the open-source finite element library **FEniCS**. The code is structured for clarity and educational purposes, allowing researchers and students to explore the basic ideas behind the phase-field method for brittle fracture.

If you are a beginner in FEniCS, you can learn more through my course here: [abhigupta.io/fenics-workshop](https://abhigupta.io/fenics-workshop)

## Overview

This implementation includes:
- The **AT2 phase-field fracture model** for brittle materials  
- Elastic energy decomposition into tensile and compressive parts  
- Quasi-static displacement loading  
- Configurable material and simulation parameters  
- Output written in XDMF format for visualization in ParaView  

## Citations

If you find this code useful, please cite the following works:

1. **Gupta, A., Krishnan, U. M., Mandal, T. K., Chowdhury, R., & Nguyen, V. P. (2022).**  
   *An Adaptive Mesh Refinement Algorithm for Phase-Field Fracture Models: Application to Brittle, Cohesive, and Dynamic Fracture.*  
   *Computer Methods in Applied Mechanics and Engineering*, **399**, 115347.  
   DOI: [10.1016/j.cma.2022.115347](https://doi.org/10.1016/j.cma.2022.115347)

2. **Gupta, A., Krishnan, U. M., & Chowdhury, R. (2020).**  
   *An Auto-Adaptive Sub-Stepping Algorithm for Phase-Field Modeling of Brittle Fracture.*  
   *Theoretical and Applied Fracture Mechanics*, **108**, 102622.  
   DOI: [10.1016/j.tafmec.2020.102622](https://doi.org/10.1016/j.tafmec.2020.102622)

3. **Gupta, A., Nguyen, D. T., Hirshikesh, & Duddu, R. (2024).**  
   *Damage Mechanics Challenge: Predictions from an Adaptive Finite Element Implementation of the Stress-Based Phase-Field Fracture Model.*  
   *Engineering Fracture Mechanics*, **306**, 110252.  
   DOI: [10.1016/j.engfracmech.2024.110252](https://doi.org/10.1016/j.engfracmech.2024.110252)

4. **Bijaya, A., Gupta, A., Krishnan, U. M., & Chowdhury, R. (2024).**  
   *A Multilevel Adaptive Mesh Scheme for Efficient Simulation of Thermomechanical Phase-Field Fracture.*  
   *Journal of Engineering Mechanics*, **150(6)**, 04024029.  
   DOI: [10.1061/JENMDT.EMENG-7480](https://doi.org/10.1061/JENMDT.EMENG-7480)

5. **Krishnan, U. M., Gupta, A., Kumar, A., & Chowdhury, R. (2024).**  
   *Adaptive PF-CZM for Multiphysics Fracture Analysis in Functionally Graded Materials.*  
   *Engineering Fracture Mechanics*, **310**, 110461.  
   DOI: [10.1016/j.engfracmech.2024.110461](https://doi.org/10.1016/j.engfracmech.2024.110461)

6. **Krishnan, U. M., Gupta, A., & Chowdhury, R. (2022).**  
   *Adaptive Phase-Field Modeling of Brittle Fracture Using a Robust Combination of Error-Estimator and Markers.*  
   *Engineering Fracture Mechanics*, **274**, 108758.  
   DOI: [10.1016/j.engfracmech.2022.108758](https://doi.org/10.1016/j.engfracmech.2022.108758)

7. **Mandal, T. K., Gupta, A., Nguyen, V. P., Chowdhury, R., & De Vaucorbeil, A. (2020).**  
   *A Length Scale Insensitive Phase-Field Model for Brittle Fracture of Hyperelastic Solids.*  
   *Engineering Fracture Mechanics*, **236**, 107196.  
   DOI: [10.1016/j.engfracmech.2020.107196](https://doi.org/10.1016/j.engfracmech.2020.107196)

8. **Modak, A., Krishnan, U. M., Gupta, A., Gangwar, T., & Chowdhury, R. (2024).**  
   *Sparse Polynomial Chaos Expansion and Adaptive Mesh Refinement for Enhanced Fracture Prediction Using the Phase-Field Method.*  
   *Theoretical and Applied Fracture Mechanics*, **133**, 104639.  
   DOI: [10.1016/j.tafmec.2024.104639](https://doi.org/10.1016/j.tafmec.2024.104639)

9. **Nguyen, D. T., Gupta, A., Duddu, R., & Annavarapu, C. (2025).**  
   *An Adaptive Mesh Refinement Algorithm for Stress-Based Phase-Field Fracture Models for Heterogeneous Media: Application Using FEniCS to Ice-Rock Cliff Failures.*  
   *Finite Elements in Analysis and Design*, **244**, 104311.  
   DOI: [10.1016/j.finel.2024.104311](https://doi.org/10.1016/j.finel.2024.104311)


## Running the Code via Docker

You can run the code using **Docker** without installing FEniCS manually.

### 1. Install FEniCS

After installing and starting Docker, open your **terminal** and pull the FEniCS image:

~~~
docker pull iitrabhi/fenics_notebook
~~~

### 2. Launch the FEniCS Notebook Server

Start the Jupyter Notebook server with the following command:

~~~
docker run -p 8888:8888 -v host_system_path:/root/ -w /root/ iitrabhi/fenics_notebook
~~~

**Note:** Replace `host_system_path` with the full path to the folder containing your code.  
For example, if your code is located in `D:\Codes`, run:

~~~
docker run -p 8888:8888 -v D:\Codes:/root/ -w /root/ iitrabhi/fenics_notebook
~~~

Once the container starts, copy the Jupyter Notebook URL shown in the terminal and open it in your web browser.

## 🤝 Collaborations

I am always open to research and development collaborations in computational mechanics and multi-physics simulations.  
Feel free to reach out to me on **[LinkedIn](https://www.linkedin.com/in/abhiguptaio/)** to discuss potential opportunities or joint projects.

## ⚖️ License

This project is released under the **MIT License**.  
If you use this repository or build upon it in your research, please cite the relevant papers listed above.