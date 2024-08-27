
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


CP violation is a phenomenon in particle physics where the laws of physics are not invariant under the combined operations of charge conjugation (C, which changes particles into their corresponding antiparticles) and parity transformation (P, which flips the spatial coordinates). Observations of CP violation indicate that the laws of nature distinguish between matter and antimatter, and this has profound implications for understanding the asymmetry between matter and antimatter in the universe.

One of the most compelling evidences of CP violation comes from the study of decays of B mesons, which are hadrons containing a bottom (or b) quark. The B factories, such as the experiments conducted at Belle (KEKB collider in Japan) and BaBar (PEP-II collider at SLAC in the US), were specifically designed to study CP violation in B meson systems. A classic example of CP violation is observed in the decay of neutral B mesons (\(B^0\) and \(\bar{B}^0\)).

### Example of CP Violation in B Meson Decays:

A well-studied process that exhibits CP violation involves the decay of \(B^0\) and \(\bar{B}^0\) mesons into a pair of charged pions (\(\pi^+\) and \(\pi^-\)). The \(B^0\) meson contains a bottom quark (\(b\)) and a down antiquark (\(\bar{d}\)), while its antiparticle, \(\bar{B}^0\), contains a bottom antiquark (\(\bar{b}\)) and a down quark (\(d\)).

The decay can proceed through several paths, including direct decay or decay after mixing. Mixing occurs when a \(B^0\) meson oscillates into its antiparticle \(\bar{B}^0\) before decaying, or vice versa. This mixing is a quantum mechanical effect unique to neutral mesons.

1. **Direct Decay**: 
   - $$\(B^0 \to \pi^+ \pi^-\)$$
   - $$\(\bar{B}^0 \to \pi^+ \pi^-\)$$

2. **Decay After Mixing**:
   - $$\(B^0 \to \bar{B}^0 \to \pi^+ \pi^-\)$$
   - $$\(\bar{B}^0 \to B^0 \to \pi^+ \pi^-\)$$

CP violation manifests as a difference in the rate of these processes for \(B^0\) and \(\bar{B}^0\), measured experimentally by comparing the number of \(B^0\) mesons decaying into \(\pi^+ \pi^-\) to the number of \(\bar{B}^0\) mesons decaying into the same final state. If CP symmetry were conserved, these rates would be identical. However, experiments have observed a difference, indicating CP violation.

### The Importance of the CP Violation Measurement:

The measurement of CP violation in B meson decays, particularly in processes like the one described, has been a critical test of the Standard Model of particle physics. The phenomenon of CP violation is incorporated into the Standard Model through the complex phase in the CKM (Cabibbo-Kobayashi-Maskawa) matrix, which describes quark mixing. The observations of CP violation in B meson decays have been in agreement with the predictions of the Standard Model, providing a powerful confirmation of its validity.

Furthermore, the study of CP violation helps to address one of the fundamental questions in cosmology: why the universe is composed predominantly of matter rather than an equal mixture of matter and antimatter. CP violation is a necessary condition for generating the matter-antimatter asymmetry in the early universe, according to the criteria outlined by Andrei Sakharov in 1967. However, the degree of CP violation observed in particle physics experiments to date is not sufficient to explain the current matter-antimatter asymmetry, suggesting that additional sources of CP violation may exist beyond the Standard Model.


The weak mixing angle, often denoted as \(\sin^2 \theta_W\), is a fundamental parameter in the Standard Model of particle physics that describes the mixing of the electromagnetic and weak forces. Here's how it's measured and its relation to parity violation:

## Measurement of the Weak Mixing Angle

#### Methods of Measurement
1. **Deep Inelastic Scattering**: Experiments like those at the SLAC (Stanford Linear Accelerator Center) involve scattering high-energy electrons off protons or neutrons. The differential cross-sections for neutral current interactions provide information about \(\sin^2 \theta_W\).
   
2. **Z Boson Properties**: Precision measurements at particle colliders, such as the LEP (Large Electron-Positron Collider) at CERN, where the properties of the Z boson (mass, width, and decay modes) are studied. The ratio of neutral current to charged current processes also gives \(\sin^2 \theta_W\).

3. **Parity-Violating Electron Scattering**: Experiments like the P2 experiment at JGU Mainz measure parity-violating asymmetries in electron scattering. The weak mixing angle can be extracted from the degree of parity violation observed.

4. **Atomic Parity Violation (APV)**: Precision measurements of parity-violating effects in atoms, where the interaction of electrons with the nucleus is affected by the weak force, also contribute to determining \(\sin^2 \theta_W\).

### Relation to Parity Violation

#### Parity Violation in the Weak Interaction
- **Weak Force and Parity**: The weak force is unique among the fundamental forces because it violates parity (P) symmetry, meaning it distinguishes between left-handed and right-handed coordinate systems.
  
- **Neutral Current Interactions**: Parity violation in neutral current interactions (mediated by the Z boson) provides a way to measure the weak mixing angle. The degree of parity violation observed in these processes is directly related to the value of \(\sin^2 \theta_W\).

