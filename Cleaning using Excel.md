The rows and columns were obtained from the original dataset using the text to columns feauture. The delimiter was tab.
<br>
The column Dt_Customer was formatted to DD-MM-YYYY date format.
<br>
Similarly, all the columns with numeric values were set to the number format and all the columns with characters were changed to the text format.
<br>
The case of all the headers was changed to lower case using =LOWER()
<br>
I deleted blank rows and rows which had cells with null entries. 
<br>
1 complete blank row, 24 null entries in income, and 1 null entry in dt_customer were found which were all then removed.
<br>
Remove duplicates feature was used to remove any existing duplicates. None were found.
<br>
The marital_status column had some strange entries like 'Alone','YOLO', and 'Absurd'. These were all updated to 'Single'. The find and replace feature was used.
<br>
Purpose of the response variable - 1 if customer accepted the offer in the last campaign, 0 otherwise.
<br>
While looking at the 2 YOLO entries, it was noticed that both the rows were COMPLETELY same except for the id and the response. 
<br>
From the observation it looked like 2 entries for the same customer. One of them had 1 for response and the other had 0. 
<br>
The greater id number had 1 as response meaning the customer accepted the offer in the last campaign. So, the row with 0 response and the smaller id was most likely an old record of the same customer, which was not needed. Hence, the row was deleted. 
<br>
The person in charge had simply forgotten to delete the old record and had registered the customer again.

