in the field of particle physics, the term "Asimov dataset" is sometimes used to refer to a hypothetical dataset that is used to determine the expected sensitivity of a particle physics experiment to a particular signal or new physics phenomenon. This dataset is named after Isaac Asimov because it is a "fake" dataset that is designed to represent an idealized scenario in which the experiment would be able to precisely measure the properties of the signal in question.

The Asimov dataset is often used to evaluate the statistical significance of a potential discovery in particle physics, by comparing the observed data to the expected background and signal in the Asimov dataset. This allows researchers to estimate the probability that the observed data is consistent with the background alone, or if there is evidence for the presence of a signal.

This page is linked to [[Mathematics of physics]]


In particle physics, the term "sensitivity" refers to the ability of an experiment to detect a particular signal or new physics phenomenon. It is a measure of the smallest possible signal that the experiment is capable of detecting with a given level of statistical significance.

The sensitivity of an experiment is typically quantified in terms of its "expected limit" on the signal strength or cross-section of the new physics phenomenon being searched for. The expected limit is the maximum allowed value of the signal strength or cross-section, such that if the actual signal strength or cross-section is smaller than the expected limit, the experiment would not be able to distinguish it from the background noise.

The expected limit is often parameterized using statistical techniques such as the Neyman construction or the frequentist approach. These techniques involve defining a test statistic that measures the deviation of the observed data from the expected background, and calculating the probability of obtaining a larger value of the test statistic under the null hypothesis of no signal.

The expected limit can then be calculated by determining the signal strength or cross-section that corresponds to a given level of statistical significance, such as a 95% confidence level. This allows researchers to evaluate the sensitivity of the experiment to the new physics phenomenon being searched for, and to compare the sensitivity of different experiments or analysis strategies.



The "expected limit" in particle physics experiments is usually quoted as a maximum allowed value for the signal strength or cross-section of a particular new physics phenomenon. This may seem counterintuitive, as one might expect that a lower limit would be more informative.

However, the reason for quoting the expected limit as a maximum allowed value is related to the statistical framework used to analyze the data. In frequentist statistics, which is the dominant framework used in particle physics, the hypothesis being tested is that the observed data is consistent with a null hypothesis, which typically represents the background-only scenario with no signal present.

The expected limit is defined as the largest signal strength or cross-section that the experiment would not be able to distinguish from the background-only scenario with a certain level of statistical significance, such as a 95% confidence level. This means that if the actual signal strength or cross-section is smaller than the expected limit, the experiment would not be able to claim a significant detection of the signal with that level of confidence.

The expected limit is therefore a measure of the sensitivity of the experiment to the signal being searched for. By quoting the limit as a maximum allowed value, researchers can compare the sensitivity of different experiments or analysis strategies in a consistent way. The lower the expected limit, the more sensitive the experiment is to the signal being searched for.




"systematics" refer to uncertainties that arise from various sources that can affect the measurements of physical observables, such as the energy or momentum of particles. These sources of uncertainty can include detector effects, calibration uncertainties, theoretical uncertainties, and others. To test systematics, a number of methods can be used, including:

1.  Comparing Data and Monte Carlo Simulation: Monte Carlo simulations are computer-generated events that simulate the expected particle interactions in a detector. Comparing data from the detector to Monte Carlo simulations can help identify sources of systematic uncertainties. If the simulations do not agree with the data, this can indicate a potential systematic effect.
    
2.  Varying Experimental Conditions: The sensitivity of a measurement to systematic uncertainties can be tested by varying experimental conditions. For example, the measurement can be repeated with different detector configurations, different calibration techniques, or different reconstruction algorithms. If the measurement remains consistent under different conditions, this suggests that the uncertainties due to those sources are well-understood.
3. -   Studying Known Effects: Some systematic effects are well-known and can be studied directly. For example, the response of a detector to a specific particle can be measured using a calibration source. These measurements can be used to quantify the systematic uncertainties associated with the detector response.
    
