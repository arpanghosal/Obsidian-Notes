
Here I will dump physics stuffs. [[EFT or BSM]]

-   "Leading order" refers to the highest-order term in a perturbative expansion of a given quantity. In the context of Feynman diagrams, the leading order diagram is the one that involves the fewest number of loops. Loops represent quantum corrections to the classical interaction, and therefore diagrams with fewer loops are considered to be more accurate approximations of the actual physics.
    
-   "Tree level" diagrams are Feynman diagrams that contain no loops. They represent the classical, or tree-level, interaction between particles. The term "tree" comes from the fact that the diagram looks like a branching tree with particles as the branches.
    
-   "Born level" is another term used to describe tree-level diagrams, but specifically for particle scattering processes. In particular, the Born approximation is the leading term in a series expansion of the scattering amplitude, which is the probability of two particles scattering off each other. The Born level diagram, therefore, represents the lowest-order approximation of the scattering process.

In quantum field theory calculations, the perturbative expansion is usually carried out in powers of a small parameter, typically the coupling constant of the theory. The leading order (LO) term represents the contribution from the lowest power of this small parameter, while the next-to-leading order (NLO) term represents the contribution from the next power.

The LO term provides a good approximation to the physical process being studied, but it is not always accurate enough for precision measurements. In order to improve the accuracy of the calculation, one needs to include higher-order corrections, which correspond to diagrams with more loops and higher powers of the coupling constant.

The convergence of the perturbative expansion depends on the value of the coupling constant and the energy scale of the process being studied. At low energies, the coupling constant is typically small, and the perturbative expansion converges well. However, at higher energies, the coupling constant becomes larger, and the higher-order corrections become more important.

To account for these higher-order corrections, one can calculate the NLO contribution to the process being studied. The NLO term includes contributions from both LO and NLO diagrams, and it can significantly improve the accuracy of the calculation. However, the NLO term is typically more difficult to calculate than the LO term, as it involves more complicated diagrams and integrals.

Bias :
There are several types of bias that can occur in an experiment:

1.  Selection bias: This occurs when the sample chosen for the experiment is not representative of the population being studied. This can happen if the sample is chosen non-randomly or if certain groups are excluded from the study.
    
2.  Measurement bias: This occurs when the instruments or procedures used to make the measurements are inaccurate or imprecise, leading to a consistent over- or underestimation of the true value.
    
3.  Observer bias: This occurs when the researchers or observers involved in the experiment have preconceived ideas or expectations that influence the interpretation of the results.
    
4.  Confounding bias: This occurs when there is a variable that affects both the independent variable being studied and the outcome of interest, leading to a distorted or incorrect relationship between them.
    
5.  Reporting bias: This occurs when the results of the study are selectively reported, either by the researchers or by the media, in a way that distorts the true findings.
    

To minimize bias in an experiment, it is important to carefully design the study and control for potential sources of bias. This can involve using random sampling methods, blinding the observers or participants to the conditions of the study, using standardized and calibrated instruments, and reporting all results, regardless of whether they support the initial hypothesis or not.


----

# SM Lagrangian:
Absolutely, I'll rewrite the mathematical expressions with the Greek characters also enclosed in `$$` for proper Markdown formatting:

---

## Different Terms in the Standard Model Lagrangian

### 1. Gauge Field Terms

- **Electromagnetic Force (QED Lagrangian)**: 
  $$ \mathcal{L}_{\text{QED}} = -\frac{1}{4} F_{\mu\nu}F^{\mu\nu} $$
  where $$ F_{\mu\nu} $$ is the electromagnetic field strength tensor.

- **Weak Nuclear Force**: Part of the electroweak theory, includes the \( W \) and \( Z \) bosons.

- **Strong Nuclear Force (QCD Lagrangian)**: 
  $$ \mathcal{L}_{\text{QCD}} = -\frac{1}{4} G_{\mu\nu}^a G^{\mu\nu}_a $$
  where $$ G_{\mu\nu}^a $$ is the gluon field strength tensor.

