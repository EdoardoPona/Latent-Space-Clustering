# Latent-Space-Clustering

This is an experiment. The idea learn a mapping for data that facilitates clustering in a latent space. 
This is achieved by having a neural network that projects the data to the lataent space then picking k points that will
serve as cluster centers and optimizing everything (inluding the clusters' positions) to minimize a 'Cluster Loss' function 
(more details in the notebook). To make sure we don't losse the data's information, we will also train a neutwork to learn
an inverse mapping from the latent space to the original data. 

This still needs some work as the projected data doesn't always split upon theclusters even with the toy data we are using. 
Some aspects where further work should be done in my opinion are the following: 
- Is there some architecture or initialisation technique that could render this more stable?
- Finding a metric that represents how well the current clusters are working and wether a new cluster would help (basically 
finding the optimal number of clusters automatically)
