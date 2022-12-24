# SAChocolateImports
Load dataset
Chocolate Imports into South Africa: 2010 - 2017
I got this dataset from 'Open Up' which stores interesting datasets from South Africa
Reference: https://data.openup.org.za/dataset/chocolate-imports-into-south-africa-2010-2017-qccd-zgyb

Why this project? We want to first get an idea of all the world regions where imports come from as well as the count for these regions. The goal is to find the districts with the highest imports and highest customs of chocolate into South Africa using Python data analytics tools such as numpy, pandas, seaborn and matplotlib.

Cleaning data
Lets identify presence of missing and/or null values within the data set

We want to avoid losing data found in the other columns that do not have null values therefore we will use the most frequent value found in the column, and impute that value to the missing values
most frequent value is BE

Visualise data
An easy way of doing this is to use a bar chart/bar graph to visualise the world regions and the count or frequency at which they appear in the dataset. This is important because it enables us to clearly view which world region provides South Africa with the most chocolate.


We notice a direct proportionality between the quantity and the customs value meaning that the different imports (represented by dots in the above visualisation) were importing the same/similar quality chocolates (implying that chocolate prices were similar) which means that when the quantity is increased, it increases in proportion with the value, which is what we see in the visualisation above. If this were not the case and certain imports had much more expensive chocolates (higher quality) then we would expect to see points with higher customs value even at lower quantities (these points would lean towards the bottom right side of the graph/visualisation). The opposite would also be true, lower quality (cheaper) chocolate imports would appear towards the top left side of the graph. But we do not see that, therefore meaning that the quality of chocolate imports from Belgium, which accounts for majority of imports from Europe to South Africa, were for the most part similar throughtout the 2010 - 2017 period

Reference: Aric A. Hagberg, Daniel A. Schult and Pieter J. Swart, “Exploring network structure, dynamics, and function using NetworkX”, in Proceedings of the 7th Python in Science Conference (SciPy2008), Gäel Varoquaux, Travis Vaught, and Jarrod Millman (Eds), (Pasadena, CA USA), pp. 11–15, Aug 2008
website: https://networkx.org/documentation/latest/
#Lets create a network graph

We readily notice that out of the world regions soecified, Africa is the only one that has 'Road' as one of its forms of transport for imports. This makes sense because South Africa is in Africa and road transport makes the most financial sense for imports. Europe for example only used air or maritime, this is most likely due to the large distance between South Africa and Europe. The same is true for America and Asia whereas Oceania only uses air.
Lastly we can compare three of our columns with each other to see how they varied throughout the entire period (2010-2017), to do this we will use Matplotlib 3D visualisation
