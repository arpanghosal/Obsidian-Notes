This page is linked to [[Systematics and Sensitivity]]

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

----

# Normalization of histograms:

Normalization of histograms in the context of particle physics experiments like ATLAS and CMS is an important concept, especially when comparing different data sets or theoretical predictions. In particle physics, histograms are often used to represent distributions of certain quantities (like particle energy, momentum, invariant mass, etc.) obtained from simulations or experimental data.

### What Does Normalization Mean?

Normalizing a histogram typically involves scaling the histogram so that its total area (or the sum of the bin heights) equals a specific value, often 1. This process allows for meaningful comparisons between histograms that may have different total numbers of events or different cross-sections. In particle physics, it's common to normalize histograms to:

1. **Unit Area**: Making the total area under the histogram equal to 1. This is useful for comparing the shape of distributions regardless of the number of events.

2. **Luminosity or Cross Section**: Scaling histograms to represent cross sections, allowing for direct comparison with theoretical predictions or other experiments.

3. **Number of Events**: Scaling histograms so that they represent the same number of events, useful for comparing efficiencies or acceptances.

### Why Normalize?

- **Comparing Different Processes**: Different processes (like signal and background in a collider experiment) might have different cross sections and luminosities. Normalizing histograms allows for the comparison of their shapes and relative contributions.

- **Theory vs. Experiment**: Comparing experimental data to theoretical predictions or simulations.

- **Visual Clarity**: Normalized histograms are easier to interpret when overlaid on the same plot.

### Illustrative Example in ROOT

Let's consider an example where you have histograms for different processes with different cross sections. You might want to normalize them for comparison. Here's a verbose example using ROOT:

```cpp
#include <TFile.h>
#include <TH1F.h>

void normalizeHistograms() {
    // Open a ROOT file containing histograms
    TFile *file = new TFile("data.root");

    // Retrieve histograms
    TH1F *hist1 = (TH1F*)file->Get("histogram1");
    TH1F *hist2 = (TH1F*)file->Get("histogram2");

    // Assume cross sections (in pb) and luminosity (in fb^-1)
    double crossSection1 = 10.0; // pb
    double crossSection2 = 5.0;  // pb
    double luminosity = 20.0;    // fb^-1

    // Convert luminosity to pb^-1
    double luminosity_pb = luminosity * 1000.0;

    // Scale histograms to luminosity and cross section
    hist1->Scale(crossSection1 * luminosity_pb / hist1->Integral());
    hist2->Scale(crossSection2 * luminosity_pb / hist2->Integral());

    // Now both histograms are normalized to the same luminosity
    // and can be compared directly

    // ... Further analysis or plotting
}
```

In this example:
- Histograms are scaled based on their cross section and a given luminosity.
- The `Scale` function is used, where the scale factor is the product of cross section and luminosity, divided by the integral (total number of events) of the histogram. This effectively normalizes the histograms to represent expected event yields for a given luminosity.

Remember, the exact method of normalization can vary depending on the specifics of your analysis and what you're trying to compare or demonstrate.
Say you've recorded the heights as follows (in meters):

- Orchard A: [4,5,4,6,5][4,5,4,6,5]
- Orchard B: [3,4,2,4,3,3,4,2,5,4][3,4,2,4,3,3,4,2,5,4]

**Normalized Orchard A Histogram**:

- 2m: 0/5=00/5=0
- 3m: 0/5=00/5=0
- 4m: 2/5=0.42/5=0.4
- 5m: 2/5=0.42/5=0.4
- 6m: 1/5=0.21/5=0.2

**Normalized Orchard B Histogram**:

- 2m: 2/10=0.22/10=0.2
- 3m: 3/10=0.33/10=0.3
- 4m: 4/10=0.44/10=0.4
- 5m: 1/10=0.11/10=0.1
- 6m: 0/10=00/10=0
Now you can compare them.

----

# Profile likelihood:
### Intuition Behind Profile Likelihood:

Profile likelihood is used in statistical modeling to concentrate on a parameter of interest, denoted as $\theta$, while managing nuisance parameters, denoted as $\phi$. This approach simplifies the analysis by reducing the complexity associated with nuisance parameters.

### Mathematical Formulation:

Given a likelihood function $L(\theta, \phi)$ that depends on both the parameter of interest $\theta$ and nuisance parameters $\phi$, the profile likelihood for $\theta$ is defined as:

$$ L_p(\theta) = L(\theta, \hat{\phi}(\theta)) $$

In this formula, $\hat{\phi}(\theta)$ represents the values of the nuisance parameters that maximize the likelihood for a specific value of $\theta$.

### Basic Example:

Suppose you're estimating the mean $\mu$ of a normal distribution, but the standard deviation $\sigma$ is unknown and is considered a nuisance parameter.

1. **Full Likelihood Function**: The likelihood function based on a sample $X = \{x_1, x_2, ..., x_n\}$ is given by:

   $$ L(\mu, \sigma) = \prod_{i=1}^{n} \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x_i - \mu)^2}{2\sigma^2}} $$

