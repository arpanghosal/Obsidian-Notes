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