4. -   Estimating Theoretical Uncertainties: Theoretical uncertainties can be estimated using calculations and simulations of the physical processes involved. By comparing theoretical predictions with experimental data, the impact of theoretical uncertainties can be assessed and quantified.
    
5. -   Performing Blind Analyses: Blind analyses are used to test the sensitivity of a measurement to systematic uncertainties by removing knowledge of the result before the analysis is completed. In a blind analysis, the data are divided into two parts, with one part used to define the analysis method and the other part used to test the method. The final analysis is only performed after the testing is complete, to prevent biases and ensure that the measurement is robust to systematic effects.


n particle physics, "pull plots" are graphical representations used to assess the agreement between the expected and observed values of a physical observable. Specifically, a pull plot shows the difference between the observed value of the observable and its expected value, divided by the uncertainty on the observed value. This quantity is called the "pull" of the measurement, and it is plotted as a histogram.

The pull plot is a powerful tool for identifying potential biases or systematic effects in a measurement. Ideally, the pull distribution should be centered around zero with a width of one, indicating that the observed values are consistent with the expected values within their uncertainties. Deviations from this expected behavior can indicate the presence of systematic effects or other issues with the measurement.

In practice, the pull distribution can take on various shapes, depending on the details of the measurement and the uncertainties involved. A pull distribution that is centered around a nonzero value may indicate a bias in the measurement, while a pull distribution with a width that is larger or smaller than expected may indicate an over- or underestimation of the uncertainties.
![[Pasted image 20230316195620.png]]
Pull plots are often used in combination with other methods to test and validate the measurements, such as comparing the data to Monte Carlo simulations or varying the experimental conditions. By examining the pull distribution and identifying any deviations from the expected behavior, researchers can improve the accuracy and precision of their measurements and ensure that they are robust to systematic effects.


Overview of Profile Likelihood : 
Here is a general overview of the procedure:

1.  Define the likelihood function: The likelihood function is a function of the model parameters, which are used to describe the expected signal and background events. The likelihood function can be constructed using Poisson statistics, taking into account both statistical and systematic uncertainties. The systematic uncertainties can be included by defining a set of nuisance parameters, which describe the size of the systematic uncertainties.
    
2.  Calculate the test statistic: The test statistic is a measure of the goodness-of-fit between the observed data and the expected signal and background events. One commonly used test statistic is the profile likelihood ratio, which is the ratio of the maximum likelihood values obtained by varying the signal strength parameter of interest (e.g. the cross section for a particular process) and keeping all other parameters fixed.
3. Compute the confidence intervals: The confidence intervals are obtained by calculating the distribution of the test statistic under the null hypothesis (i.e. the hypothesis that the signal strength is zero), and then determining the region of parameter space that is consistent with the observed data at a given confidence level. This can be done using various statistical techniques, such as the asymptotic approximation or Monte Carlo simulations.
    
 4. Incorporate systematic uncertainties: The systematic uncertainties can be incorporated by treating the nuisance parameters as additional free parameters in the likelihood function. The profile likelihood can then be computed by maximizing the likelihood over all parameters, including the nuisance parameters. The confidence intervals can be calculated by profiling over all parameters except for the parameter of interest.
    
 5.  Perform hypothesis tests: Hypothesis tests can be performed by comparing the test statistic to a distribution under a specific hypothesis. For example, one can test whether a particular signal process is present in the data by comparing the observed test statistic to the distribution expected under the null hypothesis. This can be done using the likelihood ratio test, which compares the maximum likelihood value under the alternative hypothesis (i.e. the hypothesis that the signal process is present) to the maximum likelihood value under the null hypothesis.

In step 1, systematic uncertainties are incorporated into the likelihood function through the use of nuisance parameters. This is done to account for the fact that the expected number of signal and background events may be affected by various sources of systematic uncertainty, such as uncertainties in the measurement of detector response or in the modeling of background processes. By including these systematic uncertainties in the likelihood function, one can obtain more accurate estimates of the model parameters and their uncertainties.

