# Predicting Crystal Sturctures
By using several methods of analysis and modeling to find the factors that affect the shape of a Perovskite crystal structure

Author: Ashley Grant-Hewitt

Business problem: Predict the crystal structure for a Perovskite compound based on several characteristics (to find the the ideal/most stable form)

Data: Data was sourced from https://www.kaggle.com/datasets/sayansh001/crystal-structure-classification?select=Crystal_structure.csv

Methods: The data was explored via inspection, cleaning, and visualization. Duplicates were removed, data discrepencies were fixed, and missing data was dropped as well as other columns that did not pertain to solving the buisness problem.

Results: Scatter/ Correlation Graphs

<img width="385" alt="Screen Shot 2022-05-25 at 10 24 03 PM" src="https://user-images.githubusercontent.com/96153312/170402794-c25ef94e-047c-4f3d-998f-bf2ff3fffd05.png">


In the graph above, we see that the x-axis is the octahedral factor and the y-axis is the ionic radius of the A cation and they are completely postively correlated. The octahedral factor is a parameter for predicting structure stability. When μ > 0.41, the structure is stable. So we see that all radii above 0.6 are most likely to have stable crystal structures.

Scatter/ Correlation Graphs

<img width="387" alt="Screen Shot 2022-05-25 at 10 24 18 PM" src="https://user-images.githubusercontent.com/96153312/170402835-1ae9564b-e7ab-4722-abf1-2de5e237b31e.png">


In the graph above, we see that the x-axis is the ionic radius of A cation and the y-axis is the ionic rdaius of the B cation and they are strongly positively correlated. From the previous graph we saw that all radii above 0.6 are most likely to have stablely structures. Thus, we can infer that the A cations above 0.6 that correlate with the B cations will also have stable crystal structures

Recommendations: We clearly see that structures with high octehedral factors (>0.41) and large ionic radii (>0.6) are considered more stable. Thus, the structures these compounds hold would most likely be considered the ideal Perovskite crystal structure. However, we must first create the model to predict the various compounds structure. Therefore, I created two different models on this data set. (k neareast neighbors, random forest classifier)

I recommend the random forest model because the accuracy value for the testing data is higher than the accuracy value provided by k nearest neighbors. However, both models are overfit, achieving 100% accuracy on the training data.  

Limitations & Next Steps: The best model was only able to predict the structures with about 78% accuracy. Ideally a model 80% or higher would be considered the "best". The next step would be to create another type of model that could make better predictions without creating an overfit model. With that information we could better predict the structures which would allow us to conduct deeper analysis to determine which structure is ideal. 

For further information For any additional questions, please contact me

