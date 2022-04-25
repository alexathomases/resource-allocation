# resource-allocation
Formulating the distribution of COVID-19 resources as the MWVC problem of graph theory.

Here I formulate the spread of an epidemic as a graph theory problem using a contact network with nodes weighted by the COVID-19 infection rate by age and race demographics reflective of the United States population. I contrast two algorithms for approximating the minimum weight vertex cover (MWVC) of the network: the built-in NetworkX approximation and a non-deterministic heuristic known as Master-Apprentice Evolutionary Hybrid Tabu Search (MAE-HTS). Further, I explore the effect of removing various subsets of the vertex covers from the network on the population infection rate. The SIS epidemic model is used to simulate an epidemic with no immunity upon recovery. I demonstrate that removing from the network those nodes in the MAE-HTS vertex cover with highest closeness centrality resulted in the largest decrease in population infection rate when the virus transmission rate is medium or high. These results provide promising evidence of the efficacy of epidemic intervention by means of resource distribution that takes into account the entire network structure.

To explore the effect of various resource distribution strategies on a real-life contact network, upload the .xlsx file into the Google Colab runtime and execute the cells in order.