#### Parity-Violating Asymmetry
- **Asymmetry Measurement**: In parity-violating electron scattering experiments, the asymmetry \(A_{PV}\) is measured, which is the difference in cross-sections for left-handed versus right-handed polarized electron beams.
  \[
  A_{PV} = \frac{\sigma_L - \sigma_R}{\sigma_L + \sigma_R}
  \]
  where \(\sigma_L\) and \(\sigma_R\) are the cross-sections for left-handed and right-handed electrons, respectively.

- **Dependence on \(\sin^2 \theta_W\)**: The parity-violating asymmetry is sensitive to the weak mixing angle, and precise measurements of \(A_{PV}\) allow for an accurate determination of \(\sin^2 \theta_W\).

### Example: P2 Experiment
- **Objective**: The P2 experiment aims to measure the weak mixing angle by examining parity-violating asymmetries in electron-electron (Møller) scattering.
  
- **Procedure**: Longitudinally polarized electrons are scattered off unpolarized electrons, and the parity-violating asymmetry in the scattering cross-section is measured. The degree of asymmetry provides a direct measurement of \(\sin^2 \theta_W\).

### Summary
- **Weak Mixing Angle**: A crucial parameter in the Standard Model, describing the mixing of the electromagnetic and weak forces.
- **Parity Violation**: The weak force's violation of parity symmetry allows for precise measurements of \(\sin^2 \theta_W\) through various experimental methods.
- **Experimental Relevance**: Parity-violating electron scattering, such as in the P2 experiment, provides a direct way to measure \(\sin^2 \theta_W\) by observing the asymmetry in scattering cross-sections for different polarizations.

These measurements are essential for testing the Standard Model and searching for possible signs of new physics beyond the Standard Model.


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


# QCD - p or not:
**Perturbative Quantum Chromodynamics (pQCD):**

**Application:**
- pQCD is applied in scenarios where the strong coupling constant is small, typically at high energy scales (due to asymptotic freedom). This includes processes like high-energy particle collisions where quarks and gluons are involved.

**Strengths:**
- Predictive Power: Provides precise predictions for processes at high energies where the coupling is weak.
- Tested by Experiments: Many predictions of pQCD have been confirmed by experiments, especially in collider physics.
- Calculational Framework: Allows systematic calculations using Feynman diagrams and renormalization techniques.

**Shortcomings:**
- Limited to High Energies: Not effective at low energy scales where the strong force becomes too strong (non-perturbative).
- Infrared Divergences: Issues arise in calculations at low momenta, requiring careful handling.
- Complexity: Calculations can become extremely complex at higher orders.

**Non-perturbative Quantum Chromodynamics (non-pQCD):**

**Application:**
- Non-pQCD is necessary at low energy scales where the strong coupling constant is large, like in the study of hadron structure, quark-gluon plasma, and nuclear forces.

**Strengths:**
- Applicable to Low Energies: Essential for understanding phenomena where the strong force is strong, such as hadronization and confinement.
- Rich Phenomenology: Provides insights into complex phenomena not accessible to pQCD.

**Shortcomings:**
- Lack of a Systematic Calculational Framework: Unlike pQCD, it doesn’t have a universally applicable mathematical framework like Feynman diagrams.
- Reliance on Models and Numerical Methods: Often depends on phenomenological models or numerical simulations (like lattice QCD), which may have their own limitations.
- Computational Intensity: Techniques like lattice QCD require significant computational resources.

In summary, pQCD excels in high-energy regimes where the strong force is weak and allows for perturbative methods. In contrast, non-pQCD is vital for understanding low-energy strong interactions but often relies on less precise or computationally intensive methods.

----


# Spin:
The spin of a particle in quantum mechanics is a fundamental property like its mass or charge. It's a form of angular momentum, but unlike the familiar angular momentum from classical physics (which arises from an object's rotation), spin is an intrinsic property of a particle, meaning it's a built-in feature of the particle's identity.

1. **Photon's Spin 1:**
   - Photons, which are the quantum particles of light, have a spin of 1. This classifies them as "vector bosons."
   - Spin 1 implies that photons can have three polarization states. Unlike particles with half-integer spins (like electrons, which have spin 1/2 and can only be spin up or spin down), photons can be left-circularly polarized, right-circularly polarized, or linearly polarized.
   - This property of photons is deeply connected with their role as force carriers of the electromagnetic force in quantum field theory.

2. **Higgs Boson's Spin 0:**
   - The Higgs boson, discovered at the Large Hadron Collider in 2012, has a spin of 0.
   - A spin of 0 classifies it as a "scalar boson." This means the Higgs boson does not have any intrinsic angular momentum.
   - Being a scalar boson, the Higgs does not have any directionality associated with it, which is consistent with its role in providing mass to other particles through the Higgs mechanism.