2. **Profile Likelihood for $\mu$**: To derive the profile likelihood, you calculate $\hat{\sigma}(\mu)$, which is the value of $\sigma$ that maximizes $L(\mu, \sigma)$ for each $\mu$. This value is then substituted back into the likelihood function:

   $$ L_p(\mu) = L(\mu, \hat{\sigma}(\mu)) $$

Typically, $\hat{\sigma}(\mu)$ might be the sample standard deviation if $\mu$ is assumed to be the sample mean.

### Interpretation:

- The profile likelihood $L_p(\theta)$ allows for a more straightforward analysis, focusing solely on $\theta$. This makes it easier to perform inferences, like constructing confidence intervals or conducting hypothesis tests.
- It effectively reduces the dimensionality of the problem, concentrating directly on the parameter of interest while properly considering the influence of nuisance parameters.

Profile likelihood is an essential tool in statistical analysis, especially in complex models with multiple parameters, as it offers a more manageable and focused approach to analysis in various practical applications.



The fitting done in **HistFactory**, **RooFit**, and similar frameworks like **TRExFitter** typically employs Maximum Likelihood Estimation (MLE). Here’s an overview of how the fitting process works:

### Fitting Process

1. **Model Definition**: 
   - Define the signal and background models using histograms and PDFs.
   - Include systematic uncertainties through nuisance parameters and constraint terms.

2. **Workspace Creation**: 
   - Combine data, models, parameters, and configurations into a workspace.

3. **Likelihood Construction**: 
   - Construct the likelihood function, which represents the probability of observing the data given the model and its parameters.

4. **Maximization**: 
   - Use numerical optimization techniques to maximize the likelihood function with respect to the model parameters.
   - This process finds the parameter values that best explain the observed data.

5. **Uncertainty Estimation**: 
   - Calculate the uncertainties on the fitted parameters, often using the profile likelihood method or other statistical tools.

### Example Workflow with TRExFitter

1. **Prepare Histograms**: Create histograms for data, signal, and background processes.
2. **Define Systematics**: Specify systematic uncertainties and their effects on the histograms.
3. **Configuration File**: Use a configuration file to define the model, including all components and systematic variations.
4. **Run Fit**: Execute the fitting process using the provided tools, which will perform MLE to find the best-fit parameters.

### MLE Fitting

The MLE fitting method aims to find the parameter values that maximize the likelihood function:

\[ L(\theta) = P(\text{data} | \theta) \]

Where \( \theta \) represents the parameters of the model. The goal is to find the \(\theta\) that makes the observed data most probable.

By maximizing the likelihood, MLE provides the most likely parameter values given the data, incorporating all available information, including systematic uncertainties. This approach is robust and widely used in high-energy physics experiments.


Uncertainties on the parameters in statistical fitting, such as those done with **HistFactory**, **RooFit**, or **TRExFitter**, are not simply the differences between nominal and fit values. Instead, they are typically estimated using the profile likelihood method or other statistical techniques.

### Profile Likelihood Method:
1. **Likelihood Function**: Construct the likelihood function \( L(\theta) \).
2. **Maximize Likelihood**: Find the parameter values that maximize \( L(\theta) \).
3. **Profile Likelihood**: For each parameter of interest, \( \theta_i \), profile the likelihood by maximizing \( L \) with respect to all other parameters.
4. **Confidence Intervals**: Determine the confidence intervals or uncertainties by finding the points where the profile likelihood drops by a certain amount (usually 1/2 for 1 standard deviation).

### Steps for Uncertainty Calculation:
- **Initialization**: Start with initial nominal values of the parameters.
- **Fitting**: Perform the fit to get the best-fit values.
- **Profile Likelihood**: Vary each parameter, re-maximize the likelihood for other parameters, and observe how the likelihood value changes.
- **Error Estimation**: The changes in the likelihood are used to calculate the uncertainties, giving a range within which the true parameter value is expected to lie.

### Statistical Interpretation:
The uncertainties reflect the range within which the parameter values can vary while still being consistent with the observed data, considering both statistical fluctuations and systematic uncertainties.
### Overall Fit
1. **Initial Fit**: Perform an overall fit with all parameters included to find the best-fit values that maximize the likelihood function \( L(\theta) \).

### Profiling for Uncertainties
2. **Profiling Each Parameter**: For each parameter of interest, vary that parameter while re-optimizing the likelihood function with respect to all other parameters. This is done to see how changes in this single parameter affect the likelihood, holding other parameters at their new optimized values.
   
3. **Likelihood Difference**: The profile likelihood is examined to determine the change in the likelihood value as the parameter is varied. The points at which the likelihood decreases by a specific amount (commonly 0.5 for a 1σ confidence interval) from its maximum define the uncertainty bounds for that parameter.

### Summary:
- **Best-Fit Model**: Initial fit to find the best-fit parameters.
- **Parameter Profiling**: Vary each parameter individually and re-optimize other parameters.
- **Uncertainty Estimation**: Determine the parameter uncertainties based on changes in the likelihood function.

This method ensures that the calculated uncertainties account for the correlations and interactions between different parameters.



---