### 2. Matter Field Terms (Fermions)

- **Leptons and Quarks**:
  $$ \mathcal{L}_{\text{fermions}} = \bar{\psi}(i\gamma^\mu D_\mu - m)\psi $$
  where $$ \psi $$ are the fermion fields, $$ \gamma^\mu $$ are the gamma matrices, $$ D_\mu $$ is the covariant derivative, and $$ m $$ is the mass term.

### 3. Higgs Field Term

- **Higgs Mechanism**:
  $$ \mathcal{L}_{\text{Higgs}} = |D_\mu \Phi|^2 - V(\Phi) $$
  where $$ \Phi $$ is the Higgs field, $$ D_\mu $$ is the covariant derivative, and $$ V(\Phi) $$ is the Higgs potential.

### 4. Yukawa Interactions

- **Mass Generation for Fermions**:
  $$ \mathcal{L}_{\text{Yukawa}} = -\sum_{\text{fermions}} y_f (\bar{\psi}_L \Phi \psi_R + \bar{\psi}_R \Phi^\dagger \psi_L) $$
  where $$ y_f $$ are Yukawa coupling constants, and $$ \psi_L, \psi_R $$ are the left-handed and right-handed components of the fermion fields.

---

Each term in the Standard Model Lagrangian is essential for describing the interactions and properties of fundamental particles and forces, except for gravity. This Lagrangian is a cornerstone of modern particle physics.

----



## Yukawa coupling  and other SM interactions :
The Yukawa coupling is a coupling constant that describes the strength of the interaction between a fermion and the Higgs field. It's represented by the symbol "y" in equations. Specifically, it determines how strongly a fermion field couples to the Higgs field and, consequently, how much mass the fermion acquires through this interaction.
Yukawa couplings describe the interaction between fermions (quarks and leptons) and the Higgs field. They determine how strongly these particles couple to the Higgs field, leading to mass generation.
he Yukawa coupling is considered a fundamental aspect of the Standard Model of particle physics, which is the prevailing theoretical framework describing the behavior of fundamental particles and their interactions. It's not a consequence of something more fundamental within the Standard Model; instead, it's one of the building blocks of the theory.

In the Standard Model, particles acquire mass through their interactions with the Higgs field, and the strength of these interactions is quantified by Yukawa coupling constants. These coupling constants are fundamental parameters of the theory, and they are determined experimentally for different types of particles, such as quarks and leptons.

- **Gauge Interactions:** These are associated with the exchange of gauge bosons, which are particles responsible for mediating the fundamental forces. There are three types of gauge interactions in the Standard Model:
    
    - Electromagnetic Interaction: Described by the electromagnetic coupling constant, denoted as "α" (alpha).
    - Weak Interaction: Described by the weak mixing angle (θw) and the weak coupling constants for charged (g_w+) and neutral (g_w) weak interactions.
    - Strong Interaction (Quantum Chromodynamics, QCD): Described by the strong coupling constant, denoted as "αs" (alpha_s).
- - **Higgs Interaction:** This interaction is associated with the self-interaction of the Higgs field itself. It plays a role in the dynamics of the Higgs field and the Higgs boson.
### Rise of bosons from fields:
Here's a simplified explanation of how a field gives rise to a boson:

1. **Field Concept:** In quantum field theory, fields are pervasive throughout space and time. These fields can be scalar fields (like the Higgs field), vector fields (like the electromagnetic field), or more complex fields, depending on the type of particle or force being described.
    
2. **Quantization:** When you quantize a field, you essentially divide it into tiny discrete units or quanta. Each of these quanta is associated with a particle. For example, in the case of the electromagnetic field, the quanta are called photons, which are massless bosons.
    
3. **Bosons:** Bosons are a type of particle that obeys Bose-Einstein statistics, which allow multiple bosons to occupy the same quantum state simultaneously. This is in contrast to fermions, which obey Fermi-Dirac statistics and have the Pauli exclusion principle, preventing multiple fermions from occupying the same quantum state.
    
