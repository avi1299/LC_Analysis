# Liquid Crystal Analysis
Creating a pipeline to analyse Opto-Electric Switching Data of Liquid Crystals
___

## Setup
1. Clone the repository using: ```git clone https://github.com/avi1299/Liquid_Crystal_Analysis.git```
2. Enter the directory Liquid_Crystal_Analysis using: ```cd Liquid_Crystal_Analysis ```
3. Install the necessary python packages to run the notebook: ```python3 -m pip install -r requirements.txt```
4. Start the Jupyter Server in the given directory: ```jupyter notebook```
5. Copy the link for the notebook into your browser
7. You can now access the Notebook
___

## Analysis
1. Start the Analyser.ipynb notebook
2. Change the value of the **path** variable in the noteboook to the directory where the datafiles are kept. Fill in other details such as **name_of_LC** and **temp**
3. On running the cells, you will be asked for input voltage. Give the input. The code will seach for the file of format ```<temp>_<voltage>_2.csv``` and will let you know if it finds it
4. On finding the file, run the next cell to analyse the file. Output graph created in **path/Analysis** directory( will be created if it doesnt exist)
5. If you are satisfied with the graph and output response times, run the next cell to add the response times to a table which will be used to record **ResponseTimes vs Applied Voltages**
6. Repeat steps 3-5 for the different voltages for which the file exists.
7. After analysing all the files you can run the next cell to plot the **ResponseTimes vs Applied Voltages** graph.
8. Run the last cell to push the reults into a csv format in the output directory
