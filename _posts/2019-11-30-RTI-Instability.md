---
layout: post_no_comments
title: "Properties of mixing caused by Rayleigh-Taylor
Instability"
excerpt_separator:  <!--more-->
categories:
  - Projects
tags:
  - University Projects
  - Hydrotechnical Engineering

last_modified_at: 2017-03-09T13:01:27-05:00
---

### Project Overview
<div class="message">
This is a small-scale literature review of mixing properties caused by Rayleigh-Taylor Instability, completed as part of the Environmental Hydraulics (CIVL 416) course at UBC.<br><br>

The contents of the final paper, submitted on November 30, 2018, are displayed below.

Click <a href="{{ site.url }}{{ site.baseurl }}/assets/pdfs/RTI Instability - Ali Fakhri.pdf" download>here</a> to download the pdf version.

</div>
<!--more-->
---

### 1.0 Introduction

Rayleigh-Taylor Instability (RTI) occurs at an interface where the pressure gradient opposes the density gradient [1]. This problem was first studied by Lord Rayleigh (1883), focusing on the instability at the interface of two fluids with different densities in a gravitational field [2]. Taylor (1950) later showed that this instability also arises when a fluid with lower density is accelerated into a fluid with higher density [2]. RTI is a very general problem and understanding it is important in wide range of fields ranging from oceanography to astrophysics. Some common occurrences of the RTI in oceans include river inflows, hydrothermal plumes and radiative cooling of the ocean surface [1]. The focus of this literature review is to understand various properties of mixing due to RTI.

### 2.0 Properties of RTI mixing

This section of the literature review is divided into two common themes based on the findings from the reviewed articles: the properties of mixing zone and mixing efficiency. The experimental set-up used in the cited literature is shown in Figure 1 [3]. The RTI is commenced by removing the horizontal barrier separating the two fluids. The discussion of key findings from the reviewed literature (three articles) follows.

[![Experiment configuration]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/experiment_config1.png)]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/experiment_config1.png){: .center-image }
*Figure 1: Sketch of the experimental configuration. The symbols are defined in the text [3].*{: .center-image }


### 2.1 Mixing Zone

The evolution of the mixing zone, the region where both lighter and denser fluids are found, in RTI has been a subject of extensive study [2]. Dalziel et al. [2] define the width of the mixing zone as the depth at which the plane-averaged concentration profile reaches a defined threshold concentration level [2]. For flows with high Reynolds number, the governing parameter in the RTI is found to be the Atwood number,

$$A=\frac{\rho_{1}-\rho_{2}}{\rho_{2}+\rho_{2}}$$

where $$\rho_{1}$$ and $$\rho_{2}$$ are the densities of the fluid above and below the RTI interface, respectively [ 2 ]. For an inviscid flow, dimensional analysis suggests that the penetration of either fluid into another should follow

$$h_{i}=\alpha_{i} A g t^{2}, \quad i=1,2$$

where $$\alpha_{i}$$ is a dimensionless constant [2]. For flows with small density difference, $$A \ll 1$$, the instability is symmetric; the penetration of both fluids occurs at the same rate ($$\alpha_{1}=\alpha_{2}$$) [2]. However, if the density difference is significant, the lighter fluid becomes more active which results in $$\alpha_{i}<\alpha_{i}$$ [2]. The characteristic time scale for the examined flows is given by $$\left(\frac{H}{A g}\right)^{\frac{1}{2}}$$, where $$g$$ is gravitational acceleration and $$H$$ is the depth of the tank in the experimental set-up [2]. It is often favored to nondimensionalize the mixing zone width as

$$\delta_{i}=\frac{h_{i}}{H}=\alpha_{i} \tau^{2}, \quad i=1,2$$

where

$$\tau=\left(\frac{A g}{H}\right)^{\frac{1}{2}} t$$

is the dimensionless time [2]. When the mixing zone reaches the upper and lower boundaries of the tank, the fluids overturn and a stable stratification is established [2][3].

Generally, to compare the analysis of flows from different experimental set-ups, researchers use the growth rate constants $$\alpha_{i}$$ [2]. However, Linden et al. [3] and Dalziel et al. [2] agree that is difficult to give a reasonable, unambiguous estimate of this parameter; this difficulty is attributed to the inhomogeneous structure of the flow and the sensitivity of the growth rate constant to the method used to calculate it [2]. Nonetheless, both Linden et al. [3] and Dalziel et al. [2] estimate the value of $$\alpha$$ to be ~ 0. 04. Dalziel et al. [2] further conclude that the growth rate constant is not a very useful measure of the RTI development and suggest using additional measures for comparing experiment and numerical simulations, such as finding the correlation coefficient between data sets. For instance, the frequency of the relationship between the averaged concentration values from the experiment and numerical simulations presented in the scatter plots in Figure 2 is recommended for comparing structure and growth rate of the mixing zone [2]. From these scatter plots, Dalziel et al. [2] conclude that the experiment is in closer agreement with the numerical simulation that incorporates the effects of barrier removal compared to the simulation that has idealized initial conditions.

[![Scatter plots]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/scatter_plots.png)]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/scatter_plots.png)
*Figure 2 : Scatter plot of mean concentration between: experiments and idealized simulations (a), and experiments and barrier simulations (b). In both cases the simulations occupy the vertical axis and the experiments the horizontal. The frequency of the relationship is represented as a greyscale [2].*

### 2.2 Mixing Efficiency

Mixing efficiency is often used to characterize turbulent mixing in stratified flows [1]. It is an important parameter in oceanography, since the overall stratification of an ocean in a steady-state is maintained via mixing and mixing efficiency is required to determine the total amount of mixing [1].