4. **Higgs Mechanism:** In the case of the Higgs field, which is a scalar field, the quantization process leads to the emergence of a boson called the Higgs boson. The Higgs boson is the particle associated with the Higgs field. The Higgs mechanism is responsible for giving mass to other particles in the Standard Model, as we discussed earlier. The interaction between particles with spin (fermions) and the Higgs field involves the exchange of Higgs bosons.

## CP violating couplings
CP-violating anomalous couplings refer to interactions between particles that violate both the symmetries of charge conjugation (C) and parity (P) conservation, and involve deviations from the expected behavior of particles predicted by the Standard Model of particle physics.

In the Standard Model, particles and their interactions are described by quantum field theory, and the theory predicts the strengths of various interactions between particles, including their coupling strengths. The couplings between particles can be represented by coupling constants, which are typically assumed to be constants that do not vary with energy or other parameters.

However, in some extensions of the Standard Model, such as in theories that include extra dimensions or new particles, anomalous couplings can arise. These anomalous couplings can result in deviations from the expected behavior of particles and interactions, and can lead to CP violation, where the laws of physics appear to behave differently for particles and their antiparticles.

Anomalous couplings can be studied experimentally by colliding particles at high energies and observing the resulting interactions. By carefully measuring the properties of the final state particles, such as their energies, momenta, and spin, physicists can infer the presence and strength of anomalous couplings. These measurements can help test the predictions of the Standard Model and search for evidence of new physics beyond it.

![[Pasted image 20230401220511.png]]

SUSY can solve mass hierarchy problem.
![[Pasted image 20230401220831.png]]



GIM mechanism  and Interference :

Interference occurs when two or more Feynman diagrams contribute to the same final state of a particle interaction. The probability amplitude for the overall process is obtained by summing the probability amplitudes of each individual Feynman diagram.

Interference can be constructive or destructive, depending on the relative phases of the probability amplitudes. Constructive interference occurs when the probability amplitudes have the same phase and reinforce each other, leading to an enhanced overall amplitude. Destructive interference, on the other hand, occurs when the probability amplitudes have opposite phases and tend to cancel each other out, resulting in a reduced overall amplitude.

In the context of the GIM mechanism, interference refers to the interference between different quark mixing pathways or Feynman diagrams involving the charm quark. These pathways represent different possibilities for the flavor-changing transition to occur. The interference arises because the charm quark can propagate through multiple pathways, contributing to the overall amplitude.

By considering the interference effects between the different pathways, we can observe cancellations or enhancements in the overall probability amplitude for the flavor-changing process. In the case of the GIM mechanism, the destructive interference between specific mixing pathways involving the charm quark leads to a suppression of Flavor Changing Neutral Current (FCNC) processes. The interference effects depend on the masses and couplings of the particles involved in the processes.

The GIM mechanism introduces the charm quark as an additional quark to cancel out unwanted FCNC effects. The charm quark's mass is indeed lighter than the W boson mass, but that is not the primary reason for its inclusion in the mechanism.

The interference between different quark mixing pathways, involving both the charm quark and the W boson exchange, is what leads to the suppression of FCNC processes. The interference effects depend on the masses and couplings of the particles involved, as well as the relative phases of the probability amplitudes associated with the different pathways.

The charm quark plays a crucial role in the GIM mechanism because its presence introduces additional pathways that interfere with the direct FCNC transitions mediated by the W boson. Through interference, these pathways contribute in a way that cancels out the FCNC effects, leading to the suppression of FCNC processes.

![[Pasted image 20230620135716.png]]

Buffer !

So FCNC is rare because :
1. GIM Mechanism: The Glashow-Iliopoulos-Maiani (GIM) mechanism, as we discussed earlier, plays a crucial role in suppressing FCNC processes. The interference effects between different quark mixing pathways, mediated by the GIM mechanism, lead to a cancellation or significant reduction of FCNC amplitudes.
    
