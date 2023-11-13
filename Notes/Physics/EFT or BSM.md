## Intro :

Taken below is from a cern excerpt :
"It is necessary to establish a fresh framework that goes beyond the traditional interpretation of Higgs production rates and incorporates shape information, Higgs self-interaction rates and other SM processes including Electroweak precision data and also analyses of processes including top quarks production.

The absence of definitive signals indicating physics beyond the SM at the LHC suggests the possibility of a scale separation between the SM and any potential new physics at higher energies. This motivates the utilization of the Standard Model Effective Field Theory (SMEFT) [[20](https://arxiv.org/abs/1706.08945)] as a valuable tool for indirectly searching for new physics in LHC data [read also a previous [EP news article](https://ep-news.web.cern.ch/content/lhc-takes-smeft-challenge)]. The SMEFT offers the advantages of (near) model-independence, systematic improvement capabilities, and the ability to simultaneously leverage multiple datasets.

Effective Filed theories introduce new-physics states at a high mass scale Λ, significantly larger than the electroweak scale. By expanding in terms of E/Λ, where E represents the typical energy exchanged in a process, the theory provides predictions for experimental observables. This expansion is achieved through a series of operators, which are constructed as gauge-invariant combinations of SM fields with energy dimensions greater than four.

By measuring observables that are sensitive to the effects of SMEFT operators, it becomes possible to constrain the values of c(d)/Λ4d, where c(d)) represents the Wilson coefficients associated with the dimension-d operators O(d). The leading effects of new physics are expected to be captured by dimension-six operators, as higher-dimensional operators are suppressed by greater powers of Λ−1. The extensive measurements conducted by ATLAS, focusing on electroweak interactions, the Higgs boson, and top quarks, exhibit sensitivity to a wide range of operators that impact various aspects of particle interactions. These operators influence Higgs boson couplings, self-interactions of weak bosons, couplings between weak bosons and fermions, as well as four-fermion couplings. To achieve the best possible sensitivity and disentangle the effects of these operators, it is necessary to combine a diverse set of measurements. A first measurement has been performed by the ATLAS Collaboration with the Run2 data [[21](https://cds.cern.ch/record/2816369/files/ATL-PHYS-PUB-2022-037.pdf)]. Also CP violating effects can be included.

Conducting a global analysis of constraints on the Wilson coefficients of the SMEFT is of utmost importance when allowing more than a few Wilson coefficients to be non-zero. This is due to the fact that numerous SMEFT operators contribute to multiple observables, emphasizing the need to avoid analyzing different measurement classes in isolation. This feature becomes increasingly important as the statistics of the ATLAS data increases. During the analysis of Run 3, a significant emphasis will be placed on utilizing Effective Field Theories (EFTs). This endeavor holds particular significance as it aims to uncover potential deviations from the Standard Model (SM) that could be amplified through the comprehensive interpretation of diverse measurements. Furthermore, the outcomes of these investigations will play a crucial role in guiding our future research endeavors at the HL-LHC."

---
## Basics of EFT (with examples):

Effective Field Theory (EFT) is a powerful framework used in theoretical physics to describe phenomena at a given energy scale, while "integrating out" or ignoring the details of the underlying higher-energy or shorter-distance scales. This concept can be applied to a wide range of contexts, from particle physics to condensed matter.

### Basic Idea

Imagine you're watching a movie on an old TV screen. If you stand too close, you see individual pixels, but if you step back, you see a clear picture. EFT works similarly. Instead of focusing on every detail (or every pixel), it gives us the big picture.

In EFT, we ignore the details of some high-energy interactions and only focus on long-range or low-energy processes.

### Formalism

The idea is to express the Lagrangian (a mathematical object that describes the dynamics of a system) in terms of fields that are relevant at the scale of interest. The Lagrangian will have a series of terms, organized by their dimension:

LEFT=LSM+1ΛL5+1Λ2L6+…LEFT​=LSM​+Λ1​L5​+Λ21​L6​+…

Here:

- LSMLSM​ is the Standard Model Lagrangian or some other low-energy Lagrangian.
- ΛΛ is the "cutoff" scale, where new physics might appear.
- L5L5​, L6L6​, etc., are operators of higher dimension which are suppressed by the corresponding powers of ΛΛ.

### Application

Let's discuss one of the most famous examples: Fermi's theory of beta decay. Before the discovery of the W and Z bosons, Fermi described weak interactions in terms of a four-fermion interaction. This interaction looked like direct contact between particles, with no mediator.

The Fermi interaction had the form:

LFermi=GF2ψˉνγμ(1−γ5)ψeψˉnγμ(1−γ5)ψpLFermi​=2

​GF​​ψˉ​ν​γμ(1−γ5​)ψe​ψˉ​n​γμ​(1−γ5​)ψp​

Where GFGF​ is Fermi's constant, and the ψψ terms represent various fermion fields.

Later, it was discovered that this interaction was actually mediated by the exchange of a W boson. However, for energies much less than the W boson mass, the Fermi theory provides a good approximation.

### Why is EFT Powerful?

1. **Separation of Scales**: We can effectively deal with physics at a particular scale without knowing the details of higher scales.
    
2. **Universality**: EFTs can describe a broad class of underlying theories, as long as they have the same symmetries and particle content at low energies.
    
3. **Systematic Improvements**: If we want to refine our predictions, we can systematically include higher-dimensional operators, suppressed by higher powers of the scale ΛΛ.
    

### Limitations

- **Accuracy**: The accuracy is restricted to a specific range of energy scales.
    
- **New Physics**: EFT cannot predict new particles or phenomena but can hint at their presence through deviations from expected results.
    

### In Conclusion

Effective Field Theories are a cornerstone of modern theoretical physics, providing a systematic way to describe phenomena when a full microscopic description is either unknown or too complicated to handle. They are widely used in particle physics, nuclear physics, and condensed matter physics. The ability to "integrate out" high-energy details and focus on relevant low-energy processes is what makes EFTs incredibly versatile and powerful.


$$ \LARGE{ \textbf{LLPs also form some part.}}$$

#llp #lhc [[LLP]]   : see here.

---

## Conflating EFT and renormalization : 
Effective Field Theory (EFT) and renormalization are deeply connected concepts, and they share some similarities in philosophy, but they are used for different purposes.

### Renormalization

Renormalization is a procedure to deal with the divergences that arise in the perturbative evaluation of quantum field theory (QFT) observables, especially in the context of the Standard Model (SM). When we calculate certain quantities in QFT using Feynman diagrams, we sometimes encounter infinite results, which are physically nonsensical. Renormalization provides a systematic way to absorb these infinities into the redefinition of parameters (like masses and couplings) of the theory, making predictions finite and physically meaningful.

### EFT and Renormalization

Effective Field Theories are based on the same basic idea as renormalization: separating different energy scales. Just like in renormalization, where we absorb high-energy or short-distance information into redefined parameters, in EFT we "integrate out" the high-energy or short-distance degrees of freedom to focus on the low-energy or long-distance physics.

However, while renormalization is about handling infinities and making QFT calculations meaningful, EFT is about simplifying the description of a system by focusing on the relevant degrees of freedom at a particular energy scale.

### Relationship with the Standard Model

When we use EFT in the context of the SM, it's often to describe physics that might exist beyond the SM. Since we don't know the exact form of a potential "Beyond the Standard Model" (BSM) theory, we use EFT to parametrize our ignorance. We add to the SM Lagrangian all possible higher-dimensional operators consistent with the SM symmetries, suppressed by powers of a scale ΛΛ which is the energy scale of the new physics.

As we perform calculations in this EFT, we might encounter divergences. Here's where renormalization comes in again. The renormalization process in EFT can give us insights about the structure of the UV (ultraviolet, or high-energy) completion of the theory - the more fundamental theory that the EFT is an approximation of.

### In Summary

- **Renormalization** is a technique to handle infinities in QFT calculations.
- **EFT** is a framework to describe physics at a given energy scale by integrating out higher energy scales.
- Both concepts involve the idea of separating or handling different energy scales in a QFT.
- EFT allows for a parametrized description of unknown higher-scale physics, like BSM physics. When performing calculations in such an EFT, renormalization techniques might be needed.
### Relationship with Renormalization:

When we do loop calculations in an EFT, we again encounter divergences, but some of these can be absorbed by redefining the coefficients of the higher-dimensional operators (similar to how we redefine mass and charge in QED). If an EFT is well-defined, any observable we compute should be independent of the scale at which we separate "low-energy" from "high-energy."

For instance, when doing calculations in the Fermi theory, we'd encounter divergences that would be absorbed by redefining the Fermi constant, GFGF​. However, if we were doing the calculations in the full theory with the W boson, these divergences would be absorbed into the definitions of other parameters, like the W boson mass or the weak coupling constant.

In essence, while both renormalization and EFT involve separating or handling different energy scales, the former deals directly with the divergences of QFT, while the latter offers a simplified description of phenomena by ignoring high-energy details. Both are crucial for making meaningful and accurate predictions in particle physics.


---


$\[ e(\mu) = Z_e(\mu) e_{\text{bare}} \]$

## Renormalization

In quantum field theory, infinities might arise when you calculate certain quantities. Renormalization is a procedure to rid the theory of these infinities.

The basic idea is:

$$ e(\mu) = Z_e(\mu) e_{\text{bare}} $$

$$ e(\mu) = Z_e(\mu) e_{\text{bare}} $$

Where:
- $e(\mu)$ is the renormalized charge.
- $e_{\text{bare}}$ is the bare charge.
- $Z_e(\mu)$ is the renormalization constant.

## Effective Field Theory (EFT)

EFT is a way to describe physical phenomena at a particular scale. The Lagrangian for an EFT is:


$$ \mathcal{L}_{\text{EFT}} = \mathcal{L}_{\text{SM}} + \sum_i \frac{c_i}{\Lambda^{d_i}} \mathcal{O}_i $$


Where:
- $\mathcal{L}_{\text{SM}}$ is the Standard Model Lagrangian.
- $\mathcal{O}_i$ are operators representing new interactions.
- $c_i$ are the coefficients.
- $\Lambda$ is the scale of new physics.
- $d_i$ is the dimension of the operator $\mathcal{O}_i$.

nice explanation by Knut in his atlas lecture series first talk :
https://indico.cern.ch/event/1338871/attachments/2745421/4782252/video1080087758.mp4


---
