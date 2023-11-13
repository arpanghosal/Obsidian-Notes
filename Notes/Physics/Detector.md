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


### Comparison of athena with big companies: 
The complexity of the Athena framework used in the ATLAS experiment at CERN can be quite high, primarily due to the unique requirements and challenges posed by high-energy particle physics experiments. However, comparing its complexity to similar frameworks used by big companies in other industries can be a bit like comparing apples and oranges because the nature of the tasks and the goals differ significantly. Nevertheless, I can provide some context:

1. **Specialization:** Athena is highly specialized for particle physics experiments, particularly for the ATLAS detector at the Large Hadron Collider (LHC). It's designed to handle the intricacies of tracking and reconstructing particle interactions in a high-energy physics environment. The requirements for such frameworks are often unique and demand a deep understanding of particle physics.
    
2. **Volume and Speed:** Particle physics experiments generate vast amounts of data in very short timeframes. The complexity of Athena arises from the need to process, filter, and analyze this massive data flow in real-time. This is a level of data intensity that is uncommon in many other industries.
    
3. **Distributed Computing:** ATLAS, like other particle physics experiments, relies heavily on distributed computing and grid computing systems to process and analyze data. The software framework must manage the intricacies of distributing tasks across a network of computing resources, which can add complexity.
    
4. **Open Source Collaboration:** Many particle physics experiments, including ATLAS, collaborate across institutions and countries, and their software frameworks are developed collaboratively in an open-source manner. This can introduce additional complexity in terms of coordinating contributions from a large and diverse group of developers.
    

When compared to software frameworks used by big companies in other industries, it's important to note that the goals and requirements can differ significantly. Corporate software frameworks might focus on scalability, security, and ease of integration with existing systems, which can also lead to high complexity in their own right.


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

# Data Preparation :

https://twiki.cern.ch/twiki/bin/viewauth/Atlas/AtlasTrigger

**Express Stream** : The primary scope of the <mark style="background: #FF5582A6;">Express stream is Data Quality and Monitoring</mark> **. 

It is NOT a stream for physics analysis. It will be processed 1-2 <mark style="background: #FFB86CA6;">hours</mark> after data taking to monitor and validate the quality of the data.


**Prescaling triggers** : keeping n out of N events for eg.  Need to be accounted for in analysis.

---
![[Pasted image 20231102102151.png]]

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


## Experiments : to be read  #lhc 
https://en.wikipedia.org/wiki/Category:Particle_experiments



#trivia
Momentum precision in some lhc experiments like Z pT in #ATLAS  can go from 0.1% to 1%.

#atlas 
The term "tune" in the context of Pythia typically refers to sets of parameters and configurations that are adjusted to best match experimental data from specific collider experiments (e.g., the Large Hadron Collider at CERN). These tunings help improve the accuracy of the simulations and make them more relevant for the specific conditions of a particular experiment.

---

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

# LHC Physics #lhc
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


# Why Detectors and what are they ?
Detectors are crucial for studying fundamental particles and their interactions. Here are some key aspects and concepts related to detector physics:

1. **Particle Detection**: Particle detectors are instruments designed to detect and measure various types of particles, including electrons, protons, neutrons, photons, and more exotic particles like neutrinos or dark matter candidates.
    
2. **Types of Detectors**:
    
    - **Gas Detectors**: These detectors use gases, like argon or helium, to detect particles through ionization and subsequent electrical signals.
    - **Scintillation Detectors**: These detectors use scintillating materials that emit flashes of light (scintillation) when particles interact with them.
    - **Solid-State Detectors**: These detectors are made from semiconductor materials and are common in applications like silicon detectors.
    - **Calorimeters**: Used to measure the energy of particles, calorimeters stop and absorb particles, measuring their energy through temperature changes.
