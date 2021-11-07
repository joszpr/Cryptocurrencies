# Cryptocurrencies


### **Overview** ###
Report prepared for Accountability Accounting with an analysis on Cryptocurrencies on the trading market. The purpose of the study is to look at current cryptocurrencies that would be viable to add to their portfolio for their customers to be able to invest. The goal of the analysis is to develop a classification system of the cryptocurrencies to help guide the investing strategies of their customers. 


### **Methodology** ###
The data for the study contains information for the current available cryptocurrencies; name, type of algorithm, whether its currently trading, Proof Type (type of security), Total Coins mined and the total supply. 

![data_overview](https://user-images.githubusercontent.com/85839235/140634775-4f53f8dd-a908-4b88-9993-effd3d868723.png)

The classification of the coins will be achieved with Unsupervised Machine Learning. 

**Data Process** 
  - Cleaning
    - The data was cleaned and filtered to only keep coins that were currently Trading, have all values for the analysis and had a working algorithm, among other data cleaning. 
  - The data was then parsed into numerical values and scaled in order to prepare it to be processed under a Machine Learning algorithm. 
  - The dimensions of the data were reduced to 3 Principal Components in order to increase the utility and efficacy of the model. 
  - The Elbow Curve was calculated based on the 3 Principal Components in order to find the best values to for K-Means.
  - Best value for K-Means was 4. This value helped in identifying the number of clusters that would best represent the data. 
  - A model was trained with the current available data of cryptocurrencies. 
  - A 3D interactive figure was plotted using the results of the model and how the algorithm best divided the data into classes. 
  - The 4 classes were plotted in a 2D Graph that would help in compare the number of coins that have been mined and their supply.


### **Conclusions** ###

  - The suggested classes for grouping of the Cryptocurrencies were 4 according to the behavior of the data as showcased by the Elbow Curve. But looking closer at the 3D figure and the 2D Graph, it is clear that there is a class with just 1 value. The Principal Components categorized the cryptocurrency BitTorrent as unique enough to fit in a separate cluster. Presenting 4 classes of cryptocurrency investments for clients, and one of those classes only having 1 options may not efficient. A closer, manual inspection is recommended on BitTorrent in order to decide if it is an investment option that can be eliminated from the offering portfolio or if it can be added to one of the other groups. 
![3d_figure](https://user-images.githubusercontent.com/85839235/140637091-457e72f8-6314-4231-a8e6-f0466c16ab77.png)

  - A list of offerings can be prepared once the decision regarding Class 2, which contains only BitTorrent has been decided. The groups characteristics can further be visualized with a 2D graph. 
![2d_plot](https://user-images.githubusercontent.com/85839235/140637230-84ee7d01-9328-48cd-82e5-5d0ccf89efad.png)

  - Other visualizations can be done that showcase the differences cryptocurrencies.
    -   Amount of coins mined vs amount of coins available
    -   Current price value and historic changes
    -   Daily and historic volume traded

