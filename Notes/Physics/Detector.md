The statement "using the measured Z rate to constrain the luminosity in the data" refers to a process in experimental physics, particularly in particle physics experiments.

In particle physics experiments, the luminosity represents the measurement of the number of particle collisions that occur per unit of time and unit of area. It is an important quantity because it determines the rate at which particles interact and allows researchers to study rare processes or phenomena.

To accurately interpret experimental data, it is crucial to have an accurate measurement of the luminosity. One way to achieve this is by using a known process with a well-understood rate, such as the production of Z bosons (Z rate). Z bosons are electrically neutral particles that decay into other particles, and their production rate is known from theoretical predictions and previous experimental measurements.

By comparing the observed rate of Z bosons in the data with the expected rate, researchers can calibrate and constrain the luminosity measurement. This calibration helps ensure that the observed rates of other particles or processes in the data are accurately determined, accounting for any fluctuations or uncertainties in the luminosity measurement.

In summary, "using the measured Z rate to constrain the luminosity in the data" means using the known production rate of Z bosons to adjust and improve the measurement of the overall collision rate (luminosity) in a particle physics experiment.

---
![[Pasted image 20231002194708.png]]

Anything above ANALYSIS is done with Athena.
Analysis with root or root based frameworks.
The ATLAS Event Data Model (Athena) is a software framework and data model used by the ATLAS collaboration for the simulation, reconstruction, and analysis of data collected from the ATLAS detector. It provides a structured way to process the vast amount of data produced by the detector during particle collisions.