3. **Interaction Mechanisms**:
    
    - **Ionization**: Particles passing through a medium ionize the atoms or molecules, creating charged particles that can be detected.
    - **Scintillation**: Particles excite scintillating materials, leading to the emission of light that can be detected.
    - **Cherenkov Radiation**: When a particle travels through a medium faster than the speed of light in that medium, it emits Cherenkov radiation, which is detected as a faint, bluish glow.
4. **Detector Resolution**: The resolution of a particle detector refers to its ability to precisely measure the properties of detected particles, such as energy, position, and momentum. Higher resolution detectors provide more accurate measurements.
    
5. **Detector Calibration**: Calibrating detectors is essential to ensure accurate measurements. Calibration involves adjusting the detector's response to known particle properties.
    
6. **Trigger Systems**: Particle collisions can produce an enormous amount of data. Trigger systems are used to select events of interest, allowing the most relevant data to be stored and analyzed while discarding the rest.
    
7. **Applications**:
    
    - **High-Energy Physics**: <span style="color:#0ff549">Detectors are essential components </span>of particle accelerators and colliders like the Large Hadron Collider (LHC), used to study fundamental particles and forces.
    - **Astroparticle Physics**: Detectors are used in experiments related to astrophysics, cosmic rays, and dark matter detection.
    - **Nuclear Physics**: Detectors are employed to study the behavior of <span style="color:#f5ed05">nuclei</span> and subatomic particles in nuclear reactions.
    - **Medical Physics**: Detectors are used in medical imaging techniques such as positron emission tomography (PET) and X-ray imaging.
8. **Data Analysis**: After collecting data, physicists use statistical and data analysis techniques to interpret and draw conclusions from the measurements made by particle detectors.
    
9. **Detector Innovation**: Ongoing research in detector physics focuses on improving sensitivity, precision, and scalability. Innovations include the development of more advanced semiconductor materials, scintillators, and readout electronics.


----

# Muon spectrometer
## What it contains?
- The Muon Spectrometer consists of several components, including Monitored Drift Tubes (MDTs), Cathode Strip Chambers (CSCs), and Resistive Plate Chambers (RPCs). These detectors are arranged in multiple layers.

**Drift Tubes (MDTs)**:

- MDTs are gas-filled chambers with precision-aligned anode wires and cathode strips. When a charged particle, such as a muon, passes through an MDT, it ionizes the gas. The ionized electrons drift towards the anode wire, and the time it takes for them to reach the wire is used to determine the particle's position along the tube.

**Cathode Strip Chambers (CSCs)**:

- CSCs use a different technology. They consist of gas chambers with anode wires and cathode strips arranged in a crossed pattern. When a muon passes through, it ionizes the gas, and the resulting charge distribution on the anode wires and cathode strips provides position information.

**Resistive Plate Chambers (RPCs)**:

- RPCs are additional detectors that help provide fast and redundant muon triggering. They operate in a different mode and are often used in the high-rate trigger system.

**Complementing Inner Trackers**:

- While the inner tracking detectors are designed to precisely measure the paths and momenta of charged particles, including electrons and charged hadrons, the Muon Spectrometer specifically focuses on muons. Muons are more penetrating and challenging to detect precisely, which is why a separate muon detection system is necessary.

**Triggering**:

- The Muon Spectrometer also plays a role in the ATLAS trigger system. It helps identify and trigger on events with high-energy muons, ensuring that interesting physics events are recorded.

## Why $\mu$ are so elusive?
Reasons for the elusiveness of muons:

1. **Short Lifetime**: Muons have a very short mean lifetime of approximately 2.2 microseconds when at rest. This short lifetime makes it challenging to observe muons directly in experiments, especially when they are produced in high-energy collisions. By the time they travel a short distance in a detector, many of them decay into electrons and neutrinos. To detect muons, experiments must capture and identify them quickly.
    