# Uncertainties on POI:
Let's clarify the process and then address how to calculate the error or uncertainty on \(\mu\), especially in cases where the likelihood function is not symmetrical.

### Finding the Maximum of the Likelihood

1. **Setting the Derivative to Zero**: By setting the derivative of \(-2 \ln L\) with respect to \(\mu\) to zero, \( \frac{d(-2 \ln L)}{d\mu} = 0 \), you find the value of \(\mu\) that maximizes the likelihood function (or minimizes \(-2 \ln L\)). This value is the maximum likelihood estimate (MLE) of \(\mu\).

### Estimating Confidence Intervals

2. **Profile Likelihood Method**: To find the 68% confidence interval for \(\mu\), you vary \(\mu\) away from its MLE and find where the difference in \(-2 \ln L\) from its minimum value reaches 1. Formally, if \( L_{\text{max}} \) is the maximum likelihood, you look for values \(\mu_1\) and \(\mu_2\) such that:

   \[ -2 \ln \left( \frac{L(\mu_1)}{L_{\text{max}}} \right) = 1 \quad \text{and} \quad -2 \ln \left( \frac{L(\mu_2)}{L_{\text{max}}} \right) = 1 \]

### Calculating Error/Uncertainty on \(\mu\)

3. **Asymptotic Approximation**: Under the assumption that the likelihood function is approximately Gaussian near its maximum, the standard error of \(\mu\) can be estimated from the curvature of the likelihood function at the maximum. Mathematically, it is related to the second derivative (or the Hessian matrix in multivariate cases) of \(-2 \ln L\) at the MLE of \(\mu\). The variance of \(\mu\) is approximately the inverse of this second derivative.

4. **Non-Symmetrical Likelihood**: In cases where the likelihood is not symmetrical around the maximum:
   - **Profile Likelihood**: The 68% confidence interval determined by the profile likelihood method (as described above) provides an estimate of the uncertainty. This interval may not be symmetrical around the MLE of \(\mu\).
   - **Numerical Methods**: Often, numerical methods are used to find the points where the likelihood ratio reaches the threshold. This can be done through grid searches, optimization algorithms, or Monte Carlo techniques.
   - **Covariance Matrix**: If you have access to the full covariance matrix (from fitting software, for example), the square root of the diagonal element corresponding to \(\mu\) gives the standard error. This approach assumes a multivariate normal distribution of the parameters.

### Example

In a simple likelihood analysis where \(\mu\) is the only parameter, suppose the MLE of \(\mu\) is \(\mu_0\). By exploring values of \(\mu\) around \(\mu_0\) and finding where \(-2 \ln L\) increases by 1, you determine \(\mu_1\) and \(\mu_2\), which form your 68% confidence interval. If this interval is \([a, b]\), and it is not symmetrical around \(\mu_0\), this asymmetry is indicative of the skewness of your likelihood function. The standard error can be approximated as \((b - a) / 2\) if you assume symmetry, or more accurately, the interval itself represents the uncertainty considering its asymmetry.

In summary, the calculation of the error or uncertainty on a parameter of interest depends on the shape of the likelihood function and often involves both analytical approximations and numerical techniques, especially when dealing with non-symmetrical likelihood functions.

Certainly! Let's go through a numerical example to illustrate how to calculate the error or uncertainty on a parameter of interest (\(\mu\)) in a likelihood analysis. For simplicity, we'll assume a univariate case with a somewhat symmetric likelihood function.

### Example Scenario

Imagine you are analyzing data to estimate a parameter \(\mu\) (e.g., the mean of a distribution). You have constructed a likelihood function \(L(\mu)\) based on your data. After fitting your data, you find that the maximum likelihood estimate (MLE) of \(\mu\) is \(\mu_0 = 10\).

Now, you want to calculate the uncertainty on this estimate.

### Steps

1. **Maximum Likelihood Estimation**:
   - You find that the MLE of \(\mu\) is \(\mu_0 = 10\).

2. **Calculate the Second Derivative at MLE**:
   - Suppose the second derivative of \(-2 \ln L(\mu)\) at \(\mu = 10\) is \(-20\).
   - Hence, the curvature of the likelihood function at the maximum is \(20\).

3. **Estimate Variance and Standard Error**:
   - The variance of \(\mu\) is the inverse of this curvature: \( \text{Var}(\mu) = 1/20 = 0.05 \).
   - The standard error (SE) is the square root of the variance: \( SE = \sqrt{0.05} \approx 0.224 \).

4. **Find the 68% Confidence Interval**:
   - For a symmetric likelihood, the 68% confidence interval around the MLE is approximately \(\mu_0 \pm SE\).
   - Therefore, the interval is \( 10 \pm 0.224 \), or approximately \([9.776, 10.224]\).

### Interpretation

- The MLE of \(\mu\) is 10, with a standard error of about 0.224.
- You are 68% confident that the true value of \(\mu\) lies within the range [9.776, 10.224].
- This calculation assumes that the likelihood function is approximately symmetric and Gaussian near its maximum. If this is not the case, the interval might need to be determined numerically, as mentioned earlier.