2. Small Mixing Angles: The CKM matrix, which governs quark flavor mixing, contains small mixing angles. These angles represent the relative strengths of flavor-changing transitions. The small values of these mixing angles contribute to the suppression of FCNC processes, making them relatively rare compared to other interactions.
    
3. Loop Suppression: FCNC processes typically involve loop diagrams, which involve virtual particles running in loops. Loop processes are generally less likely to occur compared to tree-level processes due to the additional suppression factor associated with loop diagrams.
    
4. Weak Interaction Strength: The weak interaction itself is relatively weak compared to electromagnetic and strong interactions. This inherent weakness of the weak interaction contributes to the rarity of FCNC processes.



<mark style="background: #FFF3A3A6;">**While off-shell particles, which are virtual particles that can temporarily violate the mass-energy relation, can appear in intermediate states of Feynman diagrams, they still obey energy-momentum conservation laws when summed over all possible intermediate states.**
</mark>


### How are they all related after all?
1. Flavor Changing Neutral Current (FCNC): FCNC refers to processes in particle physics where a quark changes its flavor (type) without changing its electric charge. FCNC processes are highly suppressed in the Standard Model due to the Glashow-Iliopoulos-Maiani (GIM) mechanism.
    
2. Charged Lepton Flavor Violation (CLFV): CLFV refers to processes in which charged leptons (such as electrons or muons) change their flavor, violating the conservation of lepton flavor. CLFV is not allowed in the Standard Model but can occur in some theories beyond it.
    
3. GIM Mechanism: The GIM mechanism is a theoretical framework developed by Glashow, Iliopoulos, and Maiani. It introduces additional quark mixing pathways involving the charm quark to cancel out unwanted FCNC effects. The GIM mechanism achieves this through interference effects between different quark mixing pathways.
    
4. Charm Quark: The charm quark is the third lightest quark in the Standard Model, denoted as c. It plays a crucial role in the GIM mechanism by introducing additional quark mixing pathways that interfere with FCNC transitions. The presence of the charm quark helps suppress FCNC processes and ensures agreement with experimental observations.
    
5. Mass Suppression: Mass suppression refers to the reduction or suppression of FCNC processes due to interference effects between different quark mixing pathways. In the GIM mechanism, destructive interference between specific pathways involving the charm quark cancels out or reduces the contributions of FCNC processes, leading to their suppression.
    

These topics are interconnected, as the GIM mechanism, charm quark, and interference effects are all relevant to understanding and suppressing FCNC processes in particle physics. Additionally, CLFV processes, which involve violations of lepton flavor conservation, provide valuable insights into physics beyond the Standard Model.


[[Detector ]]

# Cross sections
In the context of physics, particularly in particle physics experiments, the terms "absolute cross section" and "normalized cross section" refer to different ways of quantifying and presenting experimental measurements.

1. Absolute Cross Section: The absolute cross section represents the likelihood of a specific process or interaction occurring when particles (such as protons or electrons) collide with each other. It is measured in units of area, typically in barns (1 barn = 10^-28 square meters).
    
    Absolute cross section measurements provide the actual probability or rate of a particular interaction occurring, regardless of the experimental conditions or the intensity of the particle beams. These measurements are essential for understanding the underlying physics processes and for comparison with theoretical predictions.
    
2. Normalized Cross Section: The normalized cross section is obtained by dividing the measured cross section by a reference value. The reference value is typically chosen based on certain conditions or assumptions, such as a specific energy range, detector acceptance, or a well-understood process.
    
    Normalized cross section measurements are useful for comparing data across different experiments, colliders, or energy regimes. They help to remove the effects of experimental setup differences and can provide insights into the underlying physical phenomena without being dependent on absolute values.


# Development of PDFs for partons

Parton distribution functions (PDFs) are developed through a combination of theoretical calculations, experimental measurements, and statistical analysis. The construction of PDFs involves a multi-step process that incorporates various data sets and theoretical frameworks. Let's explore the general steps and touch upon the specific cases of NNPDF and CT10/CTEQ PDF sets.