**Stern-Gerlach Experiment:**
   - The Stern-Gerlach experiment is famous for demonstrating the quantization of angular momentum. In its classical form, it involves passing a beam of particles through a non-uniform magnetic field and observing their deflection.
   - If you were to pass photons through a Stern-Gerlach apparatus, you wouldn't observe any splitting based on their spin. This is because the experiment is designed to measure magnetic moments of particles, and photons, being neutral and having no magnetic moment, are not affected by the magnetic field in the apparatus.
   - Similarly, the Higgs boson, with a spin of 0, would not be expected to show any splitting in a Stern-Gerlach experiment. Moreover, the Higgs boson is extremely short-lived and would decay before it could be manipulated in such an experiment.

In conclusion, the spin values of particles like the photon and the Higgs boson are essential for understanding their behavior and interactions in the realm of quantum mechanics and particle physics. However, the Stern-Gerlach experiment is not a suitable method to probe the properties of these particular particles.

## Light polarizations:
Photon polarization describes the oscillation direction of the electromagnetic field associated with the photon. Since photons are quanta of light, which is an electromagnetic wave, their polarization refers to the orientation of the electric field vector. The different types of polarization - left-circular, right-circular, and linear - describe the various ways this vector can behave in space over time as the photon travels.

1. **Linear Polarization:**
   - In linear polarization, the electric field of the photon oscillates in a single plane as it moves forward. Imagine the electric field as a straight line that swings back and forth in a fixed direction while the photon travels along its path. This is the simplest form of polarization.
   - Linear polarization is often described by the angle that this plane makes with a reference axis. For example, you might have vertically or horizontally polarized light, depending on the direction of the electric field oscillation.

2. **Circular Polarization:**
   - Circular polarization is more complex. Here, the electric field of the photon rotates in a circle around the direction of motion. This rotation can occur in two ways, giving rise to left-circular and right-circular polarization.
   - In left-circular polarization, if you were to look at the photon coming towards you, the electric field would rotate counterclockwise. Conversely, in right-circular polarization, it would rotate clockwise.
   - This circular motion of the electric field vector creates a helical pattern in space. The direction of this helix (left-handed or right-handed) determines whether the polarization is left-circular or right-circular.

3. **Elliptical Polarization:**
   - As an additional note, there's also elliptical polarization, which is a general form encompassing linear and circular polarizations. In elliptical polarization, the tip of the electric field vector traces out an ellipse in the plane perpendicular to the direction of propagation.

The polarization of a photon is a crucial aspect in various fields of physics and technology. For example, in quantum mechanics, polarization is an essential property in understanding photon entanglement and quantum information. In everyday technology, polarized lenses in sunglasses use the property of linear polarization to reduce glare by blocking certain orientations of light. Circular polarization is significant in areas like 3D movie projection and the transmission of radio waves.



---

![[Pasted image 20231214111903.png]]

From a terascale talk on m_top < https://indico.desy.de/event/41133/contributions/158285/attachments/87444/116796/Presentation.pdf >

---


---

## Dead cone effect:
The "dead cone effect" is a phenomenon observed in particle physics, particularly in the context of the behavior of heavy quarks (like charm and bottom quarks) when they radiate gluons. This effect is a consequence of quantum chromodynamics (QCD), the theory that describes the strong interaction, one of the four fundamental forces in nature.

### Explanation of the Dead Cone Effect:

1. **Gluon Radiation from Quarks**: In QCD, quarks radiate gluons, much like charged particles radiate photons in electromagnetism. This radiation process is an essential aspect of jet formation in high-energy particle collisions.

2. **Mass of the Radiating Quark**: The pattern of this gluon radiation depends on the mass of the radiating quark. For light quarks (like up, down, and strange quarks), the radiation is relatively uniform in all directions. However, for heavy quarks, the situation is different due to their larger mass.

3. **Suppression Near the Quark Direction**: For a heavy quark, there is a suppression of gluon radiation at small angles relative to the direction of the quark's motion. This suppression creates a region with reduced gluon radiation, known as the "dead cone."

4. **Angle of the Dead Cone**: The size of the dead cone (i.e., the angular region around the heavy quark where gluon radiation is suppressed) is inversely proportional to the mass of the quark. The heavier the quark, the larger the mass, and thus, the smaller the angle of the dead cone.

### Importance in Particle Physics:

- **Jet Structure Analysis**: The dead cone effect is important in the analysis of jets produced in high-energy collisions, such as those in the Large Hadron Collider (LHC). It provides a way to distinguish between jets initiated by heavy quarks and those initiated by light quarks or gluons.
- **Testing QCD Predictions**: Observing and measuring the dead cone effect serves as a test of QCD, particularly its predictions regarding the behavior of heavy quarks.
- **Identifying Heavy Quark Jets**: In practical terms, the dead cone effect can be used as a tool to identify jets that originate from heavy quarks, which is important in many analyses searching for new physics beyond the Standard Model.

