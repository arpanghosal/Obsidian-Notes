[[2024-03-18]]
**tty incl. and diff. paper -** 
normalization to xsec?
Normalization involves simulating a large number of events for a specific process, then scaling these simulations down to match the expected number of events based on the theoretical cross section and the specific luminosity of an experiment. This process allows for direct comparison with experimental data, ensuring that the simulations accurately reflect what is observed in real-world conditions.

transverse impact parameter #todo 

how b-tag works?
In ATLAS event reconstructions for analyses, b-tagging is accomplished using the DL1r algorithm, which identifies jets from b-quark hadronization (b-jets). Jets are required to meet specific working points (WPs) that correspond to either 70% or 85% efficiency for b-quark initiated jets, depending on the analysis channel (single-lepton or dilepton). Each jet receives a pseudo-continuous b-tagging score based on how well it meets these WPs, with scores ranging from two to five indicating increasing levels of b-tagging confidence corresponding to 85%, 77%, 70%, and 60% WPs. Jets failing all WPs are given a score of one. This scoring system allows for nuanced utilization of b-tagging information in the analysis.

what is soft term in met calculations?
The purpose of adding a soft term in the calculation of missing transverse energy (MET) is to account for the low-momentum particles that are not clustered into jets or identified as specific objects (like electrons, photons, muons) in an event. These particles can originate from various sources, including the underlying event, pile-up (multiple proton-proton interactions in the same or nearby bunch crossings), or fragmentation and hadronization processes.
The soft term essentially corrects for the transverse momentum that is "missing" due to these unclustered or softly interacting particles. By including this term, the MET calculation becomes more accurate, reflecting the total momentum imbalance in the plane perpendicular to the beam direction. This is crucial for analyses involving particles that do not interact with the detector or interact very weakly, such as neutrinos or potential new particles predicted by theories beyond the Standard Model.

how big is 1 gev big?
In everyday terms, 1 GeV is approximately the kinetic energy of a flying mosquito or the energy a person uses in about a microsecond when walking. So, while it's a large amount of energy for particles at the quantum level, it's minuscule compared to the energy scales we interact with daily.

Systematics?
The correction factors applied to the simulated samples to improve the description of the photon and lepton identification and isolation efficiencies, momentum scale and resolution, and lepton trigger efficiencies are varied within their uncertainties to estimate the corresponding systematic uncertainty.

why $\eta$ - intercalibration?
The calibration process, often called "intercalibration," aims to ensure that the energy measurement of jets is accurate and uniform across the detector, regardless of where the jet originates within the detector's geometric coverage. Since detectors can have non-uniform responses due to their geometry, materials, and methods of operation, jets originating from different ηη regions might be measured with different levels of accuracy. This can introduce biases in the analysis of collision events.



