## **Abstract**
The financial landscape is ever changing, and today's fast-paced environment has shown that traditional safeguards against fraud are no longer suffice, with approximately 16\% of Dutch residents falling victim in 2020, amounting to a loss of approximately 2.75 billion euros \cite{Statistics_Netherlands_2022}. To combat this, many banks employ sophisticated machine learning (ML) models to assist in detecting fraud against their customers. These models come at the cost of transparency and explainability, and with responsible data practices becoming more the industry standard (and in many cases a legal requirement) novel solutions need to be employed to ensure resilient and explainable ML models within fraud detection. 

This thesis investigates the application of a modified Knowledge-Enhanced (KE) Graphical Neural Networks (GNN) within the fraud detection space. Knowledge-Enhanced Graphical Neural Networks (KeGNN) integrate domain-specific knowledge (or clauses) within the neural network, allowing for more interpretable and robust fraud detection models. This study evaluates the application of KeGNNs on heterogeneous graphs and evaluates the performance on Graphical Attention Networks (GAT), and Graphical Convolutional Networks (GCN) models. This study finds limited support for the application of KeGNN models within the main experiment. In a subsequent analysis designed to enhance clause value within the KeGNN models, the KeGAT model demonstrates superior performance compared to the main experiment. The observed performance gap between the KeGNN models and their GNN counterparts also widens. There is also sufficient support for all the GNN models outperforming the baseline (XGBoost).



This experiment has been setup to work within the Google Colab environment.
To run this experiment you must follow these instructions:
1. Run "download_process_data.ipynb" - this will download and process the IBM fraud detection data set
2. Run "\KE_GNN\Graph Creation\Main_experiment_graph_creation.ipynb" - This program will create the graph structures and knowledge enhancement clauses needed for the main experiment
3. Select which model and run within "\KE_GNN\Main Experiment\ *.ipynb" - within this folder are all the respective models
4. All results can be processed within the "\KE_GNN\results.ipynb" program
5. To run the post-hoc experiment you must run the programs within "\KE_GNN\Post Hoc\*.ipynb"