In summary, the dead cone effect is a unique signature in the pattern of gluon radiation from heavy quarks, and it plays a significant role in our understanding of strong interactions and in the analysis of experimental data in particle physics.

![[Pasted image 20240111145508.png]]

---


# CP Violation link :
https://www.britannica.com/science/Pauli-exclusion-principle


----


# Basics of QFT:
Quantum Field Theory (QFT) is a fundamental framework in theoretical physics that combines classical field theory, special relativity, and quantum mechanics to describe the interactions of particles. It plays a crucial role in understanding the fundamental forces of nature, including electromagnetism, weak and strong nuclear forces, and theorizing about gravity. Here are the basic principles of QFT:

1. **Quantization of Fields:** Unlike classical physics, which treats particles as distinct entities and fields as continuous, <mark style="background: #FFB8EBA6;">QFT quantizes both matter and force fields</mark>. Fields are viewed as the fundamental entities, with particles arising as excitations or quanta of these fields.

2. **Wave-Particle Duality:** Consistent with quantum mechanics, QFT embraces the principle that particles exhibit both wave-like and particle-like properties. This duality is encapsulated in the behavior of field quanta.

3. **Special Relativity:** QFT incorporates the principles of special relativity, ensuring that the theory respects the invariance of the speed of light and the laws of physics in all inertial frames. This leads to a consistent description of particles moving at or near the speed of light.

4. **Local Interactions:** Interactions in QFT are local, meaning that particles interact at specific points in space and time. This principle is crucial for the causality and locality in the theory, ensuring that effects cannot propagate faster than the speed of light.

5. **Gauge Symmetry:** A central concept in QFT is gauge symmetry, which underlies the Standard Model of particle physics. Gauge symmetry refers to the invariance of the laws of physics under certain continuous transformations. It leads to the prediction of gauge bosons, the carriers of fundamental forces.
   
```Symmetry:
Here's what gauge bosons actually preserve:
- 1. **Gauge Invariance:** Gauge bosons preserve gauge invariance, which means that the physical laws remain unchanged (invariant) under certain types of transformations. These transformations are called "gauge transformations," and they can be thought of as changes that you can make in the mathematical description of a system without altering its physical state or observable phenomena.    
- 2. **Force Interaction:** Each type of gauge boson is associated with a specific fundamental force and preserves the symmetry that corresponds to that force. By mediating interactions, gauge bosons ensure that the conservation laws associated with these symmetries are upheld. Specifically:    
  - **Photon (γγ)**: The gauge boson for electromagnetism, preserving U(1) gauge symmetry. It mediates the electromagnetic force between charged particles, ensuring the conservation of electric charge.       
  - **W and Z Bosons**: These gauge bosons are responsible for the weak nuclear force, associated with the SU(2) gauge symmetry. They play a crucial role in processes like nuclear fusion in stars and radioactive decay, ensuring the conservation laws related to weak charge (weak isospin) are upheld.       
  - **Gluons (gg)**: The carriers of the strong nuclear force, associated with the SU(3) gauge symmetry of quantum chromodynamics (QCD). Gluons mediate the interactions between quarks inside hadrons (like protons and neutrons), preserving the conservation of color charge.      
  - **Graviton (hypothetical)**: If gravity can be described by a gauge theory (an ongoing area of research), the graviton would be the gauge boson for gravity, associated with the symmetry of general covariance in the theory of general relativity. It would mediate gravitational interactions, ensuring the conservation of energy-momentum.

```


6. **Renormalization:** Many QFT calculations initially result in infinite quantities. Renormalization is a process that systematically removes these infinities to yield finite, physically meaningful results. It is essential for making accurate predictions in quantum electrodynamics (QED) and other field theories.

7. **Feynman Diagrams:** Developed by Richard Feynman, these diagrams provide a visual representation of the interactions between particles in spacetime, simplifying the calculation of probabilities for complex interactions.

8. **Quantum Entanglement:** QFT also predicts quantum entanglement, a phenomenon where particles become correlated in ways that are not possible classically, reflecting a deep and non-intuitive aspect of quantum reality.

9. **Spontaneous Symmetry Breaking:** This principle explains how symmetries in the laws of physics can appear to be broken in lower-energy states, leading to phenomena such as the Higgs mechanism, which gives particles mass.

10. **Unification of Forces:** One of the goals of QFT is to unify the different fundamental forces into a single framework. While it has been successful for electromagnetism, weak, and strong nuclear forces (via the Standard Model), incorporating gravity remains an open challenge.


---


# Mixing:

In the context of particle physics, "mixing" refers to the phenomenon where quantum states of particles, such as quarks or neutrinos, are not the same as their mass eigenstates, leading to a probability of one type of particle transforming into another over time. This concept is crucial for understanding many aspects of particle interactions, especially those involving the weak force. Let's break down some of the key concepts:

### 1. Quark Mixing and the CKM Matrix