In step 5, systematic uncertainties are again incorporated into the analysis, but this time they are used to test different hypotheses. Specifically, one can use hypothesis tests to determine whether certain systematic uncertainties are needed to describe the data, or whether they can be ignored. This is important because some systematic uncertainties may have a larger impact on the results than others, and it is necessary to understand which uncertainties are most important in order to make robust conclusions.




h-fakes :
h-fake photons refer to photons that are produced as a result of hadronic processes, rather than from the decay of a neutral particle such as a meson or a neutral pion. In high energy physics, photons are often used to identify the presence of neutral particles, such as the Higgs boson, in the final state of particle collisions. However, photons produced from hadronic processes can be misidentified as signal photons, leading to a background contribution in the analysis.

The identification of h-fake photons can be challenging because they can have similar kinematic properties to signal photons. However, h-fake photons are often produced in association with jets or other hadronic activity, whereas signal photons are typically produced in isolation. This difference can be exploited by using a variety of identification algorithms, such as the shower shape of the photon in the detector, the presence or absence of associated tracks, or the relative isolation of the photon.

The estimation of h-fake photons is an important aspect of many particle physics analyses, as their misidentification can lead to a significant background contribution and reduce the sensitivity of the analysis to new physics signals. Various methods, including the data-driven method mentioned earlier, can be used to estimate the h-fake photon rate and reduce their contribution to the final analysis results.

\mu

In particle physics, the signal strength parameter, often denoted by the symbol $\mu$, is a measure of the strength of a signal relative to the expected background in a particular analysis. It is defined as the ratio of the observed number of events to the expected number of events from the signal and background processes, normalized to the expected signal strength in the absence of new physics.

Mathematically, the signal strength parameter can be expressed as:

μ=(Nobs−Nbkg)/Nsig,

where $N_{\text{obs}}$ is the observed number of events, $N_{\text{bkg}}$ is the expected number of events from background processes, and $N_{\text{sig}}$ is the expected number of events from the signal process.

The value of $\mu$ is typically used in statistical analyses to quantify the compatibility between the observed data and the expected signal and background predictions. If $\mu$ is consistent with 1 within the uncertainties, it suggests that the observed data is consistent with the background-only hypothesis, and no evidence for new physics is found. On the other hand, if $\mu$ is significantly larger than 1, it suggests the presence of a signal, and the statistical significance of the signal can be quantified using a test statistic such as the profile likelihood ratio or the significance level.


**sensitivity** 
In particle physics, the sensitivity of an analysis refers to the ability of the analysis to detect a signal, or a deviation from the expected background, with a certain level of statistical significance. In other words, it is a measure of how well an analysis can distinguish between the presence or absence of a signal, given the observed data and the expected background.

The sensitivity of an analysis depends on several factors, such as the total amount of data collected, the efficiency of the selection criteria used to isolate the signal from the background, and the accuracy of the background estimation methods. The sensitivity is usually expressed in terms of a statistical significance, which is a measure of the likelihood that the observed excess of events over the expected background is due to a signal, rather than statistical fluctuations.

A commonly used measure of statistical significance is the p-value, which represents the probability of observing a result as extreme or more extreme than the one observed, assuming the null hypothesis (i.e., the absence of a signal) is true. A p-value below a certain threshold, usually 0.05 or 0.01, is considered statistically significant and indicates the presence of a signal.




# Backgrounds - reducible or irreducible
In the context of data analysis or signal processing, the terms "irreducible background" and "reducible background" are often used to describe different sources of unwanted signals or noise. Here's a general explanation of how these terms are used and how to differentiate between them:

1. Irreducible Background: An irreducible background refers to a source of noise or unwanted signals that cannot be eliminated or reduced further by any means within the given experimental or analytical setup. It represents an inherent limitation or fundamental aspect of the system being studied. Irreducible backgrounds are typically caused by physical processes or phenomena that cannot be completely removed or controlled. For example, in astrophysics, the cosmic microwave background radiation is an irreducible background that pervades the entire universe.
    