This example simplifies several aspects for clarity, but it demonstrates the basic principles of estimating errors and confidence intervals in the context of likelihood-based parameter estimation. In real-world scenarios, especially in complex or non-Gaussian cases, more sophisticated methods might be necessary.


----

# Root to TreXFitter:
Certainly! In high-energy physics (HEP) analyses, tools like iMinuit, RooFit, RooStats, HistFactory, HistFitter, and TRExFitter are often used in a connected workflow for statistical analysis, especially for tasks like building likelihood models and performing profile likelihood measurements. Let's go through a typical workflow using these tools, and then we'll discuss how profile likelihood measurements fit into this context.

### Workflow from Scratch:

1. **Data Preparation and Histogramming**:
    - **Use Case**: This step involves processing raw experimental data to produce histograms. Histograms are used to represent distributions of various observables, such as particle energies, momenta, invariant masses, etc.
    - **Tools**: At this stage, general data analysis tools like ROOT (a C++ framework developed at CERN) are commonly used for data manipulation and histogram creation.

2. **Model Building with HistFactory**:
    - **Use Case**: HistFactory is designed to build statistical models from histograms. It's particularly useful for constructing complex models that include multiple components (signal, various backgrounds) and systematic uncertainties.
    - **Action**: You define the structure of your model, including how different systematic uncertainties affect the shape and normalization of your histograms.

3. **Fitting the Model using RooFit/RooStats**:
    - **Use Case**: Once the model is built, the next step is to fit this model to the data to extract parameters of interest (like signal strength, particle masses, branching ratios, etc.).
    - **Tools**: RooFit and RooStats are part of the ROOT framework. RooFit provides tools for building and fitting probability models to data, while RooStats is used for statistical inference.
    - **Action**: Using these tools, you can perform maximum likelihood estimation to fit the model to the data. 

4. **Optimization with iMinuit**:
    - **Use Case**: iMinuit is a minimization tool that finds the best-fit parameters by optimizing the likelihood function.
    - **Action**: It's often used in conjunction with RooFit/RooStats to find the parameter values that maximize the likelihood or minimize the negative log-likelihood.

5. **Analysis and Interpretation with HistFitter or TRExFitter**:
    - **Use Case**: HistFitter and TRExFitter are high-level frameworks that integrate the functionalities of ROOT, RooFit, and HistFactory for comprehensive statistical analysis.
    - **Action**: They provide a more user-friendly interface for defining models, performing fits, estimating uncertainties, and conducting hypothesis testing.

### Profile Likelihood Measurements:

Profile likelihood is a technique used to handle nuisance parameters (parameters that are not of primary interest but must be included in the model) when estimating the parameters of interest.

- **In RooFit/RooStats**: These tools allow you to perform profile likelihood analyses. They automatically handle the profiling of nuisance parameters, i.e., adjusting nuisance parameters to their best-fit values at each point of the parameter of interest, and provide you with the profile likelihood ratio as a test statistic.
- **In HistFitter and TRExFitter**: These frameworks simplify the process of setting up and performing profile likelihood analyses. They use RooFit/RooStats under the hood for the statistical heavy lifting.

### Workflow for Likelihood Building to Profile Likelihood Fitting in HEP Analysis:

1. **Construct a Statistical Model**: This involves defining the signal and background models, incorporating systematic uncertainties as nuisance parameters. Tools like HistFactory are used here.
2. **Fit the Model to Data**: Using RooFit/RooStats, the model is fitted to the data. This involves adjusting both the parameters of interest and nuisance parameters to maximize the likelihood function.
3. **Perform Profile Likelihood Analysis**: The profile likelihood technique is applied to estimate the parameters of interest while properly accounting for the nuisance parameters. This can involve scanning the parameter of interest while profiling (adjusting) the nuisance parameters at each point.
4. **Extract Confidence Intervals**: The profile likelihood is used to construct confidence intervals for the parameters of interest.
5. **Interpret Results**: The final step involves interpreting the results in the context of the physics analysis, such as setting limits on particle properties or searching for new phenomena.

Throughout this workflow, the intuition is to build a model that best represents the data, fit this model using statistical techniques, and then extract meaningful physics results while properly handling uncertainties and complex dependencies in the data. The mentioned tools provide a comprehensive suite to perform these tasks effectively in high-energy physics research.

----

# Why Nuisance parameters enter as Gaussian ?
In the context of data fitting, particularly in physics, nuisance parameters are variables that are not of direct interest but must be included in the model to accurately describe the data. Confining these nuisance parameters with Gaussian constraints is a common practice, and here's why:

### What are Nuisance Parameters?

Nuisance parameters are variables in a model that are not the primary target of a study but can affect the outcome or interpretation of the experiment. These could include background levels, calibration constants, detector efficiencies, or other systematic uncertainties.

### Why Use Gaussian Constraints?

1. **Central Limit Theorem**: The Gaussian (or normal) distribution is often used due to the Central Limit Theorem, which states that the sum of a large number of independent random variables, regardless of their distribution, will tend to follow a Gaussian distribution. Many nuisance parameters are influenced by multiple factors, making the Gaussian distribution a natural choice due to this theorem.

