# TrafficExperimentCode

Highway traffic dynamics are extremely complicated, due to the erratic behaviour of human drivers. Overreacting to avoid collisions, often by suddenly decelerating, causes waves of cars behind a driver to also slow down or stop, resulting in an emergent jam. This results in many cars on the road travelling at a speed much lower than the theoretical maximum average speed of the road, and these delays create a significant cost to the economy. Inefficient driving behaviours have led to the increased interest in Autonomous Vehicles (AVs). There has also been a large amount of research on applying Machine Learning, and specifically Reinforcement Learning (RL), by using large amounts of data collected from the road, to ensure that individual AVs remain collision-free and more fuel efficient, and to maximize flow on roads that exclusively contain AVs. However, very little research has been done on mixed autonomy roads, especially in terms of improving traffic flow with AVs that are coordinated, but trained using their local observations of the road. 

The thesis associated with these experiments focused on assessing the impact of AVs on improving traffic flow in mixed autonomy collision-free highways. Roads were simulated using micro-traffic models, with adjustments designed to simulate a future world in which Automatic Braking Systems will be good enough to completely prevent rear-end and lane-change collisions on highways. Deep Neural Networks were combined with Reinforcement Learning (together known as Deep Q Networks) to model the AVs, and this approach was tested on single and double lane highways.

This repository holds the code to conduct these mixed-autonomy collision-free experiments. This includes the following:
+ Framework to represent single, double and $n$-lane roads.
+ Code to simulate human drivers, developed with reference to Nagel-Schreckenberg traffic models.
+ Code to manage the entry and exit of cars.
+ Tabular, Linear-Regression, XGBoost, Deep Neural Network based Reinforcement Learning Code for Coodinating Autonomous Vehicles.
+ Functions used to plot results, some example experiments.

These are all stored in an R-Markdown notebook, (request aditya.yow@gmail.com for the associated R scripts). Some key results obtained using the above are as follows:
+ In single-lane roads, the average speed of all cars on the road was increased by 10\% to 23\% and the percentage of stopped cars on average per iteration was decreased by 14\% to 65\%, after 5\% to 50\% of the vehicles were converted to AVs. 
+ In double-lane roads with no entries or exits, the average speed was increased by 5\% to 26\%, and the percentage of stopped cars was decreased by 25\% to 69\%, after 5\% to 50\% of the road was converted to AVs.
+ In double-lane road containing entries and exits, the average speed was increased by 24\% to 44\%, and the percentage of stopped cars was decreased by 20\% to 68\%, after 5\% to 50\% of the road was converted to AVs. 