2. Reducible Background: A reducible background, on the other hand, refers to noise or unwanted signals that can potentially be reduced or eliminated through appropriate data analysis techniques, experimental design, or by implementing suitable mitigation strategies. Reducible backgrounds are often associated with instrumental effects, systematic errors, or contamination from other sources. By employing various techniques such as calibration, data filtering, or applying statistical methods, it is possible to mitigate or remove some or all of the reducible background.
    

To differentiate between irreducible and reducible backgrounds, consider the following factors:

1. Nature of the source: Determine whether the source of the background is intrinsic to the system being studied (irreducible) or arises from external factors or experimental limitations (reducible).
    
2. Controllability: Assess whether the background can be controlled, minimized, or eliminated by modifying experimental parameters, improving instrumentation, or implementing data analysis techniques. If the background can be reduced by such means, it is likely to be a reducible background.
    
3. Data analysis techniques: Consider the available data analysis methods and statistical tools. If there are approaches that can be applied to suppress or eliminate the background, it suggests that it may be a reducible background. On the other hand, if the background remains present even after applying all possible mitigation techniques, it is likely an irreducible background.

# Application of unFolding
Unfolding is a technique commonly used in differential cross section measurements, but it is not limited to that specific application. Unfolding is a statistical and computational procedure used to correct for the effects of experimental resolution and detector response in order to obtain the true underlying distribution of a physical quantity.

Differential cross section measurements involve studying the dependence of a cross section (a measure of the likelihood of a particular scattering process) on one or more variables. Since experimental measurements are affected by the finite resolution and response of detectors, the observed distribution may be distorted or smeared compared to the true underlying distribution. Unfolding is used to recover the true distribution by deconvolving the measured distribution from the detector effects.

However, the concept of unfolding can be applied in various other scenarios beyond differential cross section measurements. It is commonly used in areas such as high-energy physics, nuclear physics, astrophysics, and other fields where precise measurements of physical quantities are essential. Unfolding techniques can be employed to correct for instrumental effects, background contamination, or other distortions in order to obtain more accurate estimates of the true underlying distributions.

----

# Systematics in Likelihood

In RooFit, systematic uncertainties are typically incorporated into the likelihood fitting process using nuisance parameters. Here's a concise outline of the process:

1. **Nominal Counts**: Let $e_i$ represent the nominal event count in bin $b_i$.

2. **Systematic Variation**: Let $s_i$ be the systematic effect on the counts, leading to varied counts $e_{i1}$ in bin $b_i$.

3. **Nuisance Parameters**: Introduce nuisance parameters $\theta_i$ to quantify the systematic uncertainties. These parameters allow the counts to vary within their systematic uncertainties.

4. **Modified Counts**: Define the modified counts $e_i(\theta_i)$ as a function of the nuisance parameters, often in the form:
   $e_i(\theta_i) = e_i + \theta_i \cdot \sigma_{s_i}$
   where $\sigma_{s_i}$ represents the standard deviation of the systematic effect.

5. **Likelihood Function**: The likelihood function $\mathcal{L}$ incorporates both the observed counts and the nuisance parameters. For observed counts $n_i$ in bin $b_i$, the likelihood function is:
  
   $\mathcal{L}(\{n_i\} | \{e_i(\theta_i)\}) = \prod_{i} \text{Poisson}(n_i | e_i(\theta_i)) \cdot \mathcal{G}(\theta_i | 0, 1)$
   
   where $\text{Poisson}(n_i | e_i(\theta_i))$ is the Poisson probability of observing $n_i$ events given the expected $e_i(\theta_i)$, and $\mathcal{G}(\theta_i | 0, 1)$ is a Gaussian constraint on the nuisance parameter $\theta_i$ with mean 0 and standard deviation 1.

6. **Fitting Process**: During the fitting process, the likelihood function is maximized with respect to both the main parameters of interest and the nuisance parameters $\theta_i$.

By including the nuisance parameters in the likelihood, RooFit effectively marginalizes over the systematic uncertainties, providing a more accurate estimate of the primary parameters while accounting for the uncertainties.



