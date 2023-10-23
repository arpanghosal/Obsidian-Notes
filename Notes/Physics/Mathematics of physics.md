In particle physics, cross section is a measure of the probability that a particle interaction will occur. It is typically measured in units of area (e.g. barns), and represents the effective area of the target particle that the incident particle interacts with.

The event number, on the other hand, is a measure of the number of particle interactions that have been observed in an experiment.

The relationship between event number and cross section depends on the specific experimental setup and the physics being studied. However, in general, the cross section can be calculated from the event number using the following formula:

cross section = event number / (luminosity x efficiency)

where luminosity is a measure of the intensity of the particle beam, and efficiency is the fraction of interactions that are successfully detected by the experiment.



The product of luminosity and efficiency is often referred to as the normalization factor. The normalization factor is used to convert the number of observed events in an experiment to a physical cross section measurement.

Luminosity is a measure of the number of particles passing through a unit area per unit time, and is typically expressed in units of inverse area-time, such as cm^-2 s^-1. Efficiency is the fraction of events that are detected by the experiment, and is typically determined through simulation or calibration studies.

The normalization factor takes into account both the intensity of the particle beam (luminosity) and the effectiveness of the experimental setup at detecting events (efficiency). By multiplying the observed event rate by the normalization factor, the resulting cross section measurement is independent of the experimental conditions and can be compared to theoretical predictions or other experimental results.

It is worth noting that the determination of the normalization factor can be a significant source of uncertainty in cross section measurements, and careful calibration and control of systematic effects is necessary to achieve precise and accurate results.

Event weights are factors used to adjust the simulated event samples to better match the expected distribution of events in real data. These weights are typically applied to simulated events during analysis, and can affect the calculation of event numbers and efficiencies.
Event weights are used to correct for various effects, such as detector response, reconstruction efficiencies, and event selection criteria, that may not be perfectly modeled in the simulated event samples. By adjusting the weights of simulated events, the distribution of events in the simulated samples can be made to better match the distribution of events in real data.
The effect of event weights on event numbers and efficiency can depend on the specific analysis being performed. In some cases, event weights may be used to correct for differences in the detection efficiency between real data and simulated events, which can affect the calculation of efficiency. In other cases, event weights may be used to adjust the number of simulated events in certain regions of phase space to better match the expected distribution of events in real data, which can affect the calculation of event numbers.

The normalization factor used to convert the number of observed events in an experiment to a physical cross section measurement is subject to various sources of uncertainty, which can contribute to the overall uncertainty in the cross section measurement.

The uncertainty in the luminosity measurement, for example, can be a significant source of uncertainty in the normalization factor. The luminosity measurement can be affected by various factors, such as beam conditions, detector response, and calibration, and the uncertainty in the luminosity measurement can propagate to the uncertainty in the normalization factor and the resulting cross section measurement.

The efficiency measurement can also contribute to the uncertainty in the normalization factor. The efficiency measurement can be affected by various factors, such as detector response, trigger efficiency, and event selection criteria, and the uncertainty in the efficiency measurement can propagate to the uncertainty in the normalization factor and the resulting cross section measurement.

In addition to these sources of uncertainty, there can be other sources of systematic uncertainty, such as uncertainties in the simulation of the particle interactions, detector response, and event reconstruction. These systematic uncertainties can also contribute to the overall uncertainty in the cross section measurement.

## Markov chains in SM:
in a Monte Carlo simulation within the context of the Standard Model (SM) of particle physics, the transition from one particle to another is often based on the SM's predictions of branching fractions and other relevant parameters. Monte Carlo simulations are powerful computational tools used to model the behavior of particles and their interactions, and they rely on the known theoretical framework of the Standard Model to make these predictions.

Here's how it typically works:

1. **Known Processes:** The Standard Model provides predictions for various particle interactions and decay processes. These predictions include information about the branching fractions, which indicate the probabilities of a particle decaying into different final-state particles or states.
    
2. **Random Sampling:** In a Monte Carlo simulation, random numbers are used to simulate the stochastic aspects of particle interactions. For example, when a particle undergoes a decay, a random number is generated to determine which decay channel it follows, according to the branching fractions specified by the Standard Model.
      ### Sampling :
      Here's a step-by-step explanation of how random sampling works in this context:

	1. **Decay Process Selection:** Imagine you have a particle, let's say a hypothetical particle X, and according to the Standard Model, this particle can decay into several possible final states or decay channels. Each of these decay channels is associated with a branching fraction, which is a probability that indicates the likelihood of the particle X decaying into that specific final state.
	    
	2. **Random Number Generation:** To simulate the decay process of particle X, the Monte Carlo simulation generates a random number. This random number is typically drawn from a uniform distribution between 0 and 1.
	    
	3. **Branching Fraction Comparison:** The generated random number is then compared to the branching fractions for each possible decay channel. Each channel's branching fraction represents its share of the total probability for the particle X to decay. The random number determines which channel is selected.
	    
	4. **Decay Channel Selection:** The decay channel with the branching fraction that corresponds to the generated random number is chosen. This means that more probable decay channels are more likely to be selected, but there is still an element of randomness.
	    
	5. **Kinematics and Final State:** Once the decay channel is determined, the simulation then proceeds to calculate the kinematics of the decay. This involves determining the momenta, angles, and other properties of the final-state particles, all while conserving energy and momentum.
	    
	6. **Repeat for Many Events:** The simulation repeats this process for a large number of events to build up a statistically meaningful sample of particle interactions. This allows researchers to make predictions about the behavior of particle ensembles in various experimental conditions.
			<details>
			<summary> Example </summary>
		   Let's consider a simplified example of a particle X decaying into two possible final states: A and B. The branching fractions for these decay channels are as follows:
		
		- Branching Fraction for Decay into A: 0.60
		- Branching Fraction for Decay into B: 0.40
		
		Now, let's simulate the decay process using random number generation:
		
		1. Generate a random number between 0 and 1. Let's say the generated random number is 0.75.
		    
		2. Compare the random number to the branching fractions:
		    
		    - Random number (0.75) is greater than or equal to 0.60 (the branching fraction for decay into A).
		    - Random number (0.75) is less than 0.60 + 0.40 (the sum of branching fractions for both decay channels).
		3. Based on this comparison, we select the decay channel:
		    
		    - Since the random number falls in the range between 0.60 and 1.00 (0.60 + 0.40), we choose decay channel B.
		
		So, in this particular event, the random number selection led to the decay of particle X into final state B. If we repeated this process many times (generating different random numbers for each event), we would obtain a distribution of decay events that reflects the branching fractions specified by the Standard Model: approximately 60% of the decays into A and 40% into B.
		</details>
1. **Kinematics:** The simulation also takes into account the kinematics of the process, including the momenta and angles of the final-state particles. These kinematic properties are determined based on the known laws of particle physics and the conservation of energy and momentum.
    
4. **Iteration:** The simulation iterates through many events, each time randomly choosing the type of interaction or decay process for each particle, based on the branching fractions and other probabilities provided by the Standard Model.
    
5. **Statistical Analysis:** After running a large number of events, the simulation results can be analyzed statistically to make predictions about the behavior of particles in specific experimental conditions.
---


![[Pasted image 20231009143214.png]]

