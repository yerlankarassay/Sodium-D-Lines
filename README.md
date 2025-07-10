# Sodium-D-Lines
Used a Michelson Interferometer setup to measure the wavelength difference between the Sodium's Emission Lines (denoted as D-Lines).

Precision Interferometer
Yerlan Karassay
L1 Discovery Labs, Lab Group: B, Lab Date: Thursday
Submitted: 19/03/2025, Date of Experiment: 20/02/2025

 
	Introduction

Every element has characteristic emission lines that are unique to the element. The characteristic emission lines can be investigated when hot and dense elements cause the electrons in specific orbitals to undergo excitation, absorbing energy, then releasing back that energy by emitting photons of energy that corresponds to the orbital energy difference of the given element. In this experiment, a sodium lamp excites electrons of Na and produces characteristic emission lines, D1 and D2 that have corresponding wavelengths, λ1 and λ2. Prism spectroscopy method to disperse the constituent emission wavelengths of Na lacks precision to calculate difference in wavelengths that are a few Angstroms apart, only being capable of calculating the average wavelength, λmean, of the emission lines. The aim of this experiment is to use an interferometer in its Michelson mode of operation to separate the D1 and D2 emission lines and calculate the difference between their wavelengths.
Constructive interference occurs when monochromatic light sources that are in phase with each other superpose to form bright fringes of higher intensity. On the other hand, destructive interference occurs when lights that are out of phase superpose to form dim fringes of low intensity. [2]
2. Method
 
Fig. 1: Michelson interferometer consists of a light source that sends out a beam onto the beam splitter with half-silvered silvered surface. The micrometre screw gauge with a gearing factor 5 can be used to adjust the distance d1 while the stationary mirror ensures the distance d2 is constant. The observer can look at the resulting interference pattern from a hole that is directed on a diffuser plate. 

The idea behind the Michelson interferometer setup in this experiment is illustrated in Fig. 1. The beam that is incident on the beam splitter is split into two beams, one beam passes through and hits the mirror M2 then reflects to hit the other side of the beam splitter to be reflected once again by the beam splitter to be transmitted to the observer. Whereas the other beam is reflected by the beam splitter and reflected again by mirror M1 to be transmitted through the beam splitter to the observer. As each beam travels twice the length of their respective paths, d1 and d2, the difference between the path lengths travelled by each beam is given by the equation below (1).

