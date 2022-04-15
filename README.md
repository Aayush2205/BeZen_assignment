# BeZen_assignment
## PIP install -

  As I was using Jupyter Notebook from Ananconda so the basic packages were already installed .
  Generally-
  **pandas**-pip install pandas
  **numpy**- pip install numpy
  **matplotlib**-pip install matplotlib
  If you are using VS Code then the insallation command is little different
  **pandas**-python -m pip install pandas
  
  
## How to run the code-

  I've written the code in Jupyter Notebook and the file that I've uploaded is in .ipynb format so it will easily open in any of the coding platform that supports    python.
  
### First Question- Products without prices
  
  I've approached this question in an easy way by just checking the price_string for NaN value using isnull() which is function of pandas and then printing the uuid for the product.
  
### Second Question-  Count of products without prices and with prices in each Product Type, Category, Level 1 

  For this question, first of all I've assigned two variables- one for products without price and another one for product with price , and now to put both the variables into the different groups, groupby (another function of pandas) is used as it will group the data in the mentioned column, and the we can count the number of products using the count() function. Mapping is done to show the count of each uuid of products.
  
 ### Third Question- Correct Product Prices in the correct format (eg: $56) wherever possible and separate them into currency and value columns. 
  
  First of all we have defined a function which will work to remove the currency symbol and convert the price_string value to float. After that we will directly convert back the float value to currency and due to this we got the corrected format of currency(eg- $58) in every row . Now we'll use the part where we converted the string to float to create a new column which will only hold the values of the price and then as we know that the currency is only '$' so we'll directly add one more column for the currency and then we'll delete the price_string .
    
### Fourth Question - List out the categories with average price of product. 

  Having the new values column in the dataset would help in the fourth question as we need the average ,so for this we would use the groupby option so to group the result with categories and then we'll use the mean() function to calculate the average. By using a Graph we could show the mean of everyg category that is present.