2. **Minimal Interaction**: Muons, like electrons, are charged particles, but their larger mass gives them greater momentum. This momentum means they are less affected by electromagnetic interactions. Muons are less likely to scatter or lose energy as they pass through matter, which allows them to penetrate dense materials, such as calorimeters and other detector components, relatively unscathed. This property is what makes muons useful for studying particles that would otherwise be hidden in the detector.
    
3. **Penetration Power**: Due to their minimal interaction with matter, muons can travel through several meters of dense material, making them ideal for studying particles produced deep within the detector or for identifying particles emerging from collisions. Muons are often used to probe the structure of large detectors and provide valuable information about the characteristics of particle interactions.
    
4. **Energy Signature**: In high-energy physics experiments, muons are associated with the decay of heavy particles. The detection of muons can indicate the presence of these particles, such as the W and Z bosons, or other heavy particles produced in collisions. The identification of muons is crucial for understanding the underlying physics processes.


----

# Triggers versus histogramming:
The High-Level Trigger (HLT) and Level-1 (L1) trigger systems in particle physics experiments, such as the ATLAS experiment at CERN, are distinct from online and offline histogramming, but they are closely related to the data acquisition and processing workflow. Here's how they fit into the picture:

1. **High-Level Trigger (HLT):**
    
    - The HLT is part of the online data acquisition system. It operates after the L1 trigger and is responsible for further reducing the data rate.
    - The HLT performs more detailed and computationally intensive analyses on the events selected by the L1 trigger. It uses a subset of detector information to make decisions.
    - While the HLT is part of the online system, it's not directly related to histogramming. Instead, it plays a <mark style="background: #FFB8EBA6;">role in selecting events of interest for further analysis</mark>.
2. **Level-1 (L1) Trigger:**
    
    - The L1 trigger is the first stage of the online data acquisition system. It makes rapid decisions based on simple criteria and a limited subset of detector information.
    - The L1 trigger is not directly related to histogramming, but it plays a crucial role in reducing the data rate by quickly selecting potentially interesting events for further analysis.
    - L1 trigger decisions are made in real-time, so there is no direct connection to offline histogramming.
3. **Online Histogramming:**
    
    - Online histogramming, as previously discussed, is part of the<span style="color:#fdf877"> <span style="color:#b4e1fe">real-time monitoring</span></span> <span style="color:#fdf877"><span style="color:#fdf877"></span></span>and quality control process during data acquisition.
    - It provides immediate visual and statistical information about the data, helping to monitor the experiment's performance.
    - Online histogramming is closely related to the DAQ and can help operators and physicists make decisions about data-taking and detector performance.
4. **Offline Histogramming:**
    
    - Offline histogramming is part of the later stages of data analysis, after data taking is completed.
    - It's used for<span style="color:#fdf877"> in-depth data analysis, detailed event reconstruction, and the creation of publication-ready results.</span>
    - Offline histogramming is not part of the real-time data acquisition process but is used for post-experiment data analysis.

---

# E/gamma identification:
Certainly! The identification of electrons and gamma rays (photons) in the ATLAS detector at the Large Hadron Collider (LHC) involves a series of steps and utilizes various components of the detector. Here's a simplified explanation in bullet points:

### Electron Identification

1. **Tracking System**: 
   - Electrons are initially identified by their tracks in the inner detector.
   - The inner detector tracks the path of charged particles, including electrons, as they pass through a magnetic field.

2. **Energy Measurement**:
   - Electrons produce electromagnetic showers when they interact with the material in the electromagnetic calorimeter.
   - The shape and total energy deposit of these showers are characteristic of electrons.

3. **Particle Identification**:
   - Algorithms analyze the track information and energy deposition patterns to distinguish electrons from other particles like pions.

4. **Isolation Criteria**:
   - Electrons are often isolated, meaning they have less energy deposited in a certain radius around their track. This helps differentiate them from jets.

![[Pasted image 20231112145644.png]]


### Gamma Ray (Photon) Identification

1. **No Charged Track**:
   - Unlike electrons, photons don’t leave tracks in the inner detector because they are uncharged.