Davies Wykes and Dalziel [1] define mixing efficiency as a ratio of change in the minimum potential energy (i.e. if the fluids were to interchange positions without any mixing until equilibrium is reached) over the change in the available potential energy of a flow (assuming initial and final states of the experiment are quiescent):

$$n=\frac{\left|\Delta E_{b}\right|}{\left|\Delta E_{a}\right|}$$

The reader is referred to [1] for detailed derivation of this parameter. In general, the maximum mixing efficiency of a system is limited to one by energetics [1]. However, for some flow systems such as the classical case of RTI (Figure 3 a), the mixing efficiency limit is imposed by the initial configurations of the system, since mixing is stopped once the density field becomes homogenous [1]. The limits imposed by initial configurations can be avoided if only stable stratification confines the RTI interface (Figure 3 b-d) [1].

[![Sketches of different cases]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/case_sketches.png)]({{ site.url }}{{ site.baseurl }}/assets/RTI_images/case_sketches.png)
*Figure 3: Sketch of classical case of RTI (a) [$$n_p$$=0. 5 ] and different initial density stratification profiles used in experiments (b-d) [$$n_p$$=0. 68 , 0. 75 , 0. 78 , respectively] [1].*

Davies Wykes and Dalziel [1] define a region as perfectly mixed once the density gradient in that region becomes zero. The perfect mixing efficiency $$n_p$$, was calculated assuming the central mixing region is perfectly mixed and stratification outside of this region is unchanged from the initial state [1]. The authors of [1] obtained values of $$n_p$$ for the profiles shown in Figure 3 (b-d), which were then used to determine the extent of mixing efficiency in the experiment. It was found that the mixing efficiency generally exceeds 95% of $$n_p$$ and the authors suggest that assuming the mixing efficiency of naturally occurring stratified shear flows to be 0.2 (as is typically done) is erroneous [1].

For the classical case of RTI shown in Figure 3 (a), the maximum mixing efficiency is 0.5 [1]. Linden et al. [3] reported a mixing efficiency value of 0.35 measured from previous laboratory experiments and values of 0.48 and 0.47 obtained from numerical simulations of RTI mixing between two homogenous layers (Figure 3 a). The latter values are in closer agreement with the maximum mixing efficiency limit for this case ( $$n_p$$=0. 5 ) [1]. The authors attribute the variation in mixing efficiency between the experiment and numerical simulations to the observed large-scale overturning motions caused by the removal of the dividing barrier, suggesting it may have resulted in the lower experimental mixing efficiency [ 3 ].

The effects of barrier removal in stratified RTI profiles were investigated in [1], particularly the variation of mixing efficiency with barrier withdrawal speed. Contrary to their expectations, Davies Wykes and Dalziel [1] found that mixing efficiency is reduced with an increase in barrier withdrawal speed. The additional kinetic energy introduced from the barrier removal was observed to preferentially sort the density profile in the central region rather than contribute to the mixing [1], thereby affirming the assumption in [3] that barrier withdrawal reduces mixing efficiency.

The effect of Atwood number on mixing efficiency of a linear stratified profile (Figure 3 c) was also investigated in [1]. The mixing efficiency was found to increase with increase in Atwood number [1]. This relation is also confirmed in [3] for the linear density profile (Figure 3 a). Davies Wykes and Dalziel [1] warn that there is some uncertainty whether the increase in the mixing efficiency can be directly attributed to the Atwood number or to its influence on the Reynolds number, defined here as

$$R_{e}=h \dot{h} / v$$

where $$h$$ is the height of the mixing zone and $$v$$ is the kinematic viscosity.

### 3.0 Summary

The focus of this literature review was to investigate some properties of the mixing that occurs due to RTI. The development of the mixing region in the classical case of RTI was examined and it was found that only using the growth rate constant, $$\alpha_{i}$$, for comparing analysis of flows is inadequate, since it is difficult to provide an unambiguous estimate of this parameter [2]. Dalziel et al. [2] recommend also finding the correlation between data sets with scatter plots of the frequency of their relation (Figure 2). The mixing efficiency of mixing due to RTI was shown to generally exceed 95% of the perfect mixing efficiency $$n_p$$ and it was concluded that assuming $$n$$= 0.2 for the naturally occurring stratified shear flows is unjustified [1]. The removal of the horizontal barrier in the experiments (i.e. adding initial kinetic energy to the system) was shown to reduce the mixing efficiency [1]. In contrast, the increase in Atwood numbers resulted in the increase in the mixing efficiency [1][3]. Overall, this endeavour helped to better understand the properties of mixing due to RTI. It was found that this instability generally results in relatively high mixing efficiency and its complicated nature requires further measures, in addition to the growth rate constant, for comparing the structure and growth of the mixing zone.

### REFERENCES

[1] M. Davies Wykes and S. Dalziel, "Efficient mixing in stratified flows: experimental
study of a Rayleigh–Taylor unstable interface within an otherwise stable stratification",
*Journal of Fluid Mechanics*, vol. 756, pp. 1027-1057, Sept. 2014.

[2] S. Dalziel, P. Linden and D. Youngs, "Self-similarity and internal structure of turbulence
induced by Rayleigh–Taylor instability", *Journal of Fluid Mechanics*, vol. 399, pp. 1-48,
1999.

[3] P. Linden, J. Redondo and D. Youngs, "Molecular mixing in Rayleigh–Taylor
instability", *Journal of Fluid Mechanics*, vol. 265, p. 97, 1994.
