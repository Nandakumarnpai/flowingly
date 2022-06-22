# flowingly
Software Development Challenge
Email Content Extractor
Configurable Fields
The below 3 fields are configurable in appsettings.json
1)	Total Tag
2)	Cost Center Tag
3)	Service Tax (Can be changed in future as well as according to different regions)
 
Steps For Running the Application
1)	Host/Run the Developed Web API in the IIS or Self Hosted Mode in Visual Studio

Once it up and running , it will show the default Page as below (Using Localhost as I used self hosted mode in Visual Studio)

 
2)	Open any Web API Development and Testing platform like POST Man or Fiddler

3)	Pass the Email Content As Body Parameter as below to the API

 

4)	You will get the sales tax and total excluding tax based on the extracted <total>  as shown below.
Note :- Sales tax is calculated as per 10% of Total as configured in appsettings.json can also be changed
 
 Missing <cost_centre> In this case value of the ‘cost centre’ field in the output is shown as ‘UNKNOWN’. 

 

5)	If the CostCenter is there it will also displayed in the Result as below, Body given as per the Exercise PDF

 

6)	If any Irregularities/Missing XML’s or Error in the XML it will Return Empty results, as below. In case of Exception it will handled appropriately and will be logged 
 