The $\theta$ nuisance parameter represents an additional variable introduced to model the systematic uncertainty in the measurement. It allows the fitting procedure to account for deviations due to systematic effects. Here's an analogous example to illustrate:

### Example: Measuring Length with Systematic Uncertainty

#### Scenario:
You want to measure the length of a rod using a ruler. The ruler itself may have a systematic error (e.g., it might be slightly stretched or compressed). This error is not known exactly but has an estimated uncertainty.

#### Steps:

1. **Nominal Measurement**: 
   - You measure the length of the rod and get a nominal value, say $L_0 = 10$ cm.

2. **Systematic Uncertainty**:
   - The ruler might be off by $\pm 0.1$ cm due to a manufacturing defect, so there's a systematic uncertainty $\sigma_s = 0.1$ cm.

3. **Nuisance Parameter ($\theta$)**:
   - Introduce a nuisance parameter $\theta$ to account for this systematic uncertainty. The true length $L$ is modeled as:
     \[
     $L(\theta) = L_0 + \theta \cdot \sigma_s$
     \]
   - Here, $\theta$ is a normally distributed variable with mean 0 and standard deviation 1, i.e., $\theta \sim \mathcal{N}(0, 1)$.

4. **Likelihood Function**:
   - When you fit the model, you construct a likelihood function that includes both the measurement and the nuisance parameter. For an observed length $L_{\text{obs}}$:
     $$ \mathcal{L}(L_{\text{obs}} | L_0, \theta) = \text{Normal}(L_{\text{obs}} | L_0 + \theta \cdot \sigma_s, \sigma_{\text{meas}}) $$
 where $\sigma_{\text{meas}}$ is the measurement uncertainty (e.g., reading error of the ruler).

5. **Constraint on $\theta$**:
   - You also include a Gaussian constraint on $\theta$ to reflect its uncertainty:
     \[
     $$ \mathcal{G}(\theta | 0, 1) = \frac{1}{\sqrt{2\pi}} e^{-\theta^2/2}$$
     \]

6. **Combined Likelihood**:
   - The combined likelihood function for the fit is:
     \[
     $$\mathcal{L}_{\text{total}} = \mathcal{L}(L_{\text{obs}} | L_0, \theta) \cdot \mathcal{G}(\theta | 0, 1)$$
     \]

#### Interpretation:
- During the fit, $\theta$ varies to account for the systematic uncertainty, while the main parameter (true length $L$) is estimated.
- The nuisance parameter $\theta$ effectively shifts the nominal length to account for potential systematic errors, constrained by its known uncertainty.

In RooFit, this approach allows systematic uncertainties to be incorporated directly into the fitting process, leading to more robust and accurate parameter estimates.


The nuisance parameter $\theta$ represents the range of possible true values due to the systematic uncertainty. Here's a detailed explanation:

### Accounting for Systematic Uncertainty with $\theta$

1. **Parameterization**:
   - The nuisance parameter $\theta$ parameterizes the systematic uncertainty. If the nominal value of the measurement is $e_i$ and the systematic uncertainty is $\sigma_{s_i}$, the true value considering the systematic effect can be expressed as:
     \[
     $$ e_i(\theta_i) = e_i + \theta_i \cdot \sigma_{s_i}        $$
     \]
   - Here, $\theta_i$ is a variable that allows $e_i$ to vary within the range dictated by the systematic uncertainty.

2. **Gaussian Constraint**:
   - The Gaussian constraint $\mathcal{G}(\theta_i | 0, 1)$ ensures that $\theta_i$ is normally distributed with a mean of 0 and a standard deviation of 1:
     \[$$
     \mathcal{G}(\theta_i | 0, 1) = \frac{1}{\sqrt{2\pi}} e^{-\theta_i^2/2}$$
     \]
   - This constraint reflects our prior knowledge about the systematic uncertainty: it is centered around zero (no systematic shift on average) and has a known spread (uncertainty).

