# Liquid Crystal Analysis
This is pipeline to analyse Opto-Electric Switching Data of Liquid Crystals.
This code was written to perform **quick analysis** of Liquid Crystal Opto-Electric Response Times and plot graphs of the same using **commonly available open-source tools and libraries.**
Apart from the **higher quality graphs** generated, the Data Processing and plotting time and for each file reduces from 5 min to less than a second.
___

## Setup
1. Clone the repository using: ```git clone https://github.com/avi1299/Liquid_Crystal_Analysis.git```
2. Enter the directory Liquid_Crystal_Analysis using: ```cd Liquid_Crystal_Analysis ```
3. Install the necessary python packages to run the notebook: ```python3 -m pip install -r requirements.txt```
4. Start the Jupyter Server in the given directory: ```jupyter notebook```
5. Copy the link for the notebook into your browser

![Link for Notebook](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/Token.png)

6. You can now access the Notebook

![StartPage](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/Jupyter_main.png)

___

## Analysis
1. Start the **Analyser.ipynb** notebook
2. Change the value of the **path** variable in the noteboook to the directory where the datafiles are kept. Fill in other details such as **name_of_LC** and **temp**

![Path](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/Setting_path.png)

3. On running the cells, you will be asked for input voltage. Give the input. The code will seach for the file of format ```<temp>_<voltage>_2.csv``` and will let you know if it finds it

![Enter Voltage](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/EnterV.png)

![Entered Voltage](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/EnteredV.png)


4. On finding the file, run the next cell to analyse the file. Output graph created in **path/Analysis** directory( will be created if it doesnt exist)

![Analysis](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/Analysis_graph.png)

5. If you are satisfied with the graph and output response times, run the next cell to add the response times to a table which will be used to record **ResponseTimes vs Applied Voltages**

![Adding Results](https://github.com/avi1299/Liquid_Crystal_Analysis/blob/master/Documentation/Images/Adding_Results.png)

6. Repeat steps 3-5 for the different voltages for which the file exists.
7. After analysing all the files you can run the next cell to plot the **ResponseTimes vs Applied Voltages** graph.
8. Run the last cell to push the results into a csv file in the output directory
