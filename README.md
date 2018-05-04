# BB-K-12_API<br/><br/>
Using the Blackbaud K-12 "ON" API lists to create data displays<br/><br/>
This is based heavily on what I gleaned from Shandor Simon's session at the 2016 BB K-12 conference: Student Information Management: Leveraging Open Application Programming Interface (API) in "ON" Products.<br/><br/>
Most of this can be found at: http://on-api.developer.blackbaud.com/<br/><br/>
Step 1: Sign up with BB K-12 to install the SDK. Create a new user in the Core database with the Role of Web Servies API Manager to allow that user access to the API results.<br/><br/>
Step 2: Create your list in the ON > Lists > Manage Lists > Advanced Lists area. For example, create a list of only Upper School Athletics games with dismissal times. To obtain the list ID for use in the API call, mouse over the Edit button - it will be the slid #. Edit list access to allow the Web Services API Manager to access.<br/><br/>
You will need to access a live server, or install a local server environment. From this point on, you can use the uploaded php file for reference.  The website, username and password are not included, so the file would be useless without these.<br/><br/>
Step 3: Use JSON format to access the results. First run a simple data dump, to test you are getting something. <br/><br/>
Step 4: Run the program again to get key value pairs to define variable names for later use. The results go into data.json.<br/><br/>
Step 5: Use the results from Step 4 and create a foreach loop to display the results from your list. Style according to the website this is displayed on.<br/><br/>
Step 6: Upload the file to a secure (https://) website to embed in your ONMessage public page.<br/><br/>
Step 7: Use the embed widget to include an iframe src= to the url in Step 6.<br/><br/>