3. **Likelihood Function**:
   - The total likelihood function, incorporating both the observed data and the nuisance parameters, is:
     \[$$
     \mathcal{L}(\{n_i\} | \{e_i(\theta_i)\}) = \prod_{i} \text{Poisson}(n_i | e_i + \theta_i \cdot \sigma_{s_i}) \cdot \mathcal{G}(\theta_i | 0, 1)
     $$\]
   - This likelihood function is maximized with respect to both the primary parameters of interest and the nuisance parameters $\theta_i$.

### Interpretation:

- **Range of True Values**:
  - The parameter $\theta_i$ allows the true value $e_i$ to vary within the range determined by the systematic uncertainty $\sigma_{s_i}$.
  - For example, if $\sigma_{s_i} = 0.1$, then $\theta_i$ can shift $e_i$ up or down by up to $0.1$ (depending on the value of $\theta_i$), effectively accounting for the systematic uncertainty.

- **Uncertainty on $\theta$**:
  - The Gaussian form $\mathcal{G}(\theta_i | 0, 1)$ itself provides an uncertainty on the nuisance parameter $\theta_i$. The standard deviation of 1 means that $\theta_i$ typically varies within $\pm 1$ around the mean of 0.
  - This constrains $\theta_i$ within a plausible range, reflecting our belief about the extent of the systematic uncertainty.

By incorporating $\theta$ and the Gaussian constraint into the likelihood function, RooFit takes into account the systematic uncertainties, allowing the fitting procedure to adjust for them and providing more accurate parameter estimates. This approach ensures that the entire range of possible true values due to systematic effects is considered, and the uncertainty on the nuisance parameter $\theta$ is also explicitly included in the analysis.


## Example:

Let's consider a simple illustrative example involving a single measurement with a systematic uncertainty.

### Example: Measuring a Quantity with Systematic Uncertainty

#### Scenario
- **True Value**: The true value of the quantity is \( T = 5 \).
- **Measurement**: You measure the quantity and get a nominal value \( M = 5.2 \).
- **Statistical Uncertainty**: The statistical uncertainty on the measurement is $\sigma_{\text{stat}}$ = 0.1.
- **Systematic Uncertainty**: There is a known systematic uncertainty \( $\sigma_{\text{sys}} = 0.2$).

### Incorporating Systematic Uncertainty

1. **Nuisance Parameter ($\theta$)**:
   - Introduce a nuisance parameter \(\theta\) to account for the systematic uncertainty. 
   - The measured value considering the systematic effect is modeled as:
     \[$$
     M(\theta) = M + \theta \cdot \sigma_{\text{sys}}
     $$\]
   - Here, \(\theta\) is a normally distributed variable with mean 0 and standard deviation 1.

2. **Likelihood Function**:
   - The likelihood function for observing the measured value \(M_{\text{obs}}\) given the true value \(T\) and the nuisance parameter \(\theta\) is:
     \[$$
     \mathcal{L}(M_{\text{obs}} | T, \theta) = \frac{1}{\sqrt{2\pi\sigma_{\text{stat}}^2}} \exp\left(-\frac{(M_{\text{obs}} - (T + \theta \cdot \sigma_{\text{sys}}))^2}{2\sigma_{\text{stat}}^2}\right)
     $$\]

3. **Constraint on $\theta$**:
   - Include a Gaussian constraint on \(\theta\):
     \[$$
     \mathcal{G}(\theta | 0, 1) = \frac{1}{\sqrt{2\pi}} \exp\left(-\frac{\theta^2}{2}\right)
     $$\]

4. **Combined Likelihood**:
   - The combined likelihood function is:
     \[$$
     \mathcal{L}_{\text{total}} = \mathcal{L}(M_{\text{obs}} | T, \theta) \cdot \mathcal{G}(\theta | 0, 1)
     $$\]

### Illustrative Example

- **True Value**: \( T = 5 \)
- **Measurement**: \( $M_{\text{obs}}$ = 5.2 \)
- **Statistical Uncertainty**: \( $\sigma_{\text{stat}} = 0.1$ \)
- **Systematic Uncertainty**: \( $\sigma_{\text{sys}} = 0.2$ \)