1. Theoretical Framework: PDFs are typically calculated within the framework of Quantum Chromodynamics (QCD), the theory of the strong nuclear force. Perturbative QCD calculations provide the foundation for understanding the dynamics of partons and their interactions.
    
2. Initial Parametrization: An initial parametrization for the PDFs is chosen based on theoretical expectations and insights from previous studies. These parametrizations include functional forms with several free parameters that will be determined through fitting to experimental data.
    
3. Fitting to Data: Experimental data from a wide range of scattering experiments are used to constrain the free parameters of the PDF parametrization. These data sets include deep inelastic scattering, Drell-Yan processes, jet production, and other high-energy scattering processes. The goal is to find the best set of parameters that reproduce the experimental measurements.
    
4. Statistical Analysis: Statistical techniques, such as the method of least squares or maximum likelihood estimation, are employed to determine the best-fit values of the PDF parameters and to estimate the uncertainties associated with them.
    

Now, let's discuss the specific cases of NNPDF and CT10/CTEQ PDF sets:

NNPDF (part of the NNPDF Collaboration): The NNPDF approach uses a neural network methodology to determine the PDFs. Neural networks are trained on a large set of experimental data to directly extract the PDFs without assuming a specific functional form. The neural network framework provides flexibility in capturing complex PDF shapes and allows for a systematic estimation of uncertainties.

CT10/CTEQ (part of the CT Collaboration): The CT10/CTEQ PDF sets are obtained through global fits to experimental data. These fits involve a wide range of data sets and incorporate theoretical calculations within the framework of QCD. The CT10/CTEQ collaborations employ a specific parametrization form and perform iterative fitting procedures to determine the best-fit PDFs and uncertainties.

In both cases, NNPDF and CT10/CTEQ, the construction of PDF sets involves the combination of theoretical calculations, fitting procedures, and statistical analysis. These PDF sets are continuously updated as new data become available, allowing for improved precision and understanding of the proton's internal structure.

https://en.wikipedia.org/wiki/Parton_(particle_physics)#Parton_distribution_functions
https://en.wikipedia.org/wiki/DGLAP_evolution_equations

---
# Bjorken Scaling:
### The Basics:

Deep inelastic scattering experiments involve firing a high-energy lepton (like an electron) at a target proton or neutron. The lepton interacts with the quarks inside the proton or neutron via the exchange of a photon (the force carrier for the electromagnetic force). The goal is to probe the internal structure of the proton or neutron – to "see" the quarks inside.

### The Observation:

When experiments of this nature were conducted, scientists noticed something surprising. When they plotted the cross-section of the scattering as a function of certain variables, they found that the cross-section depended on the energy and momentum transfer but, surprisingly, not on the specific energy of the lepton beam. This energy independence is Bjorken scaling.

### Intuition:

Imagine you're trying to understand the details of a complex machine, like the inner workings of a clock. You could use a magnifying glass (representing low energy) to get a closer look. At low magnifications, you might just see the large gears and components.

However, if you use a microscope (representing high energy), you'll see much finer details, including smaller gears, springs, and perhaps even the texture of the material.

Bjorken scaling is like saying that the pattern or distribution of these details (small gears, springs, etc.) looks remarkably the same, whether you're using a 10x microscope or a 100x microscope. The relative distribution remains consistent.

### Example:

Consider a target proton moving at a very high speed. From the perspective of the incoming lepton, the proton's internal quarks are moving rapidly. As you increase the energy of the lepton beam (akin to increasing the magnification of a microscope), you're probing finer and finer details of the proton's structure.

Bjorken scaling suggests that the distribution of these quarks, when plotted against a certain scaled momentum variable, doesn't change. It's as if, no matter how hard you throw a baseball at a car (with the car representing the proton and the baseball the lepton), the way the baseball bounces off the tires versus the doors versus the windows remains the same. It's quite unexpected!

### Importance:

