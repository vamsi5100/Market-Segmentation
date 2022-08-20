# Market-Segmentation
## Data Pre-processing:
### 1.	Categorical Variables:

•	We used three datasets for the EV market segmentation. The datasets consist of the quality, quantity of the vehicles, and geographical aspects of starting an EV business.
•	From the first dataset we selected a few variables like car Brand, Range, and Efficiency.
•	Introduced a new variable “Segment” in which we divided the price ranges into 7 categories based on the price of the vehicle.
•	Coming to the geographical aspects we only considered variables like the name of the state, location of the charging stations, and type of power supply.

 

### 2.	Numeric Variables:

•	Converted the categorical variables into numeric variables for the dataset that consists of the quality and quantity of EV vehicles to check for correlation.
•	We used variables like 2-wheeler, 3-wheeler, and 4-wheeler vehicles for the estimation of vehicle types and considered the total number of vehicles used per state.
 
### Principal Component Analysis:
•	We have used the numeric data of vehicle type data for performing “Principal Component Analysis”.
•	Extracted new variables using PCA in which we observed that the first two variables comprise of 90% of the variance of the data.
•	PCA helps to use less data when we have a very large amount of data which in return helps in reducing a lot of computation.
 

## Extracting Segments:
•	After successfully completing the Data pre-processing part we explored the data through visualization using python libraries like matplotlib and seaborn.
•	For categorical variables we used bar plots and histograms to check the quantity and quality of the respective variable.
•	After when the categorical data is converted into numeric data we used the seaborn library to plot the correlation matrix to eliminate the unwanted variables.

### 1.	Extracting Segments by exploring data:

 
•	From the above heatmap we can understand that almost 50% of the variables are highly correlated so we can take a maximum of 3-5 variables as our segmentation variables. In this case, we took “Brand, Range, Efficiency, Segment, and Seats”.

  
•	In the above bar plot we can understand that segment C has the highest demand when compared to other segments followed by segments B and D; so we can focus more on segments B, C, and D out of which most of the car brands that are purchased are Tesla, Volkswagen, BMW, Polestar and Honda.
•	When the above-extracted segments are considered most of the cars that have been purchased are 2 and 3-seater as they were more economical.

 
•	When it comes to places where most of the EVs are being used are Uttar Pradesh, Maharashtra, Tamil Nadu, Karnataka, Gujarat, and Rajasthan; so, it would be better if we consider the above places first while starting a business.

### 2.	Extracting Segments using K-means clustering:

•	K-means clustering is an unsupervised machine learning technique used to extract unidentified patterns in the data.
•	This algorithm is iterative; it improves the partition in each step, and is bound to converge, but not necessarily to the global optimum. 
•	The key idea is to systematically repeat the extraction process for different numbers of clusters (or market segments), and then select the number of segments that leads to either the most stable overall segmentation solution, or to the most stable individual segment.
•	For clustering the segments we used Range and Efficiency variables and normalized the data in order to plot against other variables.

 
 

•	To get an idea of the number of clusters we need to perform we can use the elbow method.
 