Let's calculate the likelihood for a few values of \(\theta\):

#### Case 1: $\theta = 0$ (No systematic shift)
\[$$
M(\theta = 0) = 5.2 + 0 \cdot 0.2 = 5.2
$$\]
\[$$
\mathcal{L}(5.2 | 5, 0) = \frac{1}{\sqrt{2\pi \cdot 0.1^2}} \exp\left(-\frac{(5.2 - 5)^2}{2 \cdot 0.1^2}\right) \approx 0.54
$$\]

#### Case 2: $\theta = 1$ (Positive systematic shift)
\[$$
M(\theta = 1) = 5.2 + 1 \cdot 0.2 = 5.4
$$\]
\[$$
\mathcal{L}(5.2 | 5, 1) = \frac{1}{\sqrt{2\pi \cdot 0.1^2}} \exp\left(-\frac{(5.2 - 5.4)^2}{2 \cdot 0.1^2}\right) \approx 0.01
$$\]

#### Case 3: $\theta = -1$ (Negative systematic shift)
\[$$
M(\theta = -1) = 5.2 - 1 \cdot 0.2 = 5.0
$$\]
\[$$
\mathcal{L}(5.2 | 5, -1) = \frac{1}{\sqrt{2\pi \cdot 0.1^2}} \exp\left(-\frac{(5.2 - 5.0)^2}{2 \cdot 0.1^2}\right) \approx 0.13
$$\]

### Interpretation

- The likelihood function values indicate how well the observed measurement fits the true value considering different systematic shifts.
- The Gaussian constraint $(\mathcal{G}(\theta | 0, 1))$ ensures $(\theta)$ is typically within $(\pm 1)$ (corresponding to the systematic uncertainty range of $(\pm 0.2)$).

By maximizing the combined likelihood function $(\mathcal{L}_{\text{total}})$, the fit will adjust both the true value \(T\) and the nuisance parameter $(\theta)$ to best explain the observed data while considering systematic uncertainties.



### Explanation

- The nuisance parameter $(\theta)$ is introduced to account for the systematic uncertainty in the measurement.
- It is typically assumed to follow a standard normal distribution \($\theta \sim \mathcal{N}(0, 1)$\), meaning $\(\theta\)$ has a mean of 0 and a standard deviation of 1.

### Interpretation of \(\theta\)

- \(\theta = 0\): This corresponds to no systematic shift (the nominal value).
- \(\theta = 1\): This corresponds to a shift by \(+1\) standard deviation of the systematic uncertainty.
- \(\theta = -1\): This corresponds to a shift by \(-1\) standard deviation of the systematic uncertainty.

### Effect on Measurement

If the systematic uncertainty $(\sigma_{s})$ is given, the measured value including the systematic effect can be expressed as:

$$ M(\theta) = M_{\text{nominal}} + \theta \cdot \sigma_{s} $$

- \(\theta = 1\): The measurement is shifted by \(+1 \sigma_s\):
  $$ M(1) = M_{\text{nominal}} + 1 \cdot \sigma_{s} $$
- \(\theta = -1\): The measurement is shifted by \(-1 \sigma_s\):
  $$ M(-1) = M_{\text{nominal}} - 1 \cdot \sigma_{s} $$

### Example

Given:
- Nominal measurement: \($M_{\text{nominal}} = 5.2$)
- Systematic uncertainty: \($\sigma_{s} = 0.2$)

For different values of \(\theta\):

- \(\theta = 0\): No shift
  $$ M(0) = 5.2 + 0 \cdot 0.2 = 5.2 $$
- \(\theta = 1\): Positive shift by \(+1 \sigma_s\)
  $$ M(1) = 5.2 + 1 \cdot 0.2 = 5.4 $$
- \(\theta = -1\): Negative shift by \(-1 \sigma_s\)
  $$ M(-1) = 5.2 - 1 \cdot 0.2 = 5.0 $$