$$ nice-overview $$[Data Preparation](https://indico.cern.ch/event/472469/contributions/1982677/attachments/1220934/1785823/intro_slides.pdf) 


### comparison of athena with big companies: 
The complexity of the Athena framework used in the ATLAS experiment at CERN can be quite high, primarily due to the unique requirements and challenges posed by high-energy particle physics experiments. However, comparing its complexity to similar frameworks used by big companies in other industries can be a bit like comparing apples and oranges because the nature of the tasks and the goals differ significantly. Nevertheless, I can provide some context:

1. **Specialization:** Athena is highly specialized for particle physics experiments, particularly for the ATLAS detector at the Large Hadron Collider (LHC). It's designed to handle the intricacies of tracking and reconstructing particle interactions in a high-energy physics environment. The requirements for such frameworks are often unique and demand a deep understanding of particle physics.
    
2. **Volume and Speed:** Particle physics experiments generate vast amounts of data in very short timeframes. The complexity of Athena arises from the need to process, filter, and analyze this massive data flow in real-time. This is a level of data intensity that is uncommon in many other industries.
    
3. **Distributed Computing:** ATLAS, like other particle physics experiments, relies heavily on distributed computing and grid computing systems to process and analyze data. The software framework must manage the intricacies of distributing tasks across a network of computing resources, which can add complexity.
    
4. **Open Source Collaboration:** Many particle physics experiments, including ATLAS, collaborate across institutions and countries, and their software frameworks are developed collaboratively in an open-source manner. This can introduce additional complexity in terms of coordinating contributions from a large and diverse group of developers.
    

When compared to software frameworks used by big companies in other industries, it's important to note that the goals and requirements can differ significantly. Corporate software frameworks might focus on scalability, security, and ease of integration with existing systems, which can also lead to high complexity in their own right.




---


---

https://indico.cern.ch/event/472469/contributions/1982677/attachments/1220934/1785823/intro_slides.pdf ^fb3f51
## Trigger :
We can keep one in 40,000 events.
### TTC 
timing, trigger and control (TTC) signals must be distributed to numerous electronic systems from a single location in the vicinity of the central trigger processor. 
n each experiment the TTC system must control the
detector synchronization and deliver to the front-end
electronics controllers the necessary fast signals and messages
that are phased with the LHC clock, orbit or bunch structure.
These include the 40.08 MHz bunch-crossing clock, level-1
trigger decisions, bunch and event numbers, as well as test
signals and broadcast commands.
Uses a complex architecture of timing lasers, frontends, optical connectors and encoders.


----

---

## Data Preparation :

https://twiki.cern.ch/twiki/bin/viewauth/Atlas/AtlasTrigger

**Express Stream** : The primary scope of the <mark style="background: #FF5582A6;">Express stream is Data Quality and Monitoring</mark> **. 

It is NOT a stream for physics analysis. It will be processed 1-2 hours after data taking to monitor and validate the quality of the data.


**Prescaling triggers** : keeping n out of N events for eg.  Need to be accounted for in analysis.

---

![[Pasted image 20231002200422.png]]

![[Pasted image 20231002202137.png]]

---


Bulk recon - uses calibration

lumi calc - to calculate proper Lumi from GRLs which accepts/rejects data based on goodnes..

MC warning :
Extra low momentum events must be injected into the chain to simulate the presence of multiple
proton collisions (“pile-up”) in a given LHC bunch crossing
‣ Complication: the average number of collisions per bunch crossing is a function of the LHC
parameters, and we typically do not know this when we start the Monte Carlo production
‣ Monte Carlo events must be weighted in analysis to account for discrepancies between the real
and simulated pile-up. 


---


## Experiments : to be read
https://en.wikipedia.org/wiki/Category:Particle_experiments



#trivia
Momentum precision in some lhc experiments like Z pT in #ATLAS  can go from 0.1% to 1%.

#atlas 
The term "tune" in the context of Pythia typically refers to sets of parameters and configurations that are adjusted to best match experimental data from specific collider experiments (e.g., the Large Hadron Collider at CERN). These tunings help improve the accuracy of the simulations and make them more relevant for the specific conditions of a particular experiment.



## Jet tagging WPs:
In the context of jet or quark tagging in high-energy particle physics experiments, the terms "70% working point," "60% working point," and so on refer to specific criteria used to classify or tag jets or quarks based on their properties. These working points are defined in the context of an algorithm or a set of selection criteria that aim to identify certain types of particles, such as quarks or jets, while suppressing backgrounds from other particles or processes.

Here's what these working points typically mean:

1. **70% Working Point**: If an algorithm or selection criteria are defined with a 70% working point, it means that the algorithm is<mark style="background: #FF5582A6;"> designed to be efficient</mark> in identifying the desired particle (e.g., a quark or a specific type of jet) <mark style="background: #FF5582A6;">while accepting a relatively high rate of false positives</mark>. In other words, it has a high efficiency for tagging the desired particles but may also tag some unrelated particles.
    
2. **60% Working Point**: Similarly, a 60% working point means that the algorithm is slightly more stringent in its selection criteria compared to the 70% working point. It may have a lower efficiency in tagging the desired particles but will have a lower rate of false positives.
    
3. **50% Working Point**: A 50% working point is often used as a reference or a baseline. It means that the algorithm is designed to have an approximately equal balance between efficiency and purity. It should have a moderate efficiency for tagging the desired particles while maintaining a moderate level of background rejection.
    

The choice of which working point to use depends on the specific goals of the particle physics analysis. In some cases, researchers may prioritize high efficiency (e.g., for discovering new particles), while in other cases, they may prioritize high purity (e.g., for precision measurements where background contamination must be minimized).

#Glossary 
UFO - A new type of jet input object, called a 'unified flow object' is introduced which **combines calorimeter- and inner-detector-based signals in order to achieve optimal performance across a wide kinematic range**.


---

## LHC Physics #lhc
At the Large Hadron Collider (LHC), the energy of colliding proton beams is measured using a combination of magnetic and radiofrequency (RF) systems.
- The LHC relies on powerful superconducting magnets to steer and focus the proton beams. These magnets are used to keep the protons circulating in a closed loop and guide them along their circular trajectory.
- The strength of the magnetic field determines the curvature of the proton beams and, consequently, their kinetic energy. By controlling the magnetic fields precisely, the LHC operators can control the energy of the proton beams.
- Radiofrequency (RF) cavities are another critical component of the LHC. These cavities provide electromagnetic fields that accelerate the protons as they pass through.
- As protons circulate through the LHC, they pass through RF cavities that provide them with a boost in energy. The timing and frequency of the RF cavities are precisely controlled to ensure the protons reach the desired energy.
- - - The LHC is equipped with various beam diagnostic instruments that monitor the properties of the proton beams, including their energy.
    - Beam position monitors (BPMs) are used to track the position of the beams, ensuring they remain on their designated paths.
    - Beam intensity monitors measure the number of protons in each beam.
    - Beam loss monitors detect any losses of protons from the beams, which can be an indication of problems.
    - Beam profile monitors provide information about the transverse shape and size of the beams.
- **Calibration and Precision**:
    
    - Precise calibration of the magnetic fields, RF systems, and diagnostic instruments is crucial for achieving the desired collision energy.
    - Extensive measurements and calibrations are performed regularly to ensure that the LHC operates at the specified energy levels.

----

---

### qq over gg or other way round ?
In proton-proton collisions at very high energies, such as those at the Large Hadron Collider (LHC), the gluon-gluon fusion (gg) process often becomes the dominant mode for the production of various particles. This is primarily because gluons carry a substantial fraction of the proton's momentum, and at higher energies, the gluon distribution functions grow significantly.

On the other hand, quark-antiquark annihilation processes can also be important, especially for the production of particles that couple more strongly to quarks, such as heavy quark-antiquark pairs (e.g., top quark-antiquark pairs or bottom quark-antiquark pairs).

The relative dominance of gg fusion versus quark-antiquark annihilation can vary for different particles and processes, and it depends on the specific energy regime and the kinematics of the collision. Therefore, there is no one-size-fits-all answer, and the dominance of one mode over the other can change depending on the particular physics process being studied.

----

## TDAQ partition:
The ATLAS Trigger and Data Acquisition (TDAQ) system is a combination of both hardware and software components that work together to manage the data produced by the ATLAS experiment at CERN's Large Hadron Collider (LHC). In essence, TDAQ is a complex and integrated system designed to handle the data acquisition, event selection, and data transfer processes. Here's a breakdown of its components:

1. **Hardware Components**: TDAQ includes various hardware components such as front-end electronics, data acquisition boards, and networking infrastructure. These components are responsible for reading out and digitizing data from the various subdetectors within the ATLAS detector.
    
2. **Software**: TDAQ encompasses a significant amount of software, including firmware, data acquisition software, and the High-Level Trigger (HLT) software. The firmware resides in the front-end electronics and helps with data preprocessing. Data acquisition software manages data flow and transfer, and the HLT software performs more advanced event selection and analysis.
    
3. **Partition**: In the context of TDAQ, a "partition" refers to a specific subset of the overall system that is responsible for handling data from particular subdetectors or subsystems of the ATLAS detector. Partitions are organized to efficiently process and transmit data. Each partition has its own set of hardware and software components tailored to its specific tasks.
    
4. **Distributed System**: TDAQ is a distributed system, meaning that different partitions and components are distributed across the ATLAS experiment site. Data acquisition boards, processing units, and networking infrastructure are distributed in the ATLAS control room and various underground locations. The system operates in a coordinated and synchronized manner to collect, process, and filter data from the detector in real-time.
    
5. **Data Processing and Event Selection**: TDAQ's primary function is to handle the immense data flow generated by the ATLAS detector during particle collisions. It selects events of interest based on trigger decisions, reducing the data volume to a manageable level for further analysis. This is a crucial step in particle physics experiments, as only a fraction of the data collected is relevant for physics analysis.
Here's how the ATLAS TDAQ partition relates to the various subsystems, the trigger system, and the data storage facility:

1. **ATLAS Subsystems**: The ATLAS detector is a complex instrument comprising various subsystems, including the Inner Detector, Calorimeters, Muon Spectrometer, and Tile Calorimeter, among others. These subsystems are responsible for detecting and measuring different types of particles and their properties. The TDAQ partition is responsible for collecting data from these subsystems in real-time and coordinating their operation.
    
2. **Trigger System**: The ATLAS trigger system consists of two levels: Level-1 Trigger and High-Level Trigger (HLT). The Level-1 Trigger makes rapid decisions about which events to record by performing a quick but coarse analysis of the data. The HLT, running on a large computing farm, performs a more detailed analysis of the selected events. The TDAQ is closely integrated with the trigger system, as it is responsible for the readout, filtering, and distribution of data based on trigger decisions. The TDAQ ensures that data from selected events is efficiently processed and stored while discarding irrelevant data.
    
3. **Data Storage Facility**: The data storage facility in ATLAS is responsible for archiving and managing the vast amount of data collected during LHC collisions. The TDAQ partition plays a crucial role in this process. It organizes and transmits data to the data storage facility for permanent storage, making sure that the data from selected events is properly archived for later analysis by physicists.
    

---



