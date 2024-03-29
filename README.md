# Publication bias impacts on effect size, statistical power, and magnitude  (Type M) and sign (Type S) errors in ecology and evolutionary biology

# Citation
Yefeng Yang*, Alfredo Sánchez-Tójar, Rose E. O’Dea, Daniel W.A. Noble, Julia Koricheva, Michael D. Jennions, Timothy H. Parker, Malgorzata Lagisz, Shinichi Nakagawa*. *Low statistical power and overestimated anthropogenic impacts, exacerbated by publication bias, dominate field studies in global change biolog*. BMC Biology, in revision 2022. [ecoevorxiv](https://ecoevorxiv.org/repository/view/3665/)

# How to use
This repository houses the code used to reproduce the models, Figures, and Tables in the paper of 'Publication bias impacts on effect size, statistical power, and magnitude  (Type M) and sign (Type S) errors in ecology and evolutionary biology'.

To run the analysis and plot the graphs provided in the paper, use: 
#### EcoEvo_PB_script.Rmd

The code has detailed annotations for our analysis pipelines. Using the datasets containing 88 independent meta-analytic cases (36 SMD, 20 lnRR, and 31 Zr cases, respectively), we used a two-step modelling procedure to assess (i) the estimated prevalence and severity of publication bias across the fields of ecology and evolutionary biology, and (ii) how such publication bias affects the estimates of effect size, statistical power, Type M and S errors. In the first step (i.e., within-meta-analysis level), multilevel meta-analytic approaches will be used to estimate the overall mean (used for power and errors calculations), and test and adjust for publication bias for each meta-analytic case. In the second step (i.e., between-meta-analysis level), the estimates from the first step were statistically aggregated using either mixed-effect models or random-effects meta-analytic models (i.e., secondary meta-analysis). 

### Deviations
we added a post-hoc analysis where we removed the meta-analyses with statistically non-significant mean effects and subsequently calculated the average statistical power, Type M and S error rates. The reason why adding this post-hoc analysis was that the underlying true effect sizes in some meta-analyses were likely to be so trivially small (and biologically significant) that corresponding power calculation was meaningless. In such a case, if we included those effects when estimating average power across meta-analyses in ecology and evolution, we would get downwardly biased average power estimate. Note that relevant results were reported at Supplementary Material.

# data folder contains:
20 lnRR datasets, 36 SMD datasets, 31 Zr dataset

# Figures folder contains:
Figures 1 - 6  reported in the main text; funnel plots and model residuals in the online supplementary materials
