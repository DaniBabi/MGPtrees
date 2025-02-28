Click the sections to open the details.

<details>
 
<summary><h2>Fields in treedata.geojson:</h2></summary>  <br>

 ### The following attributes are set in the data structure:<br>
 
"Tree_ID":1,&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;#int  <br>
"Diameter1":12,&emsp;&emsp; &emsp;&emsp;#int    <br>
"Diameter2":null,&emsp;&emsp;&emsp;&emsp;#int  <br>
"MorF":"M",&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;#string  <br>
"Two_Stem":null,&emsp;&emsp;&emsp;&emsp;#boolean  <br>
"Health_Status":null,&emsp;&emsp;&emsp;#string  <br>
"Symptom":null,&emsp;&emsp;&emsp;&emsp;#string  <br>
"Last_Treated":null,&emsp;&emsp;&emsp;#date  <br>
"Note":null,&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;#string  <br>
"Species":"White Ash",&emsp;&emsp;#string  <br>
"Age":null,&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;#int  <br>
"Sponsored":null,&emsp;&emsp;&emsp;&emsp;#boolean<br>
"Sponsor_Name":null,&emsp;&emsp;&emsp;#string<br>
"Sponsor_Date":null,&emsp;&emsp;&emsp;&emsp;#date<br>
"Tree_Nickname":null,&emsp;&emsp;&emsp;#string<br>
"Link":"https://",&emsp;&emsp;&emsp;&emsp;&emsp;#string<br>
"Payment_ID":null,&emsp;&emsp;&emsp;&emsp;#string<br>
"Longitude":-77.82096667,&emsp;#float<br>
"Latitude":39.4211,&emsp;&emsp;&emsp;&emsp;#float<br>
"Individuals":1&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;#int<br>
</details>
<details>
 
<summary><h2>How to edit treedata.geojson:</h2></summary>

### How to Edit treedata.geojson

1. In Github, click on treedata.geojson to go to the file.
2. Above the code, where it says Preview, Blame, Code, click Code to view the dataset.
3. On the right hand side of the interface, click on the pencil to edit the dataset. <br>
<img width="500" alt="image" src="https://github.com/user-attachments/assets/068142d3-04cb-4332-8672-a6b6ba3169b8" /> <br>
4. On the right hand side of the interface, click the No Wrap dropdown to change the line wrap mode to Soft Wrap.
5. The interface will orient the data so that the first two lines appear like:
 
 ```
{"type":"FeatureCollection","features":[{"type":"Feature","properties":  
{"Tree_ID":1,".....
```
  * This helps view the records in a more organized way.

6. Find the tree_ID that needs to be changed from "Sponsored": null to "Sponsored": True.
7. Click commit changes to end the editing session. Add a description about the edit if you'd like. 
<img width="528" alt="image" src="https://github.com/user-attachments/assets/9093dc84-e764-43e3-9d28-f9208f340fa0" />



### What you can and can't update:
* Do not change the attribute names, which appear as above enclosed in double quotes, followed by a colon (:) unless you change them all across the records.
* Numeric fields are integers aka whole numbers and are entered, for example, as ```"Tree_ID":1.```
* Lat and Long are floats aka numbers containing decimals and unless the trees are sprouting legs and moving, should remain the same.
* String aka text fields must be enclosed in double quotes: ```"Sponsor_Name":"Jacko Lantern"```
* ****Sponsored**** and ****Two_Stem**** are boolean data types, so True or False do not get any single or double quotes, therefore,
  * ```"Sponsored":null``` until somone pays the fee, and then change null to True. ```"Sponsored":True```
  * When the sponsorship period expires, change True to False
  * ****DO NOT CHANGE**** anything after the number of individuals.
  * ****DO NOT DELETE**** any commas, brackets, or parentheses. 
</details>

<details>
 
<summary><h2>What's what</h2></summary>

### mapfile contains the code to embed on the google site.
* To use, simply click on mapfile to open it, then copy and paste into a code window on your google site.
* When a user submits a payment<sup>*</sup>, that information is not connected to the form or the tree app.
* When a user completes and submits the form, an email is sent to the administrator with the data to update treedata.geojson and sponsors.csv.
treedata.geojson is the data form containing the geometry and attributes of each ash tree.
sponsors.csv is a delimited text file that contains sponsor data for future individuals. The single record is here as an example. sponsors.csv is linked to the google form.

### On the website,

https://sites.google.com/view/adopt-an-ash-tree/home

* The Shopfy Element html page contains the widget for the payment process **and is broken**<sup>*</sup>	. This needs to be fixed to enable people to adopt via the web. <h4> *This snippet of code was **provided to the developer by the organization and is not affiliated with the developer**.</h4>
* The Shopify Element code is pasted into a small embed window above the google form on the adoption page.  
  <img width="377" alt="image" src="https://github.com/user-attachments/assets/5a0fd313-3b00-4385-ae91-dc3a21d1a5a5" />  <br>
* The google form is added from drive into the google page beneath the shopify element.  
  <img width="196" alt="image" src="https://github.com/user-attachments/assets/56379f39-3a1f-4a57-8bcd-a332375f3dae" />  <br>

### Behind the scenes

* The google form is stored in google drive with sponsors.csv
* sponsors.csv is updated when a form is submitted.
* The form contains required entries to ensure all fields are updated in sponsors.csv.
</details>
