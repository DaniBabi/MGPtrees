## ****Fields in Treedata.geojson:****
  * "Tree_ID":1,                   &emsp;&emsp;&emsp;&emsp;  #int
  * "Diameter1":12,               &emsp;&emsp; &emsp;&emsp;  #int  
  * "Diameter2":null,              &emsp;&emsp;&emsp;&emsp;  #int
  * "MorF":"M",                    &emsp;&emsp;&emsp;&emsp;  #string
  * "Two_Stem":null,               &emsp;&emsp;&emsp;&emsp;  #boolean
  * "Health_Status":null,          &emsp;&emsp;&emsp;&emsp;  #string
  * "Symptom":null,                &emsp;&emsp;&emsp;&emsp;  #string
  * "Last_Treated":null,           &emsp;&emsp;&emsp;&emsp;   #date
  * "Note":null,                  &emsp;&emsp;&emsp;&emsp;   #string
  * "Species":"White Ash",         &emsp;&emsp;&emsp;&emsp;   #string
  * "Age":null,                    &emsp;&emsp;&emsp;&emsp;   #int
  * "Sponsored":null,             &emsp;&emsp;&emsp;&emsp;   #boolean
  * "Sponsor_Name":null,          &emsp;&emsp;&emsp;&emsp;   #string
  * "Sponsor_Date":null,          &emsp;&emsp;&emsp;&emsp;   #date
  * "Tree_Nickname":null,         &emsp;&emsp;&emsp;&emsp;   #string
  * "Link":"https://",            &emsp;&emsp;&emsp;&emsp;   #string
  * "Payment_ID":null,            &emsp;&emsp;&emsp;&emsp;   #string
  * "Longitude":-77.82096667,     &emsp;&emsp;&emsp;&emsp;   #float
  * "Latitude":39.4211,           &emsp;&emsp;&emsp;&emsp;   #float
  * "Individuals":1               &emsp;&emsp;&emsp;&emsp;   #int

## ****To edit treedata.geojson:****
1. In Github, click on treedata.geojson to go to the file.
2. Above the code, where it says Preview, Blame, Code, click Code to view the dataset.
3. On the right hand side of the interface, click on the pencil to edit the dataset.
4. On the right hand side of the interface, click the No Wrap dropdown to change the line wrap mode to Soft Wrap.
5. The interface will orient the data so that the first two lines appear like:
   {"type":"FeatureCollection","features":[{"type":"Feature","properties":
   {"Tree_ID":1,".....
7. This helps view the records in a more organized way.
8. Find the tree_ID that needs to be changed from "Sponsored": null to "Sponsored": True
9. What you can and can't update:
      * Do not change the attribute names, which appear as above enclosed in double quotes, followed by a colon (:) unless you change them all across the records.
      * Numeric fields are integers aka whole numbers and are entered, for example, as "Tree_ID":1.
      * Lat and Long are floats aka numbers containing decimals and unless the trees are sprouting legs and moving, should remain the same.
      * String aka text fields must be enclosed in double quotes: "Sponsor_Name":"Jacko Lantern"
      * ****Sponsored**** and ****Two_Stem**** are boolean data types, so True or False do not get any single or double quotes, therefore,
        * "Sponsored": null until somone pays the fee, and then "Sponsored":"True".
        * When the sponsorship period expires, change True to False.
      * ****DO NOT CHANGE**** anything after the number of individuals.
      * ****DO NOT DELETE**** any brackets or parentheses. 
      
