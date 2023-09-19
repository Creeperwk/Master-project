# Master-project(Association of Stress and connectivity in UK lakes with beetles species richness)

## Introduction
Therefore the "Hydroscape" project funded by the UK Natural Environment Research Council (NERC). This project delves deep into the exploration of the interactions between stressors and connectivity and how they affect biodiversity and ecosystem functionality in the UK's freshwater systems. With a spotlight on some specific species such as beetles, the project aims to demystify the mutual effects of stress and connectivity on the species diversity. 

## Study area and dataset
This study is based on Great Britain islands(Some offshore islands not included: Isle of Man, Shetlands etc.), an island in the North Atlantic Ocean with an area of 209,331 $km^2$ and contains over 40,000 water bodies in total.The secondary dataset we used in this project is base on the compilation from Dr. Alan Law and Dr. Philip Taylor from the project NERC. The collected dataset comprises 1418 samples from various lakes throughout the UK and each of them have 26 different variables. They are categorized they belongs to three facet concerning the lakes: Lake typology, Connectivity and Stressors.

## Task
The objective of this program is to answer the following questions:  
(i) What are the main relationships between species richness and surrounding land cover stressors?  
(ii) What is the primary correlation between species diversity in freshwaters and connectivity to its buffers?  
(iii) Does the association between species distribution and stress factors change depending on connectivity to other nearby freshwaters?  

## Method
A Generalized Linear Model(GLM) will typically be the first choice the count response variable, which is the number of species in a certain sample. Poisson/Quasi-poisson/Negative binomial GLM should be considered based on different level of dispersion. In this case, Negative binomial GLM is selected to give another penalty to the overdispersion in this case. AIC is used for evaluating the goodness of fit when selecting the most appropriate model from among multiple fitted options. Dispersion parameter k is used to check the amount of overdispersion of this model.

## Conclusion
Results have shown the significance on specific variables: "Land.MeanT ", "Land.watersports" and "Land.riverlength" etc have good impact on species richness. Moreover, "Land.fishing", "Land.lakeper" etc have negative affect on the diversity. 
On the other hand, the variables: "Land.pondarea","Land.pondper","Land.obstacles" from the connectivity have interactions with some of the stressors variables which do have influence on species richness.
The model still have reveal a measurable degree of uncertainty and bias. Which some results might be affected by a certain number of extreme values in the data.