2. **Energy Measurement**:
   - Photons also produce electromagnetic showers in the electromagnetic calorimeter.
   - The characteristics of these showers, such as their width and depth, are key to identifying photons.

3. **Conversion Identification**:
   - Sometimes photons convert into an electron-positron pair before reaching the calorimeter. The inner detector tracks from these conversions can be used to identify photons.
   
_The loose selection is based on shower shapes in the second layer of the electromagnetic calorimeter and on the energy deposited in the hadronic calorimeter. The tight selections add information from the finely segmented strip layer of the calorimeter, and are separately optimized for unconverted and converted photons, to account for the generally broader lateral shower profile of the latter.

4. **Isolation Criteria**:
   - Similar to electrons, isolated energy deposits in the calorimeter are indicative of photons.

![[Pasted image 20231112145626.png]]

https://cds.cern.ch/record/2634679/files/ATL-PHYS-SLIDE-2018-606.pdf 


### Common Aspects

- **Calorimeter Role**: Both electrons and photons are primarily identified by their interactions in the electromagnetic calorimeter.
- **Pattern Recognition**: Advanced algorithms analyze patterns of energy deposition and other properties to identify and distinguish these particles.
- **Vertex Reconstruction**: For events with photon conversions, reconstructing the vertex (point of origin) of the electron-positron pair helps in confirming photon identification.

### Shower Variables
Shower variables are key parameters used in particle physics to characterize the cascade of secondary particles, known as a shower, produced when a high-energy particle (like a photon or an electron) interacts with a detector, particularly a calorimeter. These showers are crucial for identifying the type of particle and measuring its energy. Here's an elaboration on their nature:

#### Types of Showers

1. **Electromagnetic Showers**: Caused by high-energy photons or electrons. These showers are characterized by a series of processes like pair production, Bremsstrahlung, and photoelectric effect, leading to a cascade of electrons, positrons, and photons.

2. **Hadronic Showers**: Produced by particles that interact via the strong nuclear force, like protons and neutrons. These showers involve more complex interactions and typically penetrate deeper into the calorimeter.

#### Key Shower Variables

1. **Shower Depth (Longitudinal Profile)**: 
   - This refers to how deep the shower penetrates into the calorimeter. 
   - Electromagnetic showers typically have a well-defined peak (due to the rapid multiplication of particles) followed by an exponential decrease.
   - The depth at which the shower reaches its maximum intensity is an important variable.

2. **Shower Width (Lateral Spread)**:
   - This measures the spread of the shower perpendicular to the direction of the incoming particle.
   - It provides information about the nature of the particle; electromagnetic showers are generally more compact compared to hadronic showers.

3. **Total Energy Deposit**:
   - The total amount of energy deposited in the calorimeter gives the energy of the original particle.
   - Calibration is crucial to accurately convert the energy deposit into the particle's energy.

4. **Shower Shape**:
   - The shape of the shower in the calorimeter, including asymmetries and irregularities, helps distinguish between different types of particles.
   - Algorithms analyze the shape to differentiate between, for example, a single photon and a jet of particles mimicking a photon.

5. **Number of Secondary Particles**:
   - Counting the number of particles in a shower can provide insights into the original particle's nature and energy.

#### Importance in Particle Detection

- **Particle Identification**: Shower variables are crucial for identifying the type of incident particle. For instance, photons and electrons produce similar electromagnetic showers, but they can be distinguished by whether or not there's an associated track in the detector.

- **Energy Measurement**: The measurement of the shower variables allows for the determination of the energy of the original particle, which is essential for reconstructing the physics of the particle collision event.

### Conclusion

The identification of electrons and gamma rays in the ATLAS experiment is a complex process that leverages the detector's capabilities in tracking charged particles and measuring energy deposition. Sophisticated algorithms analyze these data to accurately identify and differentiate between these and other types of particles.

----