2. **Mathematical Convenience**: Gaussian distributions are mathematically tractable, making them convenient for analytical calculations. They are characterized by just two parameters (mean and standard deviation), simplifying the process of incorporating them into a fitting procedure.

3. **Physical Interpretation**: In many cases, Gaussian distributions reasonably represent the real-world behavior of the uncertainties associated with nuisance parameters. For example, measurement errors, instrumental calibration uncertainties, and other systematic effects often follow a Gaussian distribution.

### How Are They Constrained?

1. **Incorporating in Likelihood Function**: In a fitting procedure, the likelihood function (which measures how well the model fits the data) is modified to include terms for nuisance parameters. These terms are often Gaussian functions centered around the expected value of the nuisance parameter, with a width corresponding to the uncertainty in its value.

2. **Regularization**: This inclusion acts as a form of regularization, preventing the nuisance parameters from straying too far from their expected values. It essentially tells the fitting algorithm, "You can adjust this parameter to improve the fit, but if you move too far from the expected value, it will significantly decrease the likelihood."

3. **Penalizing Extreme Values**: The Gaussian constraint penalizes extreme values of the nuisance parameters, effectively incorporating our prior knowledge or uncertainties about these parameters into the fitting process.

4. **Bayesian Interpretation**: From a Bayesian perspective, these Gaussian constraints can be seen as prior probabilities for the nuisance parameters. The fitting process then updates these priors in light of the observed data.

### Intuition Behind the Practice:

The intuition is that while these parameters are necessary for the model, their exact values aren't known. By constraining them within a Gaussian distribution, you're essentially saying, "I expect this parameter to be around this value, give or take this much, based on previous knowledge or measurements." This approach helps to account for uncertainties in a controlled way, ensuring that they don't unduly influence the primary parameters of interest.

In summary, constraining nuisance parameters with Gaussian distributions in physics is a balance of mathematical convenience, the central limit theorem, and realistic representation of uncertainties. It allows for a more accurate and controlled fitting process, especially when dealing with complex models and datasets.

---

![[Pasted image 20231211154303.png]]


---


# How are \mu determined?
In the context of statistical analysis, particularly when using the profile likelihood (PL) method, determining fixed values of \( \theta \) (the parameter of interest) involves a combination of theoretical considerations, experimental design, and practical constraints. Here's how these values are typically determined:

### 1. **Parameter of Interest (\( \theta \))**:
   - **Definition:** The parameter \( \theta \) represents a specific quantity that the analysis aims to estimate or test. This could be anything from a physical constant in a physics experiment to a mean value in a survey analysis.
   - **Range of Interest:** Often, researchers have a range of values for \( \theta \) that they consider plausible or of interest based on previous studies, theoretical predictions, or practical considerations.

### 2. **Setting the Values of \( \theta \)**:
   - **Grid or Range:** In practice, values of \( \theta \) are often chosen to span a range or grid that covers the region of interest. The granularity of this grid (how many values and how far apart they are) can depend on the precision required and the computational resources available.
   - **Initial Estimates:** Initial estimates or educated guesses about \( \theta \) can be obtained from previous studies, theoretical models, or pilot data.

### 3. **Statistical Methods**:
   - **Maximum Likelihood Estimation (MLE):** An initial MLE can be performed to find a starting point. This is the value of \( \theta \) that maximizes the likelihood function, ignoring the nuisance parameters (\( \alpha \)).
   - **Confidence Intervals:** In some analyses, the range of \( \theta \) might be determined based on desired confidence intervals.

### 4. **Iterative Process**:
   - **Refinement:** As analysis proceeds, the range of \( \theta \) values might be refined based on interim findings. If certain values of \( \theta \) lead to significantly lower likelihoods, they might be excluded from further analysis.

### 5. **Practical Considerations**:
   - **Computational Limitations:** The number of values of \( \theta \) that can be practically tested might be limited by computational resources, as maximizing the likelihood function over \( \alpha \) for each value of \( \theta \) can be computationally intensive.
   - **Resolution vs. Computation Trade-off:** There is often a trade-off between the resolution of the \( \theta \) grid and the computational time required.

### 6. **Exploring the Parameter Space**:
   - **Sensitivity Analysis:** In some cases, a sensitivity analysis might be conducted to understand how changes in \( \theta \) affect the results.

### Conclusion:
The fixed values of \( \theta \) are determined based on the specific objectives of the study, prior knowledge, and practical constraints. The goal is to systematically explore the parameter space of \( \theta \) to understand the behavior of the likelihood function and, by extension, to make inferences about \( \theta \) itself in the presence of nuisance parameters (\( \alpha \)).

---



# Differences - histfitter vs. trex-fitter:

"HistFitter" and "TRExFitter" are software frameworks used in particle physics, particularly for data analysis in experiments like those conducted at the Large Hadron Collider (LHC). Both are designed to perform statistical fits to histograms, primarily to extract signal and background contributions in searches for new particles or processes. Let's delve into what each tool is and their similarities and differences:

### HistFitter:
1. **Overview:**
   - HistFitter is a software framework developed for statistical data analysis in particle physics. It's used to construct, fit, and interpret histograms from collider data.
   - The tool is designed to handle complex fits involving multiple regions, channels, and systematic uncertainties.