Quark mixing occurs because the weak interaction eigenstates (the states that participate in weak interactions) are not aligned with the mass eigenstates (the states with definite mass). This is described by the Cabibbo-Kobayashi-Maskawa (CKM) matrix, a mathematical framework that predicts the likelihood of one type of quark transforming into another through the weak interaction. For example, a down quark in a proton could, during a weak interaction, transform into an up quark, turning the proton into a neutron.

The CKM matrix is a unitary matrix that contains complex elements, each representing the probability amplitude for a transition between quark flavors. The existence of these off-diagonal elements in the matrix signifies quark mixing, which is fundamental to processes such as beta decay and the generation of the matter-antimatter asymmetry in the universe.

### 2. Weak Mixing Angle (Weinberg Angle)

The weak mixing angle, also known as the Weinberg angle, is a parameter in the electroweak theory of the Standard Model that measures the mixing between the electromagnetic and weak forces. It defines the relationship between the W and Z bosons (the carriers of the weak force) and the photon (the carrier of the electromagnetic force). This angle determines the strength of the weak force and plays a crucial role in predicting the outcomes of various particle interactions involving the weak interaction.

The physical manifestation of this mixing can be seen in processes such as the decay of subatomic particles, where the weak mixing angle influences the decay rates and the patterns of particle production.

### 3. Neutrino Oscillations

A similar concept of mixing occurs for neutrinos, known as neutrino oscillations, described by the Pontecorvo-Maki-Nakagawa-Sakata (PMNS) matrix. Neutrinos are produced in specific flavor states (electron, muon, or tau neutrinos), but as they travel, they can oscillate between these flavors. This phenomenon implies that neutrinos have mass and that the flavor eigenstates are superpositions of the mass eigenstates. Neutrino oscillations are a direct consequence of mixing and have been experimentally observed, providing key insights into the properties of neutrinos and their role in the universe.

### Physical Implication

The concept of mixing in particle physics has profound implications, revealing the fundamental interconnectedness of particle states and forces at the quantum level. It challenges the classical notion of particles having fixed identities, showcasing the fluidity and dynamism of quantum states. Through the study of mixing, physicists have deepened their understanding of the weak interaction, CP violation (a difference in the behavior of particles and antiparticles), and the generation of mass for fundamental particles via the Higgs mechanism. These insights are essential for both explaining the observed phenomena in the universe and guiding the search for new physics beyond the Standard Model.

If the mass eigenstates align with the quantum states (flavor eigenstates) of particles, it means that the particles do not mix and there is no transformation between different flavors (or types) of that particle due to quantum mechanical effects. This scenario simplifies the understanding of particle interactions, as each particle type remains distinct and does not oscillate into another type over time. In particle physics, the alignment of mass eigenstates with quantum states means that the probability matrix (like the CKM matrix for quarks or the PMNS matrix for neutrinos) becomes an identity matrix, indicating no mixing and thus no oscillations between different flavors.

### Examples in Particle Physics:

#### 1. Photon
One of the simplest examples is the photon, the quantum of light and carrier of the electromagnetic force. Photons are massless particles and do not have different flavor states that could mix. Their quantum state is aligned with their "mass" eigenstate (though they are massless), meaning there's no concept of mixing or oscillations for photons.

#### 2. Gluons
Gluons are the force carriers of the strong nuclear force, responsible for holding quarks together inside protons, neutrons, and other hadrons. Gluons themselves come in eight types due to the color charge in quantum chromodynamics (QCD), but these types do not mix in the same way as the flavor eigenstates of quarks or neutrinos. Their behavior and interactions are dictated by the rules of QCD, and while they exhibit complex interactions like color confinement and gluon self-interaction, they do not have a mixing matrix like the CKM or PMNS matrices for quarks and neutrinos.

#### 3. Electron, Muon, and Tau (without Neutrino Mixing)
In a hypothetical world where neutrino masses were exactly aligned with their flavor states (electron neutrino with the electron, muon neutrino with the muon, etc.), there would be no neutrino oscillations. This would mean that an electron neutrino, for example, would always interact as an electron neutrino and could not be observed as a muon or tau neutrino at a later time. However, in reality, neutrino oscillation experiments have shown that neutrinos do indeed mix and oscillate between flavors, indicating that their mass eigenstates are not aligned with their flavor states.

### Physical Consequences
The alignment of mass and quantum states significantly affects the predictions and interpretations of particle physics. Mixing and oscillations provide crucial insights into the properties of particles, such as mass differences and the presence of CP violation. Without these phenomena, the understanding of particle mass hierarchies, flavor dynamics, and the asymmetry between matter and antimatter in the universe would be fundamentally different. The study of these mixing and oscillation effects has been central to many breakthroughs in particle physics, including the discovery of neutrino mass and the study of CP violation in the quark sector.

---
# No 4th gen:
The question of whether there is a fourth generation of fundamental particles is intriguing and has been explored through both theoretical considerations and experimental searches. As of the current understanding, several lines of evidence from particle physics experiments, particularly those involving the properties of the Higgs boson and precision measurements of the Standard Model parameters, suggest that a fourth generation of standard fermions (quarks and leptons) is highly unlikely. Here are some of the key arguments:

### 1. **Higgs Boson Production and Decay Rates**

The discovery of the Higgs boson at the Large Hadron Collider (LHC) provided critical insights into the structure of the Standard Model. The Higgs boson production and decay rates observed are consistent with the predictions of the Standard Model with three generations of fermions.

- **Enhanced Higgs Production**: A fourth generation would significantly enhance the production rate of the Higgs boson through gluon fusion, due to the additional heavy quarks. This enhanced rate has not been observed.
- **Higgs Decay into Photons**: The presence of a fourth generation would also affect the Higgs decay into two photons. The rate of this decay process, which is sensitive to loops of charged particles, including hypothetical heavy quarks and leptons, is consistent with three generations.

### 2. **Electroweak Precision Tests**

Electroweak precision tests involve measurements of the properties of the W and Z bosons (mass, width, and couplings to fermions) and other electroweak processes at high precision. These measurements are sensitive to the effects of virtual particles in quantum loops, and thus to the number of fermion generations.

- **Z Boson Width**: The decay width of the Z boson, measured very precisely, agrees with the predictions for three generations of neutrinos. A fourth generation of light neutrinos (with mass less than half the Z boson mass) would have increased the Z boson's decay width significantly, which is not observed.
- **Global Fits to the Standard Model**: Global fits of the electroweak precision data, which include a wide range of measurements, show excellent agreement with the predictions of the Standard Model with three generations. Adding a fourth generation would disturb this agreement, particularly because of the modifications it would imply for the loop corrections in various processes.

### 3. **Direct Searches**

Direct searches for fourth-generation quarks and leptons have been conducted at particle accelerators, including the LHC. No evidence has been found for the existence of such particles up to the highest masses explored by current experiments.

### 4. **Theoretical Considerations**

- **Stability of the Higgs Potential**: Theoretical studies suggest that the addition of a fourth generation could make the Higgs potential unstable at energies not much higher than the electroweak scale unless new physics comes into play.
- **Yukawa Couplings**: The Yukawa couplings of the fourth-generation fermions to the Higgs boson would have to be very large to account for their heavy masses, which leads to potential issues with perturbativity and vacuum stability.

----


# UV incompleteness of SM:

The Standard Model of particle physics, while highly successful in describing the fundamental particles and their interactions, is considered incomplete and does face issues with ultraviolet (UV) divergences.

1. **UV Incompleteness**: The Standard Model is deemed incomplete because it does not incorporate gravity at the quantum level. Gravity is described by general relativity, a classical theory, and integrating it into the quantum mechanics framework of the Standard Model remains a significant challenge. Additionally, the Standard Model does not explain dark matter, dark energy, or the matter-antimatter asymmetry in the universe, all of which are observations that the model does not account for.

2. **UV Divergences**: In terms of UV divergences, these occur in quantum field theories, including the Standard Model, when certain integrals over all possible energy scales lead to infinite results. These infinities appear in the calculations of various physical quantities, making them seemingly nonsensical without further intervention. However, a technique called renormalization is used to handle these divergences. By this method, the parameters of the theory (like masses and coupling constants) are adjusted to absorb these infinities, resulting in finite predictions that agree remarkably well with experimental data.

Thus, the Standard Model is both incomplete in its description of the universe and involves dealing with UV divergences through renormalization techniques. The search for a more complete theory, such as theories of quantum gravity or various extensions of the Standard Model like supersymmetry, continues to be a vibrant field of research in theoretical physics.

"UV" refers to "ultraviolet divergences," which is a technical term unrelated to the ultraviolet light in the electromagnetic spectrum. It refers instead to<mark style="background: #ABF7F7A6;"> problems in the mathematics of quantum field theories that arise at very high energy scales</mark> (short distances), metaphorically similar to the ultraviolet end of the spectrum which corresponds to high energy and short wavelengths in light.

**UV incompleteness** in particle physics, particularly in relation to gravity, means that the current theories, like the Standard Model, do not effectively handle the physics at these very high energy scales where gravitational effects become significant on quantum scales.

Gravity's role in this is crucial because:

1. **Quantum Gravity**: At extremely small scales, on the order of the Planck length (about \(10^{-35}\) meters), quantum effects of gravity are expected to become significant. The Standard Model does not include gravity in its framework, and at these scales, it is believed that a theory of quantum gravity would be required to properly describe interactions.

2. **Renormalization Issues**: In most parts of the Standard Model, divergences (infinite results) that appear in calculations can be managed by the process of renormalization. However, gravity, when attempted to be incorporated in a similar quantum field theoretical framework, leads to non-renormalizable divergences. This means that if gravity is treated like other forces within the quantum field theory, the infinity problems become unmanageable under the current renormalization techniques.