█(∆d=2(d_1-d_2 )  #(1))

When the path difference, Δd, is an integer multiple of wavelength of the beam, λ, then the two beams are in phase to constructively interfere and produce defined circular fringes that can be seen by the observer. Whereas when Δd is a half-integer multiple of the wavelength, then the two beams are out of phase to destructively interfere, and a dark fringe is seen by the observer. [2]

The mirrors M1 and M2 were aligned to be perpendicular to each other by using the metal screws so the two beams overlapped to produce a single circular image, which ensures that the two beams interfere.

The distance of the mirror M1 from the beam splitter was varied using the micrometre screw gauge to change the path difference of D1 and D2 lines to vary how each wavelength of beam interferes with itself individually.
The observed fringe pattern arises due to the combination of interference patterns from D1 and D2. Observing bright concentric circles meant that D1 and D2 both constructively interfered to reinforce each other’s bright fringes. Observing a uniformly yellow image meant that for D1 and D2, when one interfered constructively, the other interfered destructively.

█(s=nt #(2))

By varying the distance of the adjustable mirror, thus changing the length d1 while d2 is kept constant, the micrometre reading, s, could be plotted against the order of interference pattern, n, that are denoted by half integers. A correspondent graph was plotted for the linear relationship given in the equation above (2). The gradient, m, corresponding to the value of t represents the micrometre reading that creates the path difference needed to skip between a whole cycle of maxima (or minima).

█(t=(λ_1 λ_2)/2(λ_1-λ_2 ) ≈λ^2/2(λ_1-λ_2 ) #(3))

Due to the values of λ1 and λ2 being so small in magnitude, the equation above (3) could be obtained by approximating them to be equal. The latter equation (3) is rearranged to make (λ1 - λ2) the subject, followed by subbing in the known value of λ_mean= (589.294 ± 0.001) ×10-9 m [1] and then the calculated value of t could be subbed into the equation after dividing t by 5 to account for the micrometre gearing factor. A value for (λ1 - λ2), which is the aim of this experiment, Δλ, is obtained. 

3. Results

 

Fig. 2: The micrometre readings as a function of 12 orders of successive interference patterns starting from the first pattern of maximum fringe visibility. The vertical error bars for most of the data points are not visible due to similar micrometre measurements in each trial. The residual plot reflects the variation of each data point from the predicted value given by the trendline and the histogram presents information about the distribution of residuals.

The measurements of micrometre readings corresponding to successive orders of maxima or minima were combined to show a positive linear relationship between the variables. The gradient of the straight-line regression graph shown in Fig. 2 was calculated as t= (1.49 ± 0.01) ×10-3 m using Python regression line library such a SciPy.
The wavelength difference between sodium D1 and D2 lines were calculated as Δλ= (5.83±0.04) ×10-10 m.

4. Discussion

The accepted literature value for the wavelength difference between sodium D1 and D2 lines in metres are given as Δλ = 6.01 ×10-10 m [1]. This means that our experimental value, Δλ= (5.83±0.04) ×10-10 m, differs from the accepted value by 4.25 standard errors given our standard error is calculated as σ = 0.04×10-10 m [4]. The percentage difference between the results is 2.85% but the 4.25 standard error deviation suggests a systematic error. Due to the lack of qualitative methods used in the process of identification of the patterns with maximum fringe visibility, looking directly with my eye through the diffusing plate has possibly caused a systematic error in the experiment. Especially the first 6 measurements of maximum fringe visibility were very challenging to identify due to the limited number of fringes in the first few orders of maxima and the blurry pattern. Misjudging the maximum fringe visibility throughout taking readings likely caused me to take smaller micrometre readings throughout, thus reducing the value of t. Furthermore, due to the absence of a lab partner and having taken only two sets of measurements for the same 12 orders of interference patterns, I likely stopped early and taken readings at the same positions in the second sets of measurements leading to the histogram plot in Fig. 2 which was expected to resemble a normal distribution. The subjectivity of measurements could be seen by the large uncertainty in the 8th maximum fringe visibility that suggests that I severely misidentified the maxima in successive trials.
Integrating an independent measurer other than myself and having approximately 10 sets of measurements would lead to unbiased measurements which would improve the accuracy of the measurements for each interference pattern position, leading to a more accurate gradient calculation in Fig. 2. Further improvements can be made by for identifying the true positions of interference patterns using an intensity detector which quantifies the maximum fringe visibility into higher values of intensity and lower values of intensity for minimum fringe visibility.
The work conducted in this experiment has various potential future applications in science and astronomy. The interferometric methods used in this experiment can be used to study distant stars and galaxies as their chemical composition can be deduced from their atomic spectra [3]. The precise measurement techniques such as of interferometers can be used to measure the wavelengths of spectral lines to be then compared to known values of known spectral line values of elements, giving valuable insights into the given star’s stellar evolution.

5. Conclusions

In this experiment, an Interferometer in its Michelson mode of operation was used to determine the wavelength difference between sodium D1 and D2 lines, which are key characteristics of the sodium emission spectrum. By analysing the interference fringes, the wavelength difference between sodium D1 and D2 lines were calculated as Δλ= (5.83±0.04) ×10-10 m. This result is only two standard errors away from the accepted experimental value of Δλ= (5.97±0.001) ×10-10 m, which demonstrates the effectiveness of interferometers in measuring small distances that require high levels of precision.
This experiment shows the utility of interferometers in understanding atomic spectra and shows its potential applications in spectroscopy which ties back to the aims outlined in the introduction, which emphasised the need for high precision methods to study atomic structures of elements [3].
References

[1] NIST Atomic Spectra Database (ASD), Version 5.12 National Institute of Standards and Technology
[2] Hecht, E (2017). Optics (5th Edition). Pearson (Chapter 9: Interference)
[3] Malacara, D. (2007) Optical Shop Testing (3rd Edition). Wiley. (Chapter 5: Michelson Interferometers)
[4] I. G. Hughes and T. P. A. Hase, Measurements and their Uncertainties (Oxford University Press, 2010). 
Error Appendix

This section follows error propagation methods discussed in Hughes and Hase [4], the vertical error bars in the y-axis of the Fig.1 was obtained using Eq. 4 where the error in the micrometre reading, α_s, was the standard error in the mean of the measurements. 

█(α_s=σ_(N-1)/√N.#(4))

We had two sets of measurements for the micrometre reading which sets N=2, to calculate the standard error using the given equation (4). The standard deviation of the sample, σN-1, was calculated in Excel. Fig. 1 doesn’t include horizontal error bars associated with the order of interference pattern, n, as they represent discrete half integer values that are exact and not subject to uncertainty in measurement.

The micrometre reading corresponding to the separation for one cycle skip, t, corresponded to gradient value of the line of best fit in Fig.1. The gradient, m, of the plot and its uncertainty αm were calculated using Python’s SciPy. Optimise library where the weighted least-squares method was implemented, yielding the final value for the gradient:  m = (1.49 ±0.01) × 10-3 m.


The error in t=(1.49±0.01)×10^(-3)  m and the mean wavelength of the D1 and D2 lines λ_mean= (589.294 ± 0.001) ×10-9 m [1], were propagated for our desired value of difference in wavelength Δλ, using functional approach of error propagation Δλ given by Eq.4. The uncertainty in the multivariable function, Δλ (t, λ_mean ) is calculated by considering the effect of αt and α_(λ_mean )  respectively.

█(α_∆λ^(λ_mean )=|Δλ (t ̅,λ ̅_mean+ α_λmean )-Δλ (t ̅,λ ̅_mean  )|#(5))


█(α_∆λ^t=|Δλ (t ̅+α_t,λ ̅_mean )-Δλ (t ̅,λ ̅_mean  )|#(6))



The associated errors due to each variable t and  λ_mean were propagated using the equation given below (7), where the error in difference in wavelength depended on the error in t.
█(α_∆λ=√((α_∆λ^(λ_mean ) )^2+(α_∆λ^t )^2   ).#(7)) 
 
Scientific Summary for a General Audience

Every element has fingerprints that are called characteristic emission lines. These emission lines are unique to each element, and they correspond to specific wavelengths of light when the element absorbs energy. In this experiment, we have investigated the element sodium, which is a common element found in places like streetlamps to table salts. Sodium produces two emission lines called D1 and D2 which are so close in wavelength that they are indistinguishable unless you know any high precision measuring techniques. Luckily, we know a method called interferometry that can measure minute distances by splitting a beam of light into two different paths and then recombining them resulting in the formation of various patterns. These patterns are sensitive to smallest changes in the travel distances of the beam; thus, the scientist can deduce minute distances such as the difference between the sodium D1 and D2 lines by analysing these patterns. This experiment showcases the effectiveness of interferometers in measuring vanishingly small distances which is vital in many technologies from enhancing the precision of GPS systems to advancing medical imaging technologies. In summary, fundamental properties of light such as interference can be used to advance technology and scientific research.