2. **Usage:**
   - HistFitter is extensively used in various analyses by the ATLAS Collaboration at the LHC, especially in searches for new particles or phenomena beyond the Standard Model.
   - It facilitates the estimation of signal strengths, setting limits on new physics, and conducting hypothesis testing.

3. **Key Features:**
   - Incorporates systematic uncertainties and correlations.
   - Allows for simultaneous fits across multiple channels or regions.
   - Performs statistical interpretation of the results, like setting upper limits or calculating significances.

### TRExFitter:
1. **Overview:**
   - TRExFitter, originally part of the HistFitter framework, was later developed as a separate tool. It shares many features with HistFitter but has some differences in implementation and functionality.
   - Like HistFitter, it is used for fitting histograms in particle physics experiments.

2. **Usage:**
   - TRExFitter is also used in the ATLAS Collaboration for various analyses. It's particularly valuable in the measurement of cross-sections, setting limits, and performing discovery tests.

3. **Key Features and Differences:**
   - TRExFitter offers a more flexible configuration system and improved graphical outputs.
   - It provides enhanced capabilities for handling systematic uncertainties and performing global fits.
   - The tool has been designed with a focus on user-friendliness and robustness.

### Similarities and Differences:
- **Similarities:**
  - Both are used for statistical analysis in particle physics.
  - Each can handle complex fits with multiple systematic uncertainties.
  - Both are used by the ATLAS Collaboration for various types of analyses.

- **Differences:**
  - TRExFitter is seen as an evolution of HistFitter, with improvements in usability, flexibility, and output visualization.
  - TRExFitter may offer more advanced features for certain types of analyses, particularly those involving complex systematic uncertainties and multi-region fits.

### Conclusion:
HistFitter and TRExFitter are both powerful tools in the field of particle physics, enabling researchers to perform detailed statistical analyses of experimental data. While HistFitter laid the groundwork for this type of analysis, TRExFitter has built upon and expanded these capabilities, offering enhanced features and user experience. The choice between the two may depend on the specific needs of an analysis, the preference of the researchers, and the evolution of the tools themselves.


---

# Pseudo data set:

Asimov data is a theoretical concept used in statistical analyses, particularly in high-energy physics, to evaluate the expected performance of an analysis under a given model. It differs from actual data, which consists of the real experimental results. Let's clarify these concepts and address your questions:

### Asimov Data:
1. **Concept:** Asimov data refers to a dataset where the observed values are set exactly equal to the expected values under a particular model (usually the null hypothesis, like the Standard Model in particle physics). 
2. **Purpose:** It's used for testing and calibration purposes, particularly to evaluate the sensitivity of an analysis or to validate analysis procedures without relying on real experimental data.
3. **Characteristics:** In Asimov data, there's no statistical fluctuation - it represents an idealized scenario.

### Comparing Asimov Data with Actual Data:
- **130 Simulated Events vs. Asimov Data:** If you have 130 simulated events (MC simulated events), the corresponding Asimov dataset under the assumption that your model is correct would also expect 130 events. In this case, the Asimov data acts like a perfect realization of your model.
- **Actual Data with 140 Events:** If the actual data consists of 140 events, this is a different scenario from what your model (or the Asimov dataset) predicts. This discrepancy could be due to statistical fluctuations or could indicate that your model doesn't perfectly describe reality.

### Impact on Signal Strength (\(\mu\)):
- **Asimov Fit:** When fitting the Asimov data, the signal strength \(\mu\) would typically be consistent with the expectation under your model. For instance, if your model expects 130 events and you observe 130 events in the Asimov data, \(\mu\) would be around 1, indicating that the observed data matches the expectation.
- **Actual Data Fit:** If you fit the actual data and find 140 events, the signal strength \(\mu\) might differ from 1, depending on the specifics of your analysis. A \(\mu\) greater than 1 could suggest that there are more events than expected, possibly hinting at new physics if the excess is statistically significant.
- **Statistical Analysis:** The difference in \(\mu\) between the Asimov fit and the actual data fit can provide insights into how well the model describes the real data. In rigorous analyses, confidence intervals and p-values are often calculated to assess the significance of any discrepancies.


## How fitters handle them?

Fitters like TRExFitter can indeed create Asimov datasets, and they are often used for this purpose in high-energy physics analyses. The process and expectations surrounding Asimov datasets in the context of these fitters are as follows:

### Creation of Asimov Datasets in Fitters:
- **Generating Asimov Data:** Fitters like TRExFitter have the capability to generate Asimov datasets. This is done by setting the observed data to the expected values under a specific model (usually the null hypothesis or a model of interest).
- **Use of Asimov Data:** The Asimov dataset is used to evaluate the expected performance of an analysis. This includes determining expected signal strengths, setting expected limits, and estimating uncertainties, all in an idealized scenario without statistical fluctuations.