So, when discussing UV incompleteness in relation to gravity, it refers to the theoretical limitation where at very small (ultraviolet) scales, the current models (like the Standard Model) fail to account for gravitational effects and cannot predict phenomena accurately due to these unmanageable infinities. This is one of the reasons why physicists are searching for a unified theory, like string theory or loop quantum gravity, which hopes to integrate gravity with the quantum framework effectively.

----

# CP violation 

CP violation refers to the phenomenon where the laws of physics change when particles are replaced with their antiparticles (charge conjugation, C) and their spatial coordinates are inverted (parity transformation, P). This concept plays a crucial role in explaining why there is more matter than antimatter in the universe.

### Why Was CP Violation Proposed?

1. **Matter-Antimatter Asymmetry**:
   - One of the major unsolved problems in cosmology is the observed dominance of matter over antimatter in the universe. According to the Big Bang theory, matter and antimatter should have been created in equal amounts. However, if that were the case, they would have annihilated each other, leaving behind only radiation. The fact that the universe is filled with matter suggests an asymmetry in the laws governing particles and antiparticles.

2. **Sakharov Conditions**:
   - In 1967, Andrei Sakharov outlined three necessary conditions for baryogenesis (the process that produced an excess of baryons over antibaryons in the early universe):
     - Baryon number violation.
     - C and CP violation.
     - Departure from thermal equilibrium.
   - CP violation is essential because it allows processes that distinguish between matter and antimatter, leading to the observed asymmetry.

### Historical Context and Theoretical Development

1. **Parity Violation**:
   - In 1956, theoretical physicists Tsung-Dao Lee and Chen-Ning Yang proposed that parity (P) might not be conserved in weak interactions. This was a radical idea because parity conservation was assumed to be a fundamental symmetry of nature.

2. **Madame Wu's Experiment**:
   - In 1956-57, Chien-Shiung Wu conducted an experiment involving the beta decay of cobalt-60. She and her team found that parity was indeed violated in weak interactions, confirming the theoretical predictions of Lee and Yang. This discovery earned Lee and Yang the Nobel Prize in Physics in 1957.

3. **CP Violation Prediction**:
   - After the discovery of parity violation, physicists began to question whether the combined symmetry of charge conjugation (C) and parity (P) might also be violated. In 1964, James Cronin and Val Fitch conducted experiments with neutral kaons (a type of meson) and observed CP violation. This discovery provided the first experimental evidence that CP symmetry is not conserved in certain weak interactions.

### Experimental Evidence and Importance

1. **Cronin and Fitch Experiment**:
   - Cronin and Fitch's 1964 experiment with neutral kaons demonstrated that the decay rates of kaons and antikaons were not identical, thus providing clear evidence of CP violation. This work earned them the Nobel Prize in Physics in 1980.

2. **Further Studies**:
   - Subsequent experiments have confirmed CP violation in other systems, such as B mesons. The study of CP violation has become an important part of particle physics, influencing the development of the Standard Model.

3. **Implications for Cosmology**:
   - CP violation is a critical ingredient in explaining the matter-antimatter asymmetry of the universe. Without CP violation, it would be impossible to account for the predominance of matter over antimatter.

### Summary

CP violation was proposed to address the problem of matter-antimatter asymmetry in the universe and was predicted as a necessary condition for baryogenesis. It was first experimentally observed by Cronin and Fitch in 1964, not by Chien-Shiung Wu, who earlier demonstrated parity violation. CP violation remains a fundamental aspect of particle physics and cosmology, helping to explain why the universe is composed predominantly of matter.

----


# Mass hierarchy problem:

### The Mass Hierarchy Problem Explained

The mass hierarchy problem is a significant issue in particle physics related to the vast difference in the masses of elementary particles, particularly focusing on the Higgs boson and other particles. Let's break down the problem in a detailed yet simple manner:

#### What is the Mass Hierarchy Problem?

1. **Elementary Particles and the Higgs Boson**:
   - **Elementary particles**: Fundamental particles like quarks, leptons (e.g., electrons, neutrinos), and gauge bosons (e.g., photons, W and Z bosons).
   - **Higgs boson**: A particle associated with the Higgs field, responsible for giving mass to other elementary particles through the Higgs mechanism.

2. **Hierarchy of Masses**:
   - In the Standard Model of particle physics, particle masses vary widely. For example, the electron is much lighter than the top quark, and the Higgs boson has a mass around 125 GeV (giga-electron volts).
   - The **Planck scale** (about \(10^{19}\) GeV) is a fundamental energy scale related to gravity, many orders of magnitude larger than the mass of the Higgs boson.

3. **The Core Issue**:
   - The mass of the Higgs boson should be subject to quantum corrections from interactions with other particles.
   - These corrections tend to be very large, potentially pushing the Higgs mass up to the Planck scale. However, the observed Higgs mass is relatively low (125 GeV).
   - The question arises: **Why is the Higgs boson mass so much lighter than the Planck scale?**

#### Why is This Considered an Issue?