Bjorken scaling provided the first strong evidence for the parton model of hadrons, where hadrons (like protons and neutrons) are made up of point-like constituents called partons (which we now understand as quarks and gluons). The scaling phenomenon hinted that these partons were not interacting strongly with each other, paving the way for the development of Quantum Chromodynamics (QCD), the theory of the strong force.

---

### Good summary of the analysis process :
[answer](https://physics.stackexchange.com/posts/87218/timeline)

The experiments take many years. Using the Higgs boson search as an example, the reason it takes so long is because there is no "smoking gun" signature of a Higgs boson. You don't search for the Higgs boson directly, but for the Standard Model particles to which the Higgs decays. Since other Standard Model processes (called "backgrounds") can produce these particles, for any given collision at the LHC you cannot be sure that you have seen the Higgs boson. You have to produce thousands of Higgs bosons before you have a large enough statistical sample from which to draw any conclusions. And even then it can be a difficult process of comparing your observed rate of Higgs-like events to the predicted background rate. So finding the Higgs boson is not trivial; it corresponds to the experimental observation of a Higgs-like rate that is slightly larger than the predicted background rate. Since the background rate prediction has its own set of errors and assumptions, and statistical fluctuations are possible, it takes a long time to create enough Higgs bosons, and understand the detector well enough, to be confident that an observed excess of Higgs-like events is real.

---

# To be read: 
https://en.wikipedia.org/wiki/Category:Experimental_particle_physics
---
# Question about SM:

 Could all of the fundamental forces be of equal strength at very high energy, indicating a potential common origin? Could new, unknown interactions be modifying the strong force in certain processes or at certain energies?

---

#measurement

[[ Measurements and Analysis ]]


#Glossary
Smirnov transform : Smirnov transform of ee -> yy in MC. Used in yy bkg evaluation usually.
(inverse transform to go from pdf to data).

Observables and the significance (coming from h->yy ppr, ):
![[Pasted image 20231003004914.png]]
![[Pasted image 20231003004931.png]]
--

[[ Measurements and Analysis ]]
Also, for continuum bkg, we have :
"The background in the Higgs boson signal extraction fit is modelled analytically. The
functional form chosen for the background model is based on background templates built
using simulations and data control-regions, and these are also used in the estimation of
related systematic uncertainties. "

---

## Can $\sigma$  reduce with reduced cms $\sqrt{s}$  ?
Cross section is a measure of the likelihood of a specific process occurring when particles collide. The cross section typically depends on several factors, including the center-of-mass energy of the collision (often denoted as √s), the nature of the process, and the properties of the particles involved.

For many Standard Model processes, the cross section generally increases as the center-of-mass energy of the collision (√s) increases. This is because higher collision energies provide more available energy to produce massive particles, which may be involved in the process of interest.

However, there are scenarios where the cross section might decrease as the collision energy decreases, but these situations are relatively less common. Here are a couple of cases where this might occur:

1. **Threshold Effects**: Some particle reactions or decays have energy thresholds, below which they cannot occur. If the center-of-mass energy is reduced to a value below this threshold, the cross section for that particular process effectively drops to zero because there is not enough energy available to create the required particles or conditions.
    
2. **Resonance Behavior**: In certain cases, the cross section can exhibit resonance behavior. A resonance occurs when the energy is close to the mass of a specific particle. Near the resonance energy, the cross section can be significantly enhanced. However, as the energy moves away from the resonance, the cross section can drop rapidly.
    
    - For example, the cross section for producing the Z boson in proton-proton collisions at the Large Hadron Collider (LHC) increases as the collision energy approaches the Z boson's mass (about 91 GeV). At higher energies, the cross section decreases because the collision energy is far above the resonance peak.
        
    - Similarly, in electron-positron colliders, the cross section for producing the ϒ (Upsilon) mesons, which are resonances of the bottom quark-antiquark system, has a maximum at a specific energy that corresponds to the ϒ mass. At higher or lower energies, the cross section decreases.


---

---

## NWA
1. **Decay Width (Γ):** The decay width of a particle is a measure of how quickly it decays into other particles. It quantifies the probability of the particle decaying in a given time interval. Particles with a larger decay width are shorter-lived and tend to decay more quickly, while particles with a smaller decay width are longer-lived and decay more slowly.
    

Now, let's explain the narrow width approximation:

- When the decay width (Γ) of a particle is much smaller than its mass (M), it means that the particle is relatively long-lived compared to the time scale of the process being studied.
    
- In this approximation, one can treat the particle as if it were stable for the purposes of certain calculations. This simplification is particularly useful when studying resonance phenomena, where particles temporarily exist in excited states before decaying into other particles.
    
- Mathematically, the narrow width approximation can be expressed as Γ << M. This implies that the particle spends a relatively long time in its excited state before decaying, allowing it to interact with other particles and form a resonance peak in a scattering process.
---


## Why study prompt?
Prompt photons and prompt muons are two examples of such objects:

1. Prompt Photons: A prompt photon refers to a photon that is produced directly from the primary interaction vertex in a particle collision. It is not the result of the decay of other particles. Prompt photons can arise from various processes, such as quark-gluon interactions, annihilation processes, or the decay of other prompt particles. They are often used as a probe to study specific interactions or to search for new phenomena in high-energy collisions.
    
2. Prompt Muons: Similarly, a prompt muon is a muon that is produced directly from the primary interaction vertex. Muons are heavy leptons, and prompt muons can be produced in processes like Drell-Yan production, where a quark and an antiquark annihilate to produce a virtual photon or Z boson, which subsequently decays into a muon-antimuon pair. Prompt muons are crucial in precision measurements, such as the determination of the W boson mass or the search for rare processes.
---

# A map of particle physics 
Creating an extensive map of particle physics topics is a complex endeavor due to the vast scope and intricate history of the field. I'll provide a high-level map of key topics, developments, and experiments in particle physics to give you a broad understanding of its evolution. This map will be divided into several sections:

**Foundations and Early Discoveries (Late 19th and Early 20th Century):**

- **Discovery of the Electron (1897):** J.J. Thomson's experiments led to the discovery of the electron, the first subatomic particle.
- **Development of Quantum Mechanics (1920s):** Pioneered by Schrödinger, Heisenberg, and Dirac, quantum mechanics laid the groundwork for understanding subatomic particles.

**The Rise of the Standard Model (Mid-20th Century):**

- **The Strong Interaction (1950s):** The theory of Quantum Chromodynamics (QCD) emerged to describe the strong nuclear force.
- **Discovery of the Pion (1947):** The first meson was discovered, confirming the existence of these particles.
- **Electroweak Theory (1960s):** Glashow, Salam, and Weinberg proposed the unification of the electromagnetic and weak forces.

**The Higgs Boson and the Standard Model Completion (Late 20th Century - Early 21st Century):**

- **Higgs Mechanism (1964):** Higgs, Brout, and Englert postulated the Higgs field and Higgs boson.
- **LHC and Higgs Discovery (2012):** The Large Hadron Collider (LHC) at CERN discovered the Higgs boson, confirming the last missing piece of the Standard Model.

**Beyond the Standard Model (Late 20th Century - Present):**

- **Grand Unified Theories (GUTs):** Theories attempting to unify forces emerged.
- **Supersymmetry (SUSY):** Postulates the existence of supersymmetric particles (sparticles).
- **String Theory:** An ambitious theory aiming to unify all fundamental forces.
- **Dark Matter and Dark Energy:** Ongoing efforts to understand the nature of these cosmic components.
- **Neutrino Oscillations (2001):** Neutrinos were found to change flavor, implying they have mass.

**Experimental Efforts:**

- **Particle Colliders:** The LHC, Tevatron, and others conducted experiments to probe the fundamental particles.
- **Neutrino Experiments:** Experiments like Super-Kamiokande and IceCube studied neutrinos.
- **Cosmic Ray and Cosmic Microwave Background (CMB) Observations:** These provided insights into the early universe and cosmic ray sources.

**Technological Developments:**

- **Detectors:** Advancements in particle detectors (e.g., silicon detectors, calorimeters, and time-of-flight detectors).
- **Computing:** High-performance computing for data analysis and simulations.
- **Accelerators:** Advances in accelerator technology, such as the LHC.

**Unsolved Mysteries:**

- **Dark Matter:** Its nature remains unknown, with various candidates being explored.
- **Dark Energy:** The cause of the accelerated expansion of the universe is still a mystery.
- **Flavor Physics:** Exploring the properties of quarks and leptons to understand CP violation.
- **Hierarchy Problem:** Why is the Higgs boson's mass so much smaller than expected?
- **Grand Unification:** The quest to unify all fundamental forces.

----


## Nice view of SM by quanta :
https://www.quantamagazine.org/a-new-map-of-the-standard-model-of-particle-physics-20201022/#comments

![[Pasted image 20231019113718.png]]

----

### LLPs : #llp    #measurement 
Long lived particles - something that has caught my attention. Please find more abou it here in this dedicated section : [[LLP]]

----

# BSM Naturalness :
**Naturalness** is the aesthetic property that the dimensionless ratios between free parameters or physical constants appearing in a physical theory should take values "of order 1" and that free parameters are not <span style="color:#00b0f0">fine-tuned.</span> 


----

# SM quantum numbers:
Understanding the relationships between chirality, isospin, helicity, spin, and handedness in the context of fundamental particles can indeed be challenging due to the abstract nature of these concepts. Here’s a breakdown that might help make these concepts more memorable:

1. **Spin**: 
   - Think of it as an intrinsic form of angular momentum that every fundamental particle possesses. It's a quantum property, meaning particles have a fixed spin value (like 1/2 for fermions).

2. **Chirality**:
   - Chirality, or handedness, is a property that does not have a classical analog. It's purely quantum mechanical. For massless particles, chirality is well-defined and corresponds to the direction of the spin relative to the direction of motion. For massive particles, chirality is defined by the particle's wavefunction and is invariant under Lorentz transformation (meaning it doesn't change if you go to a different inertial frame).
   - Remember: Chirality is crucial because it determines how a particle interacts with the weak force. Only left-chiral particles and right-chiral antiparticles interact with the weak force.

3. **Helicity**:
   - Helicity is the spin's projection along the direction of motion. It's like asking whether the particle is spinning clockwise or counterclockwise as it moves along. For a particle moving near the speed of light, if you can overtake it and look back, does the spin seem to be rotating with or against its motion? That's helicity.
   - Note: For massless particles, helicity and chirality are the same because you can't overtake a massless particle (it always moves at the speed of light).

4. **Isospin**:
   - This is a concept inspired by the proton and neutron being almost identical in strong interactions. Isospin is a quantum number that differentiates members of a particle family, like up and down quarks, or protons and neutrons.
   - Think of isospin as a label in a quantum doublet: for up quarks and down quarks, up has isospin +1/2, and down has isospin -1/2.

5. **Weak Isospin**:
   - Weak isospin is similar to isospin but specifically for weak interactions. It's related to chirality: left-chiral particles have weak isospin, while right-chiral particles do not.
   - In the Standard Model, left-chiral fermions are doublets under the weak isospin (they have weak isospin values), and right-chiral fermions are singlets (they don't have weak isospin values).

6. **Handedness**:
   - This term can be confusing because it's used interchangeably with chirality and sometimes with helicity. In general, "handedness" refers to whether a particle is left-chiral or right-chiral.
   - For a simple mnemonic, think: "Left-handed particles shake hands with the weak force; right-handed particles do not."

Remembering the differences can be aided by associating each property with a specific aspect of particle behavior or interaction. You can also think about these properties in pairs: spin is a fundamental characteristic like the particle's eye color, while chirality/helicity is more about behavior, like whether they write with their left or right hand. Isospin and weak isospin are about the particle's identity in the context of forces, like different badges they wear in specific scenarios.

---