Certainly, I'll make sure to use double $$ T $$
- **Nominal Measurement**: $$ M_{\text{nominal}} $$
- **Statistical Uncertainty**: $$ \sigma_{\text{stat}} $$
- **Systematic Uncertainty**: $$ \sigma_{s} $$

The measurement incorporating the systematic effect is:
$$ M(\theta) = M_{\text{nominal}} + \theta \cdot \sigma_{s} $$

The likelihood function for observing a measurement $$ M_{\text{obs}} $$ given the true value $$ T $$ and the nuisance parameter $$ \theta $$ is:
$$ \mathcal{L}(M_{\text{obs}} | T, \theta) = \frac{1}{\sqrt{2\pi\sigma_{\text{stat}}^2}} \exp\left(-\frac{(M_{\text{obs}} - (T + \theta \cdot \sigma_{s}))^2}{2\sigma_{\text{stat}}^2}\right) $$

### 2. Add Constraints for Nuisance Parameters

Include a Gaussian constraint on the nuisance parameter $$ \theta $$ to represent the prior knowledge of the systematic uncertainty:
$$ \mathcal{G}(\theta | 0, 1) = \frac{1}{\sqrt{2\pi}} \exp\left(-\frac{\theta^2}{2}\right) $$

### 3. Construct the Total Likelihood Function

Combine the measurement likelihood and the constraint on the nuisance parameter to form the total likelihood function:
$$ \mathcal{L}_{\text{total}} = \mathcal{L}(M_{\text{obs}} | T, \theta) \cdot \mathcal{G}(\theta | 0, 1) $$

### 4. Maximize the Likelihood Function

The goal is to find the values of the parameters $$ T $$ (the true value) and $$ \theta $$ (the nuisance parameter) that maximize the total likelihood function. This is done using numerical optimization techniques.

#### Steps in the Optimization Process:

1. **Initialize Parameters**: Start with initial guesses for $$ T $$ and $$ \theta $$.
2. **Evaluate Likelihood**: Compute the total likelihood function $$ \mathcal{L}_{\text{total}} $$ for the current parameter values.
3. **Adjust Parameters**: Use optimization algorithms (e.g., gradient ascent, Newton-Raphson, or other numerical methods) to adjust the parameters to increase the likelihood.
4. **Convergence Check**: Repeat the evaluation and adjustment steps until the parameters converge to values that maximize the likelihood function.

### 5. Obtain Parameter Estimates and Uncertainties

- **Best-fit Values**: The parameter values at which the total likelihood function is maximized are the best-fit estimates for $$ T $$ and $$ \theta $$.
- **Uncertainties**: The uncertainties on the parameters can be estimated from the shape of the likelihood function around the maximum. This is often done by finding the points where the log-likelihood decreases by 0.5 units from the maximum, which corresponds to a 68% confidence interval for normally distributed uncertainties.

### Example Summary

Given the measurement $$ M_{\text{obs}} = 5.2 $$, statistical uncertainty $$ \sigma_{\text{stat}} = 0.1 $$, and systematic uncertainty $$ \sigma_{s} = 0.2 $$:

1. **Initial Guess**: $$ T = 5 $$, $$ \theta = 0 $$
2. **Likelihood Evaluation**: Compute $$ \mathcal{L}_{\text{total}} $$ for initial values.
3. **Parameter Adjustment**: Adjust $$ T $$ and $$ \theta $$ to maximize $$ \mathcal{L}_{\text{total}} $$.
4. **Convergence**: Continue adjusting until $$ \mathcal{L}_{\text{total}} $$ is maximized.
5. **Result**: Obtain best-fit values for $$ T $$ and $$ \theta $$ along with their uncertainties.

This process ensures that both the primary parameters of interest and the nuisance parameters accounting for systematic uncertainties are optimally estimated, providing a robust fit to the observed data.






----



# Calculating errors (stat and such in HistFactory):
#statistics

https://www-zeuthen.desy.de/~wischnew/amanda/discussion/wgterror/working.html

Here you can find some details about how and why sum of squared weights is taken.


----