### Determining \( \mu \) and Uncertainties:
- **Fitting Process:** During the fit with an Asimov dataset, the fitter uses the likelihood model to estimate the signal strength (\( \mu \)) and uncertainties. It assumes that the observed data is exactly as predicted by the model.
- **Expected Signal Strength:** When fitting an Asimov dataset, you would typically expect a signal strength (\( \mu \)) of around 1, assuming the Asimov data is generated under the assumption that the model perfectly describes the reality (i.e., the null hypothesis is true).
- **Uncertainties Estimation:** The fitter also estimates uncertainties, including both statistical and systematic uncertainties, based on the model and the Asimov dataset.

### Expectations from Asimov Fitting:
- **Signal Strength (\( \mu \)) Around 1:** Yes, in an Asimov fit, since the observed data (in this case, the Asimov data) matches the expectation by construction, \( \mu \) should be around 1. This indicates that the model's prediction is in perfect agreement with the "observed" data (the Asimov dataset).
- **Sensitivity and Calibration:** The primary purpose of using an Asimov dataset in this context is to understand the analysis's sensitivity and to calibrate statistical methods. It allows researchers to anticipate how the analysis will behave under ideal conditions.

## Further clarification:

When you perform an Asimov fit, especially in the context of a tool like TRExFitter, the concept of "comparing 130 against 130 or 66 against 66 with variable signal strength" needs a bit of clarification. The Asimov dataset is constructed to represent an idealized scenario where the expected number of events (both signal and background) matches exactly with the observed number of events. Here's how it works in your case:

### Asimov Dataset Construction:
- **Total Events:** You have a total of 130 simulated events, comprising 64 signal events and 66 background events from various processes.
- **Asimov Dataset:** In the Asimov dataset, the number of events (both signal and background) will be set to their expected values under the model you are testing. If your model predicts 64 signal events and 66 background events, then the Asimov dataset will also contain exactly 64 signal and 66 background events.

### Asimov Fitting Process:
- **Signal Strength (\(\mu\)):** When you fit this Asimov dataset with TRExFitter, the tool will adjust the signal strength (\(\mu\)) and other parameters to see how well the model can explain this idealized dataset. In an Asimov fit, since the dataset is constructed to match the model's expectations, the fitted signal strength \(\mu\) will typically be around 1.
- **Comparison:** The fitting process isn't so much about comparing 130 against 130 or 66 against 66, but rather about adjusting the model parameters (including \(\mu\)) to find the best match between the model's predictions and the Asimov dataset. In this context, "best match" means the parameter values under which the model's predictions would have most likely resulted in the observed Asimov data.

### Practical Implications:
- **Purpose:** The purpose of the Asimov fit is to evaluate the sensitivity of your analysis and the expected behavior of your fitting procedure under ideal conditions.
- **Results Interpretation:** The results from an Asimov fit are used to understand the expected statistical uncertainties and the potential to distinguish signal from background under the assumption that the model is correct.

### Conclusion:
In summary, when you perform an Asimov fit with TRExFitter in your scenario, the tool uses the total set of events (130 in your case) but constructs the Asimov dataset so that it perfectly matches the expected distribution of signal and background events according to your model. The fitting process then adjusts \(\mu\) and potentially other model parameters to evaluate how well the model fits this idealized data. The key point of an Asimov fit is to validate and understand your analysis approach in a controlled, predictable setting.


## Why Asimov? Purpose they serve - 
The Asimov dataset and the corresponding Asimov fit play crucial roles in statistical analysis, particularly in high-energy physics experiments. Let's delve deeper into their purposes, possible scenarios, how they are handled in analysis frameworks like TRExFitter, the behavior of the signal strength parameter (\(\mu\)), and more.

### Purpose of Asimov Fit:
1. **Sensitivity Evaluation:** The Asimov fit assesses how sensitive your analysis is to the presence of a signal. This involves determining how well your analysis can detect a signal if it is present and how it can differentiate this signal from the background.
2. **Expected Behavior:** It helps understand how the fitting procedure will behave under "perfect" conditions, i.e., when the observed data perfectly matches the expected model predictions without statistical fluctuations.

### Case Scenarios for Asimov Fit:
1. **Discovery Potential:** Assessing the potential of an analysis to discover new phenomena. If the Asimov fit with an injected signal shows a significant deviation from the null hypothesis, it indicates good discovery potential.
2. **Limit Setting:** In searches where no significant excess is observed, the Asimov fit helps in setting upper limits on the production cross-section or the strength of a new interaction.
3. **Systematics Assessment:** Evaluating the impact of systematic uncertainties under controlled conditions.

### Handling of Asimov Dataset in Fitters:
- **Runtime Generation:** In tools like TRExFitter, the Asimov dataset is typically generated at runtime. The expected event yields (both signal and background) are calculated based on the model and used to create a hypothetical dataset.
- **Storage:** This dataset may not necessarily be stored as a traditional dataset; instead, it's often used on-the-fly for fitting and analysis.

