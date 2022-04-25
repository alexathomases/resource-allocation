# resource-allocation
Formulating the distribution of COVID-19 resources as the MWVC problem of graph theory.

Here I formulate the spread of an epidemic as a graph theory problem using a contact network with nodes weighted by the COVID-19 infection rate by age and race demographics reflective of the United States population. I contrast two algorithms for approximating the minimum weight vertex cover (MWVC) of the network: the built-in NetworkX approximation and a non-deterministic heuristic known as Master-Apprentice Evolutionary Hybrid Tabu Search (MAE-HTS). Further, I explore the effect of removing various subsets of the vertex covers from the network on the population infection rate. The SIS epidemic model is used to simulate an epidemic with no immunity upon recovery. I demonstrate that removing from the network those nodes in the MAE-HTS vertex cover with highest closeness centrality resulted in the largest decrease in population infection rate when the virus transmission rate is medium or high. These results provide promising evidence of the efficacy of epidemic intervention by means of resource distribution that takes into account the entire network structure.

To explore the effect of various resource distribution strategies on a real-life contact network, upload the .xlsx file into the Google Colab runtime and execute the cells in order.

# References 
Wang, Y., Lu, Z., Punnen, A.P. (2021). A Fast and Robust Heuristic Algorithm for the Minimum Weight Vertex Cover Problem. IEEE Access 9, pp. 31932-31945. 

Villegas, M., Gonzales-Agirre, A., Gutierres-Fandino, A. (2021). Predicting the Evolution of COVID-19 Mortality Risk: a Recurrent Neural Network Approach. medRXiv doi: https://doi.org/10.1101/2020.12.22.20244061. 

United States Census Bureau (2022). Quick Facts: United States. https://www.census.gov/quickfacts/fact/table/US/PST045221. 

Centers for Disease Control and Prevention (2022). Risk for COVID-19 Infection, Hospitalization, and Death By Race/Ethnicity. https://www.cdc.gov/coronavirus/2019-ncov/covid-data/investigations-discovery/hospitalization-death-by-race-ethnicity.html 

B. Wang, Y. Sun, T. Q. Duong, L. D. Nguyen and L. Hanzo, "Risk-Aware Identification of Highly Suspected COVID-19 Cases in Social IoT: A Joint Graph Theory and Reinforcement Learning Approach," IEEE Access, vol. 8, pp. 115655-115661, 2020, doi: 10.1109/ACCESS.2020.3003750.

E. Meirom, H. Maron, S. Mannor and G. Chechik, "Controlling graph dynamics with reinforcement learning and graph neural networks", Proc. Int. Conf. Mach. Learn., pp. 7565-7577, 2021.

Yoshua Bengio, Prateek Gupta, Tegan Maharaj, Nasim Rahaman, Martin Weiss, Tristan Deleu, Andrew Williams, “Predicting Infectiousness for Proactive Contact Tracing, ICLR, 2021.

Supady, A., Curtis, J.R., Abrams, D. (January 2021). Allocating scarce intensive care resources during the COVID-19 pandemic: practical challenges to theoretical frameworks. Lancet Respiratory, vol. 9, pp. 430-434, doi: https://doi.org/10.1016/S2213-2600(20)30580-4. 

Emanuel, E. J., Persad, G., Upshur, R. (2020). Fair Allocation of Scarce Medical Resources in the Time of Covid-19. N Engl J Med 2020; 382:2049-2055, doi: 10.1056/NEJMsb2005114. 

Baunez C, Degoulet M, Luchini S, Pintus PA, Teschl M (2021) Tracking the dynamics and allocating tests for COVID-19 in real-time: An acceleration index with an application to French age groups and départements. PLoS ONE 16(6), doi:10.1371/journal.pone.0252443. 

Degoulet, Mickael and Luchini, Stephane and Pintus, Patrick and Teschl, Miriam, Sub-National Allocation of COVID-19 Tests: An Efficiency Criterion with an Application to Italian Regions (April 15, 2020). http://dx.doi.org/10.2139/ssrn.3576161. 

Yin, X. (March 2021). COVID-19: Optimal Allocation of Ventilator Supply under Uncertainty and Risk. medRXiv, doi: https://doi.org/10.1101/2021.03.09.21253216. 