1. **Naturalness Problem**:
   - According to the principle of naturalness, parameters in a theory should not be fine-tuned without a good reason. The large difference between the Higgs mass and the Planck scale suggests an unnatural fine-tuning.

2. **Quantum Corrections**:
   - In quantum field theory, the mass of the Higgs boson receives corrections from loops involving all other particles it interacts with. These corrections can be extremely large.
   - For example, if a particle interacts with the Higgs field, the Higgs boson mass should reflect contributions from the mass of that particle. Heavy particles like the top quark contribute significantly to these corrections.
   - Without some mechanism to counteract these corrections, the Higgs mass would naturally be very large.

3. **Fine-Tuning**:
   - To keep the Higgs mass at the observed value, one must precisely cancel out these large corrections, which seems highly improbable without a deeper reason.
   - This precise cancellation appears to be an unnatural fine-tuning, which many physicists find unsatisfactory.

#### Potential Solutions

1. **Supersymmetry (SUSY)**:
   - Supersymmetry proposes that every Standard Model particle has a corresponding superpartner with different spin characteristics.
   - These superpartners contribute opposite-sign corrections to the Higgs mass, potentially canceling out the large quantum corrections and stabilizing the Higgs mass at a lower value.
   - Despite being an elegant solution, direct experimental evidence for supersymmetry has not yet been found.

2. **Extra Dimensions**:
   - Some theories suggest the existence of extra spatial dimensions beyond the familiar three.
   - These extra dimensions could alter the effective scale at which gravity operates, potentially lowering the Planck scale and mitigating the hierarchy problem.

3. **Composite Higgs Models**:
   - In these models, the Higgs boson is not a fundamental particle but a composite of other, more fundamental particles.
   - This compositeness could explain why the Higgs mass is naturally lighter than expected.

4. **Technicolor**:
   - This is a theory that replaces the Higgs mechanism with a new strong interaction.
   - In technicolor theories, the Higgs boson is a bound state of new fermions, similar to how pions arise from the strong interaction in quantum chromodynamics (QCD).


## Real vs. Virtual Particles

1. **Real Particles**:
   - Real particles are those that we can observe directly and measure in experiments.
   - They satisfy the energy-momentum relation \(E^2 = p^2c^2 + m^2c^4\), meaning they are on-shell (i.e., their mass is well-defined).

2. **Virtual Particles**:
   - Virtual particles are internal particles in Feynman diagrams that exist temporarily during interactions.
   - They do not need to satisfy the energy-momentum relation exactly, meaning they are off-shell.
   - Their masses can deviate from the physical (on-shell) masses of the corresponding real particles.

### Virtual Particles in Loop Corrections

1. **Off-Shell Nature**:
   - Virtual particles can have a range of momenta and energies, which means their effective masses can vary during the interaction.
   - However, the virtual particles contribute to the loop corrections based on their coupling constants and the nature of the interaction.

2. **Effective Contributions**:
   - Even though virtual particles are off-shell, their contributions to loop corrections are influenced by their physical (on-shell) masses because the propagators (terms in the Feynman diagram calculations) still depend on these masses.
   - For example, the contribution of a virtual top quark to the Higgs boson mass correction will be influenced by the top quark's on-shell mass because the propagator involves terms like \(1/(p^2 - m_t^2)\), where \(m_t\) is the top quark mass.

### Higgs Mass Corrections and Heavy Particles

1. **Top Quark Contributions**:
   - The top quark has a large physical mass (~173 GeV), and this large mass significantly affects the loop corrections.
   - The heavy mass of the top quark enhances its contribution to the Higgs boson mass correction, even when the top quark is virtual.

2. **Why Heavy Virtual Particles Matter**:
   - The loop integrals that involve virtual top quarks will integrate over a range of momenta, but the integrand will still be heavily influenced by the physical mass of the top quark.
   - The heavier the physical mass of the particle, the larger its contribution to the loop corrections, due to the terms in the propagators and vertices.

### Simplified Picture

- Even though virtual particles are off-shell, the corrections to the Higgs boson mass are computed using integrals that take into account the physical masses of the particles involved.
- The effective mass corrections reflect the influence of these physical masses. For a heavy particle like the top quark, this means it has a large impact on the corrections, making the Higgs boson mass sensitive to the top quark's physical mass.

### Summary

- Virtual particles have undetermined, off-shell masses, but their contributions to loop corrections are influenced by their physical, on-shell masses.
- The heavy physical mass of the top quark leads to significant contributions to the Higgs boson mass correction because the terms in the loop integrals are sensitive to the top quark's mass.
- This is why, despite being virtual and off-shell, the top quark's large mass plays a crucial role in the quantum corrections to the Higgs boson mass.

By considering the above, we recognize that while virtual particles are off-shell, the physical properties of these particles, such as their mass, still play a critical role in determining the magnitude of their contributions to loop corrections. This is a fundamental aspect of quantum field theory and the calculations involved in understanding particle interactions.

----


