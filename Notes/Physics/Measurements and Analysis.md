### Measuring strong force with Z-bosons:
Z bosons are typically produced when two quarks in the colliding protons annihilate. In this weak-interaction process, the strong force comes into play through the radiation of gluons off the annihilating quarks. This radiation gives the Z boson a “kick” transverse to the collision axis (transverse momentum). The magnitude of this kick depends on the strong coupling constant. A precise measurement of the distribution of Z-boson transverse momenta and a comparison with equally precise theoretical calculations of this distribution allows the strong coupling constant to be determined.

---

### ATLAS H->yy , H mass analysis (JHEP08(2022)027) :
https://doi.org/10.1007/JHEP08(2022)027
"We choose multiple H signal samples and then do analytic fits. 
For signal we choose DS crystall ball with Gaussian center and falling tails. 
Similarly something for the bkg we have templates from data-driven estimates, MC etc."

---

There are boosted taggers for jets, there are top taggers as well. 
[[Detector#Jet tagging WPs]]


---

# Unknown Background processes :
In cases where the Standard Model (SM) doesn't provide comprehensive information about the backgrounds, experimentalists employ several approaches to determine or estimate these background processes. Here are some common strategies:

1. **Data-Driven Methods**:
    
    - **Sidebands**: In cases where the signal and background regions of a distribution overlap, sidebands are regions of the distribution away from the signal region. By examining the data in these sidebands, researchers can estimate the shape and rate of the background.
    - **Control Regions**: Similar to sidebands, control regions are areas of the data that closely resemble the background process but are separate from the signal region. Data from these control regions can be used to estimate background contributions.
2. **Monte Carlo Simulations**:
    
    - Researchers use Monte Carlo (MC) simulations to model both SM and background processes. MC generators simulate the production and decay of particles, and these simulated events are processed through the same detector simulation and reconstruction software used for real data. Comparing real data to MC simulations can help estimate background processes.
3. **Data-Background Comparison**:
    
    - Researchers perform a detailed comparison of data to the background predictions from various sources, such as MC simulations or known SM processes. Discrepancies between data and background predictions can be used to refine estimates of the background.
4. **Extrapolation and Scaling**:
    
    - Sometimes, the background in one region of the analysis can be extrapolated or scaled from a region where it is better understood. For example, if a certain background process is well-measured at high energies, it may be extrapolated to lower energies.
5. **Template Fits**:
    
    - In cases where multiple background processes contribute to a signal region, researchers use template fits to simultaneously estimate the contributions of each background. This method involves modeling the shape of the background processes with templates and fitting them to the observed data.
6. **Machine Learning Techniques**:
    
    - Advanced machine learning techniques, such as neural networks or boosted decision trees, can be used to distinguish between signal and background events based on multivariate data analysis. These techniques can help improve the separation of signal and background events.
7. **External Data Sources**:
    
    - In some cases, researchers may use external data sources, such as data from other experiments or theoretical predictions, to estimate background processes.
8. **Blind Analyses**:
    
    - In blind analyses, researchers deliberately hide a portion of the data to avoid potential biases in the estimation of background processes. Once the background estimates are finalized, the hidden data can be unblinded for the final analysis.

---


# Trivia - for note-keeping:
**Loose Online Identification**: "Online" implies that this identification happens in real-time, as the data is being collected. "Loose" means the criteria for identifying photons aren't very stringent – the system is set to cast a wide net to capture as many potential photon events as possible.
#### $\gamma$ identification :
- **Based on Energy Leakage in the Hadronic Calorimeter**:
    
    - **Hadronic Calorimeter**: A component of the detector that measures the energy of particles that interact strongly (like protons and neutrons, collectively known as hadrons).
    - **Energy Leakage**: When a photon passes through the calorimeter, it might deposit some energy. This "leakage" of energy is one of the factors used to identify the presence of photons.
- **Shower Shape in the Second Layer of the EM Calorimeter**:
    
    - **EM Calorimeter**: This stands for Electromagnetic Calorimeter, a part of the detector specifically designed to measure the energy of particles that interact electromagnetically, like electrons and photons.
    - **Shower Shape**: When a photon hits the EM calorimeter, it creates a cascade of secondary particles, known as a "shower." The spatial pattern (shape) of this shower, especially in the second layer of the EM calorimeter, helps in identifying the photon.


-----

# Cross section:
The concept of a "cross section" in particle physics, especially in the context of experiments like those at the Large Hadron Collider (LHC), is an aggregate measure and not specific to individual events. Let's clarify this concept:

### Definition of Cross Section:

- **Aggregate Measure**: The cross section of a specific process in particle physics is a measure of the probability of that process occurring. It is an aggregate or average measure over many events, not a characteristic of individual events.
- **Unit of Measurement**: Cross sections are typically measured in units such as barns (where 1 barn = \(10^{-24}\) cm²). This unit essentially quantifies the "effective target area" for the process to occur.

### Cross Section in the Context of LHC:

1. **Total vs. Differential Cross Sections**:
   - **Total Cross Section**: This refers to the total probability of a certain type of interaction occurring between particles, integrated over all possible final states and kinematic configurations (the entire phase space).
   - **Differential Cross Section**: This describes how the probability is distributed over different parts of the phase space, such as how it varies with angle or momentum.

2. **Not Event-Specific**: The cross section is not a property of a single collision event but is derived from observing many events. For example, in a proton-proton collision at the LHC, the cross section of producing a Higgs boson is a statistical measure based on the number of Higgs bosons produced in a large number of collisions.

3. **Calculating Cross Sections**:
   - The cross section is calculated by counting the number of times a particular process occurs (e.g., the production of a certain particle), normalizing by the number of total collisions, and considering factors like luminosity (a measure of the number of particles colliding per area per time).
   - It is an average measure that reflects how likely a specific process is to occur under given conditions.

### Example:

Imagine conducting an experiment at the LHC to measure the cross section of a specific process, like the production of a top quark pair (\(t\bar{t}\)). You would:

1. Count the number of \(t\bar{t}\) production events observed.
2. Divide this count by the total number of proton-proton collisions (taking into account the integrated luminosity).
3. The result is the cross section for \(t\bar{t}\) production, representing the average likelihood of this process occurring per collision, not a property of each individual collision event.

### Conclusion:

In summary, the cross section is a statistical concept that reflects the average likelihood of a specific process occurring in a particle collision. It is not a characteristic of individual events but rather a property derived from the ensemble of many events. This measure is fundamental in particle physics, allowing physicists to compare experimental results with theoretical predictions and to understand the fundamental interactions governing particle behavior.

----

### Why different event generators?
Event generators like Herwig and Pythia are crucial tools in high-energy physics, particularly in the study of particle collisions, such as those occurring at the Large Hadron Collider (LHC). Although they are designed to simulate the same underlying physics, different event generators have distinct features and approaches, which lead to a variety of them being developed and used. Here are some of the major differences:

### 1. Modeling of Physical Processes

- **Different Algorithms and Approximations**: Each event generator uses its own algorithms and approximations for simulating various aspects of particle collisions. This includes the initial hard scattering process, parton shower development, hadronization (the process by which quarks and gluons transform into hadrons), and decay of unstable particles.
- **Example**: Pythia uses the Lund string model for hadronization, while Herwig uses a cluster model. These models have different theoretical underpinnings and lead to different predictions in certain scenarios.

### 2. Tuning and Parameterization

- **Tuning to Experimental Data**: Each generator has numerous parameters that need to be tuned to experimental data. Different generators may be tuned to different sets of data, or use different methods for tuning, resulting in variations in their predictions.
- **Parameter Choices**: The choice and range of parameters available for tuning can also differ, affecting the flexibility and applicability of the generator in various scenarios.

### 3. Software Architecture and Usability

- **Ease of Use and Integration**: The design and architecture of the software can vary, affecting how easy it is to use, modify, and integrate with other tools and frameworks in particle physics.
- **Community and Support**: Different generators may have different levels of community support, documentation, and frequency of updates, impacting their adoption and longevity.

### 4. Niche Applications

- **Specialization for Certain Processes**: Some event generators are more specialized for certain types of processes. For example, a generator might be particularly adept at simulating electroweak interactions, QCD jets, heavy-ion collisions, or other specific aspects of particle physics.
- **Development Philosophy**: Different development teams might focus on different aspects of simulation, leading to generators with distinct strengths and weaknesses.

### 5. Theoretical Framework

- **Variations in Theoretical Models**: Although all generators are based on the Standard Model of particle physics, they might implement the theoretical framework differently, especially in areas where the theory is less certain or in modeling beyond the Standard Model physics.

### Why Multiple Generators?

- **Cross-Validation**: Having multiple event generators allows for cross-validation of results. If different generators, with their unique approaches and models, agree on a prediction, it increases confidence in the results.
- **Coverage of Uncertainties**: Different generators can help in exploring the theoretical uncertainties in particle physics predictions.
- **Adaptation to New Discoveries**: As new experimental data becomes available, different generators may adapt at different rates or in different ways, providing a broader understanding of the data.

In summary, while event generators like Herwig and Pythia aim to simulate the same fundamental physics, their differences in modeling approaches, parameterizations, and software design make each of them suitable for different purposes. The existence of multiple generators enhances the robustness and depth of theoretical predictions in particle physics.

----

#prwfiles 

# Pileup and reweighting:

In the context of ATLAS data analysis at CERN, PRW (Pileup Reweighting) and LumiCalc files are specific tools used for handling aspects of data related to luminosity and pileup. These are terms related to the ATLAS software framework Athena and are crucial for ensuring the accuracy and reliability of the data analysis. Let’s delve into each of these:

### 1. PRW (Pileup Reweighting) Files:
- **Pileup:** In the high-energy physics context, pileup refers to multiple proton-proton collisions that occur in a single bunch crossing at the LHC. This can create additional tracks or energy deposits in the detector that are not associated with the primary interaction of interest. Pileup can vary significantly from one data-taking period to another.
- **Purpose of PRW:** Pileup Reweighting is a process used to correct the simulated data so that its pileup distribution matches that of the real data. This is important because the conditions under which the real data were collected (including the intensity of the proton beams and the operational configuration of the LHC) can vary and may not always align with the conditions assumed in the simulation.
- **PRW Files:** These files contain information about the pileup conditions in the real data and are used to adjust the simulated data accordingly. The adjustments ensure that analyses using simulated data are representative of the actual experimental conditions.

### 2. LumiCalc Files:
- **Luminosity Data:** Luminosity is a measure of the number of particles per area per time passing through a detector and is a crucial parameter in particle physics. It determines the rate at which collisions occur in the detector.
- **LumiCalc Tool:** LumiCalc is a software tool used to calculate the integrated luminosity of data sets. It takes into account various operational parameters of the LHC and the ATLAS detector to determine the amount of useful data collected over a given period.
- **LumiCalc Files:** These files contain detailed luminosity calculations and are essential for data analysis. They help researchers understand how much data they have and under what conditions it was collected, which is critical for calculating cross-sections and other important physical quantities.

### Integration in Data Analysis:
- Both PRW and LumiCalc files are integral to the data analysis process in ATLAS. Researchers use these tools to ensure that their analyses of simulated data accurately reflect the experimental conditions and that they correctly interpret the amount of data they have collected.

### Usage in Athena:
- In the Athena software framework, these tools and files are used as part of the data processing and analysis chain. Athena, being the primary software used by the ATLAS Collaboration, provides the necessary infrastructure for implementing these corrections and calculations.

Pileup Reweighting (PRW) in the context of ATLAS data analysis is a crucial procedure to ensure that simulations accurately reflect real experimental conditions, specifically regarding pileup - the occurrence of multiple proton-proton interactions in a single bunch crossing at the Large Hadron Collider (LHC). Let’s explore how this reweighting is performed:

### Understanding Pileup:
- **Pileup:** In the high-luminosity environment of the LHC, a single bunch crossing can result in multiple collisions, leading to additional tracks or energy deposits in the detector.
- **Average Pileup (\(\mu\)):** The average number of interactions per bunch crossing, denoted as \(\mu\), is a key parameter in describing pileup. 

### The PRW Process:
1. **Data Collection:**
   - **Real Data:** For actual LHC data, the distribution of \(\mu\) (pileup profile) is measured. This involves counting the number of interactions in each bunch crossing.
   - **Simulated Data:** Simulations are run with an assumed pileup distribution. However, this assumed distribution might not match the actual pileup experienced in the collected data.

2. **Pileup Reweighting:**
   - **Objective:** The goal is to adjust the simulated data so that its pileup distribution aligns with what was actually observed in the real data.
   - **Calculation of Weights:** Weights are calculated as the ratio of the pileup distribution in real data to that in the simulated data, for each value of \(\mu\). 
   - **Applying Weights:** These weights are then applied to the simulated events. An event from the simulation that corresponds to a particular \(\mu\) value is weighted by the corresponding calculated ratio. This ensures that the overall pileup profile of the weighted simulation matches the real data.

### Algorithm and Logic:
1. **Histogram Comparison:**
   - Histograms of the pileup distribution are created for both real and simulated data.
   - The weight for each \(\mu\) bin is calculated as $(\text{Weight}(\mu) = \frac{\text{Histogram}_{\text{Real}}(\mu)}{\text{Histogram}_{\text{Simulated}}(\mu)})$.

2. **Normalization:**
   - The weights are usually normalized such that the total number of events remains the same.

3. **Event-by-Event Reweighting:**
   - In the simulation dataset, each event is assigned a weight based on its \(\mu\) value.

### Practical Considerations:
- **Accuracy of Simulation:** The more accurately the simulation’s initial pileup distribution approximates the real data's distribution, the smaller the adjustments that need to be made.
- **Variability:** Pileup conditions can vary significantly over time, so this process is crucial for analyses spanning long data-taking periods.


### Understanding \(\mu\) in More Detail:
- **Pileup Distribution:** In both real and simulated collider data, pileup can vary. In some bunch crossings, there might be just a few interactions, while in others, there could be many more. This distribution of interactions is what \(\mu\) represents.
- **Variable Nature:** The value of \(\mu\) can change from one bunch crossing to another, influenced by factors like the intensity of the proton beams and the operational configuration of the collider.

### How Weights are Calculated for Each Value of \(\mu\):
1. **Histograms of Pileup Profiles:**
   - For real data, a histogram is created representing the distribution of pileup, showing how often different values of \(\mu\) occur.
   - Similarly, simulated data will have its own pileup profile, showing the expected distribution of \(\mu\) values based on the simulation parameters.

2. **Weight Calculation:**
   - The weight for a given value of \(\mu\) is calculated by taking the ratio of the frequency of that \(\mu\) value in the real data to its frequency in the simulated data.
   - Mathematically, if \( P_{\text{real}}(\mu) \) is the frequency of a particular \(\mu\) value in the real data and \( P_{\text{sim}}(\mu) \) is the frequency in the simulated data, then the weight for that \(\mu\) value is calculated as \( \text{Weight}(\mu) = \frac{P_{\text{real}}(\mu)}{P_{\text{sim}}(\mu)} \).

3. **Applying the Weights:**
   - When analyzing the simulated data, each event is weighted according to the \(\mu\) value it corresponds to. This reweighting adjusts the simulated pileup profile to match the observed real data profile.

### Purpose of this Approach:
- **Matching Real Conditions:** The objective is to ensure that the simulated data reflects the actual pileup conditions as closely as possible. Since pileup can significantly affect the detector's response and the subsequent data analysis, accurately modeling it is crucial for drawing reliable conclusions from the simulation.

In summary, "each value of \(\mu\)" refers to the different possible average numbers of interactions per bunch crossing in the collider, and PRW involves adjusting the simulated data so that its pileup distribution matches the observed distribution in the real data. This process is fundamental in high-energy physics to ensure that simulations are representative of real experimental conditions.

## How is it done?

### Event-by-Event Reweighting:
- **General Approach:** In pileup reweighting, each simulated event is indeed reweighted on an event-by-event basis, but it's not about finding a corresponding real event. Rather, it's about adjusting the overall statistical distribution of pileup in the simulated dataset to match that of the real data.

- **How It Works:**
   - **Pileup Profile in Simulated Event:** For each simulated event, the pileup scenario (characterized by the average number of interactions per bunch crossing, \(\mu\)) is known.
   - **Weight Assignment:** This event is then assigned a weight based on the \(\mu\) value it represents. The weight is derived from the ratio of how often this \(\mu\) value occurs in the real data compared to the simulated data.

### Conceptual Simplification:
- You might think of it as if each simulated event is being "corrected" so that its pileup characteristics more closely resemble what was actually observed in the collider at that level of pileup. However, it's more about aligning statistical distributions rather than matching individual events.

### Time Factor in Pileup Calculations:
- **Temporal Variation:** You are correct that pileup can vary over time due to changes in LHC operational conditions like beam intensity.
- **Handling Temporal Variation:**
   - **Luminosity Blocks:** The real data is often divided into periods (luminosity blocks) where the operational conditions are relatively stable. The pileup profile is measured for each of these periods.
   - **Dynamic Reweighting:** The reweighting process takes into account these temporal variations by using the appropriate pileup profile for each period when adjusting the simulated data.

### Summary:
- Pileup reweighting is indeed done on an event-by-event basis in simulations, with each event being weighted according to its \(\mu\) value to align the pileup distribution with that observed in real data.
- The process is statistical in nature and aims to match the overall distribution rather than individual events.
- Temporal variations in pileup conditions are accounted for by segmenting the real data according to operational periods and applying the corresponding pileup profile for reweighting.

This approach ensures that the simulated data is representative of the actual conditions under which the experimental data was collected, which is crucial for accurate analysis and interpretation in high-energy physics research.


## Pileup Simulations:
Pileup simulation in high-energy physics, such as at the Large Hadron Collider (LHC), is a complex process. It involves modeling the additional proton-proton interactions that occur in the same bunch crossing as the primary interaction of interest. Let's explore how pileup is simulated and how the expected average number of interactions per bunch crossing (\(\mu\)) is determined:

### Simulating Pileup:
1. **Primary Interaction:** In a typical simulation for a collider experiment, the first step is simulating the primary interaction. This is the interaction that researchers are most interested in, such as the production of certain particles.

2. **Additional Interactions:** Alongside this primary event, additional proton-proton interactions are simulated. These additional interactions represent the pileup and are generally softer (lower energy) than the primary interaction.

3. **Modeling Pileup Interactions:**
   - These interactions are simulated using Monte Carlo techniques, which use probabilistic models to mimic the physical processes occurring in the collider.
   - The simulation includes various types of interactions, from relatively simple soft scatters to more complex processes.

4. **Overlaying Pileup on the Primary Event:** The simulated pileup interactions are then superimposed on the primary event. This creates a composite event that includes both the interesting physics from the primary interaction and the background noise from pileup.

### Determining the Expected \(\mu\):
1. **LHC Operational Parameters:**
   - The expected \(\mu\) is influenced by the operational parameters of the LHC, such as beam intensity, the number of protons per bunch, and the rate of bunch crossings.
   - The LHC operating conditions are planned and known in advance, which allows for predictions of the expected \(\mu\) for a given running period.

2. **Historical Data and Predictive Models:**
   - Historical data from previous runs of the LHC is used to build predictive models of pileup conditions.
   - These models take into account the varying conditions and efficiencies of the collider over time.

3. **Monte Carlo Simulations:**
   - Monte Carlo simulations are also used to predict the distribution of \(\mu\) values for different LHC running scenarios.
   - These simulations help in understanding how often certain \(\mu\) values are likely to occur.

### Practical Considerations:
- **Variability:** Pileup conditions can vary significantly from one run to another or even within a single run, depending on the LHC’s performance.
- **Adjustments in Data Analysis:** As the actual pileup conditions can differ from the initial predictions, adjustments using pileup reweighting techniques (as discussed in previous messages) are necessary when analyzing the collected data.

## Separate MC and Data:

In the ATLAS experiment at the Large Hadron Collider (LHC), the processing of pileup information is indeed handled separately for real experimental data (often just referred to as "data") and for simulated data. This separate processing reflects the different nature and requirements of these two types of datasets:

### Processing Pileup in Real Data:
- **Measurement of Pileup:** For real experimental data, the pileup conditions are directly measured. This involves analyzing the data from each bunch crossing to determine the number of interactions that occurred, which is used to calculate the average number of interactions per bunch crossing (\(\mu\)).
- **Luminosity Blocks:** The data is often divided into luminosity blocks, periods during which the operational conditions of the LHC, including pileup, are relatively stable. The pileup profile is calculated for each of these blocks.
- **Creation of Pileup Profiles:** The result is a pileup profile that represents the actual conditions during the data-taking periods. This profile is essential for subsequent data analysis and for comparison with simulations.

### Processing Pileup in Simulated Data:
- **Simulating Pileup:** In simulated data, pileup is artificially generated. This involves simulating additional proton-proton interactions (other than the primary interaction of interest) that would occur in a typical LHC bunch crossing.
- **Pileup Models:** The simulation uses models of pileup that are based on the LHC's operating parameters and historical data. These models predict the pileup conditions that the simulated events are likely to experience.
- **Adjustment via Reweighting:** Since the exact pileup conditions can vary, the simulated data is often reweighted after the fact to match the pileup profile of the real data. This ensures that the simulation accurately reflects the experimental conditions.

### Why Separate Processing is Necessary:
- **Reflecting Actual Conditions:** The real data contains the actual pileup conditions experienced during the experiment, which are crucial for understanding the experimental environment.
- **Controlled Conditions in Simulation:** In contrast, simulations allow for controlled modeling of pileup, enabling researchers to test various scenarios and conditions. However, these simulated conditions need to be aligned with the real data for accurate analysis.
- **Pileup Reweighting:** The process of reweighting the simulated data to match the real data's pileup profile is a critical step in ensuring that analyses based on simulations are valid and representative of the true experimental conditions.

In summary, the separate processing of pileup information in real and simulated data within the ATLAS experiment is a necessary step to ensure that both datasets accurately reflect the pileup conditions and can be reliably used for physics analyses.


---

# Athena:
ATLAS Athena is a software framework used for processing and analyzing data collected by the ATLAS experiment at the Large Hadron Collider (LHC) at CERN. It's a comprehensive suite of tools and algorithms designed to handle everything from the initial processing of raw data from the detector through to the high-level physics analysis. Let's break down the purpose, workflow, and types of tools in Athena.

### Purpose of Athena:
Athena is designed to:
- **Process Raw Data:** Transform raw data from the ATLAS detector into formats suitable for analysis.
- **Simulation:** Simulate particle collisions and detector responses.
- **Data Analysis:** Provide tools for data reconstruction, event selection, and physics analysis.

### Workflow of Athena:
The typical workflow in Athena involves several key stages:

1. **Data Processing:**
   - **Raw Data Handling:** The first step involves processing the raw data from the ATLAS detector. This includes decoding the data from its raw format and performing initial calibrations.
   - **Reconstruction:** The next major step is reconstruction, where the processed data is converted into physical objects like tracks, vertices, jets, photons, electrons, muons, etc.

2. **Monte Carlo Simulation:**
   - To compare the observed data with theoretical predictions, Monte Carlo simulations are used to model what the detector should see for various theoretical scenarios.
   - The simulated data undergoes a similar reconstruction process as the real data.

3. **Data Analysis:**
   - Once the data is reconstructed, physicists use various analysis tools to select events of interest, apply further calibrations and corrections, and perform statistical analyses.
   - This stage involves a lot of custom code written by individual physicists or analysis groups, tailored to specific analysis goals.

4. **Derivation Production:**
   - For complex analyses, derived datasets (called derivations) are produced, containing only the necessary information. This reduces the data volume and simplifies subsequent analyses.

### Tools in Athena:
- **Algorithms and Sequencers:** Athena uses algorithms (specific tasks like track finding) and sequencers (which define the order of executing algorithms) for data processing.
- **Gaudi Framework:** Athena is built on top of the Gaudi software architecture, a framework for HEP data processing.
- **ROOT Integration:** Athena integrates with ROOT, a major data analysis framework in HEP, for tasks like histogramming and statistical analysis.
- **Pythia, Geant4, etc.:** For simulation, Athena interfaces with tools like Pythia (for particle decay and hadronization) and Geant4 (for simulating particle interactions with the detector).

### Purpose and Impact:
- **Multi-Purpose:** Athena is designed to be versatile to handle a wide range of analyses, from Standard Model measurements to searches for new physics.
- **Collaborative Development:** It is developed and maintained collaboratively by a large community of physicists and software engineers.

---

# Jet physics terminology:

In jet physics, particularly in the context of analyzing data from high-energy particle collisions, "N-subjettiness," "tuning," and "grooming" are important concepts. They are used to analyze and interpret the substructure of jets, which are sprays of particles produced by the hadronization of quarks and gluons. Understanding these concepts is crucial in identifying different types of particles and processes in collider experiments like those at the Large Hadron Collider (LHC). Let's break down each term:

### N-Subjettiness
- **Definition**: N-subjettiness is a quantitative measure used to determine the structure of a jet. It helps in identifying how many subjets (smaller jet-like structures) are contained within a jet. 
- **Calculation**: It is defined for each integer N and is calculated based on the distances between particles in the jet and N candidate subjet axes. The smaller the value of N-subjettiness, the more consistent the jet is with having N subjets.
- **Application**: This

is especially useful in distinguishing between jets originating from different types of particles, such as differentiating a jet from a single quark or gluon from those originating from a top quark or a W/Z boson, which can decay into multiple quarks.

### Jet Tuning
- **Definition**: Jet tuning refers to the process of adjusting parameters in jet algorithms to optimize the performance of jet reconstruction and identification.
- **Application**: This can involve tuning parameters that define how particles are clustered into jets and how the jet properties are calculated. The goal is to maximize the efficiency and accuracy of jet identification, particularly in complex environments with overlapping jets or high background noise.
- **Context**: Jet tuning is often performed using simulations to match the jet reconstruction to the theoretical or phenomenological models as closely as possible.

### Jet Grooming
- **Definition**: Jet grooming involves techniques to remove soft and wide-angle radiation from a jet. This is done to reduce the impact of less relevant, low-energy particles and initial-state radiation, or multiple interactions in the jet formation process.
- **Techniques**: Common grooming techniques include trimming, pruning, and soft drop. These methods help to reveal the hard, core structure of the jet and make the jet properties less sensitive to the details of the softer radiation.
- **Usage**: Grooming is particularly important in analyses where the jet substructure plays a key role, such as in searches for new particles or in precision measurements where understanding the core of the jet is crucial.

By employing N-subjettiness, tuning, and grooming techniques, physicists can better analyze and interpret the data from particle collisions, leading to more accurate identification of particles and processes. This is essential in the search for new physics phenomena and in improving our understanding of fundamental particles and their interactions.


---

# Look Elsewhere effect:

   The Look-Elsewhere Effect (LEE) is a statistical phenomenon that occurs in the analysis of data over a wide parameter space or multiple testing scenarios. It's particularly relevant in fields like particle physics, astronomy, and any discipline involving extensive data searches for signals among background noise. The essence of the Look-Elsewhere Effect is that the more places you look for a signal, the higher the chance of finding a significant signal-like fluctuation purely by chance, even in the absence of a real signal.

### Understanding the Look-Elsewhere Effect

Imagine you're searching for a specific signal in a large dataset. If you look at many different regions or test multiple hypotheses, it's likely that at least one of them will show an apparent signal just due to random fluctuations in the data. This apparent signal might seem statistically significant within that local region or specific hypothesis test but becomes less significant when considering the entire search area or the number of hypotheses tested.

### Example in Particle Physics

A classic example is the search for new particles in collider experiments, where physicists scan a wide range of energy levels for excess events (signals) that might indicate the presence of a new particle. If the analysis is not corrected for the Look-Elsewhere Effect, a local excess that appears significant could merely be a statistical fluctuation that's expected when examining many energy bins.

### Correcting for the Look-Elsewhere Effect

To account for the LEE, researchers use various statistical methods to adjust the significance of their findings. One common approach is to calculate a "global significance" from the "local significance." The local significance measures how unlikely it is to observe a signal-like fluctuation in a specific region of the parameter space, assuming no real signal is present. The global significance, however, reflects the probability of observing such a fluctuation anywhere in the searched parameter space.

- **Trial Factor:** This is an adjustment factor that quantifies the effective number of independent searches or hypothesis tests performed. Calculating the trial factor can be straightforward in some cases (e.g., when the parameter space is evenly and discretely divided) but may require more sophisticated statistical techniques in others, especially when the parameter space is continuous or when the tests are not independent.

- **P-Value Adjustment:** Another method involves adjusting the p-values obtained from individual tests to reflect the multiplicity of tests performed. Techniques like the Bonferroni correction are examples of this approach, although they may be overly conservative in some contexts.

### Importance

Correcting for the Look-Elsewhere Effect is crucial for maintaining the integrity of scientific findings. Without such corrections, the risk of false positives increases, potentially leading to incorrect conclusions about the presence of new phenomena. By appropriately accounting for the LEE, researchers can better differentiate between true signals and statistical fluctuations, ensuring that claims of discoveries are robust and reliable.

----


# Ideogram method:
The ideogram method in particle physics is used for mass fitting, particularly in the context of particle decay studies. It involves constructing a likelihood function based on the invariant mass of particle decay products, incorporating various factors like resolution effects and background contributions. This method allows for precise determination of particle masses and is often utilized in experiments such as those conducted at the Large Hadron Collider (LHC).

For more detailed information, you can refer to specific particle physics literature or research papers that delve into the technical aspects of the ideogram method.

See cms paper on top mass measurement: https://arxiv.org/pdf/1805.01428

The ideogram method is also a fitting method used in particle physics. It combines the results of multiple invariant mass measurements to extract the most probable value for the mass of a particle. This method constructs a likelihood function that accounts for statistical and systematic uncertainties, providing a precise fit to the mass distribution. The ideogram approach is valuable for achieving high precision in mass determinations, often applied in the analysis of data from particle collision experiments.

----