### Variation and Range of Signal Strength (\(\mu\)):
1. **Definition:** \(\mu\) represents the signal strength, with \(\mu = 1\) indicating that the signal yield is as predicted by the model, \(\mu = 0\) indicating no signal, and \(\mu > 1\) suggesting a signal stronger than the model prediction.
2. **Variation in Asimov Fits:** In an Asimov fit, \(\mu\) is typically set to 1 to assess the analysis's ability to recover the expected signal. However, different values of \(\mu\) can be tested to evaluate the analysis's response to various signal strengths.
3. **Interpreting \(\mu\) in Real Data Fits:** When fitting real data, the value of \(\mu\) that best fits the data is determined. A \(\mu\) significantly different from 1 may indicate new physics if the model assumes the Standard Model as the null hypothesis.

### Detailed Process:
1. **Model and Hypothesis:** Define the theoretical model or hypothesis, including the expected signal and background yields.
2. **Generating Asimov Dataset:** Calculate the expected yields for signal and background and construct an Asimov dataset that perfectly matches these expectations.
3. **Performing the Fit:** Fit this Asimov dataset using the statistical model, adjusting \(\mu\) and other parameters. In the ideal scenario, \(\mu\) should return to the value it was set at (often 1).
4. **Analyzing Outcomes:** Evaluate the fit's outcome, including the estimated \(\mu\), confidence intervals, and the effect of systematic uncertainties.
5. **Comparing with Actual Data:** Perform the same fit procedure on actual data and compare the results with those from the Asimov fit to understand the analysis's performance and potential deviations from the model predictions.

### Conclusion:
The Asimov fit is a powerful tool for testing and validating analysis strategies in particle physics. By using a hypothetical dataset that perfectly aligns with model predictions, physicists can gauge the effectiveness of their analysis methods and prepare for various outcomes when analyzing real data. This approach is fundamental in scenarios where precise measurements and the search for new phenomena are involved.

### Note:
<mark style="background: #FFB8EBA6;">
If the observed data is consistent with the background-only hypothesis (null hypothesis) within the uncertainties, then no discovery claim can be made. This doesn't necessarily mean the signal isn't there; it might just be that the analysis doesn't have enough sensitivity to detect it under the given conditions.</mark>


----


# Information:
The concept of information in physics is profound and multifaceted, intertwining with the very fabric of reality according to quantum mechanics and thermodynamics. Physically,<mark style="background: #FFB86CA6;"> information refers to the arrangement or state of a system that can be measured and known</mark>. It plays a crucial role in understanding physical processes, from the microscopic world of quantum particles to the cosmic scale of black holes.

### Information in Quantum Mechanics

In quantum mechanics,<mark style="background: #FFB86CA6;"> information is related to the state of a quantum system</mark>. The wave function of a quantum system encodes all possible information about the system's properties, such as position, momentum, spin, etc. Measurements of these properties collapse the wave function to a specific state, revealing information about the system at the cost of disturbing it.

### Information and Thermodynamics

The relationship between information and thermodynamics is epitomized in the concept of entropy, which measures the amount of disorder or randomness in a system. <mark style="background: #FFB8EBA6;">Entropy is also a measure of information</mark>, specifically the information that is not known about a system. The more disordered a system, the more information it theoretically contains, because there are more possible microstates it could be in. This idea is central to the second law of thermodynamics, which states that the total entropy of an isolated system can never decrease over time.

### Black Hole Information Paradox

The black hole information paradox arises from the properties of black holes as described by general relativity and quantum mechanics. According to classical general relativity, anything that falls into a black hole is lost forever, beyond the event horizon from which not even light can escape. However, quantum mechanics suggests that information cannot be destroyed. This leads to a paradox when considering what happens to the information about the state of matter that falls into a black hole.

Hawking's radiation, predicted by Stephen Hawking, complicates this issue further. It suggests that black holes emit radiation due to quantum effects near the event horizon, causing them to lose mass and eventually evaporate. <mark style="background: #ABF7F7A6;">The paradox is: if the black hole evaporates completely, where does the information about the matter that fell into it go? Does it get destroyed (violating quantum mechanics), or is it somehow preserved?</mark>

### Resolutions and Implications

Several theoretical resolutions to the black hole information paradox have been proposed, involving concepts like holographic principles, where information is encoded on the event horizon; firewall theories, suggesting violent quantum activity at the horizon; or ideas that information is somehow returned to the universe through Hawking radiation. These discussions touch on the fundamental nature of information in physics and its conservation laws.

The interplay between information and physics challenges our understanding of reality, hinting at a deeper level of physical laws where information plays a central role. The resolution of issues like the black hole information paradox could lead to significant breakthroughs in our understanding of the universe, quantum mechanics, and gravity.

### Quantum Gravity and Pre-Big Bang Scenarios

- **Beyond Classical Physics**: Theories of quantum gravity, such as string theory and loop quantum gravity, attempt to describe the universe's behavior at the smallest scales, including the state of the universe at the Big Bang. These theories suggest that the classical concept of a singularity might be replaced with something more complex and understandable, potentially resolving the paradoxes associated with infinite density and temperature.
    
- **Information Conservation**: In quantum mechanics, information is considered to be conserved. This principle leads to intriguing implications for the Big Bang and the nature of singularities. If information is conserved, then in some form, the information that constitutes the current universe was present at the Big Bang, transformed through the laws of physics from the initial state to the complex cosmos we observe today.

---

