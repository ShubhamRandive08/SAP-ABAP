Steps Of Project



Step No. 01: Table and TMG creation



Create the tables which are ZEMP\_MASTER\_MY and ZEMP\_LEAVE\_MY with the respective fields.



**MASTER TABLE NAME	ZEMP\_MASTER\_MY**

**LEAVE TABLE NAME	ZEMP\_LEAVE\_MY**





Then create the TMG to maintain table records.



TMG FOR MASTER TABLE	ZEMP\_MASTER\_MY

TMG FOR LEAVE TABLE	ZEMP\_LEAVE\_MY





Step No. 02: Module Pool creation

We have two methods for the creation of the module pool 

Using the **SE80**

Using the **SE38** (Using)



We are using here with SE38 - Create the program as '**ZLEAVE\_APP\_MY**'

&#x09;	- Give the title and select the type as Module Pool



&#x09;(Program Name: **ZLEAVE\_APP\_MY**)

&#x09;Create DATA 

&#x09;DATA: gv\_emp\_id type zemp\_id,

&#x20;     	      gv\_from\_date type sy-datum,

&#x20;     	      gv\_to\_date type sy-datum,

&#x20;     	      gv\_reason type char100,

&#x20;             ok\_code type sy-ucomm.



&#x09;Then open your program (**ZLEAVE\_APP\_MY)** in **SE80**



&#x09;	**Steps:** 

&#x09;		Then right click on your **program name** --> click on **create** --> click on the **screen** --> Provide the screen number as '**100'** --> Then provide the Short Description --> 			Next Dynpro is **'0'** --> **Save** --> **Activate** --> **Layout** 



&#x09;		Then it will automatically open the **Layout** screen - Provide the **text and its header (Empleyee ID, From Date, To Date, Reasone**  --> Then create the **input field** --> 			Then create the **button(SAVE, BACK, CLEAR) -->** Then bind the data to the input fields ( gv\_emp\_id, gv\_from\_date, gv\_to\_date, gv\_reason) \[Double click on the **input 			field** and provide this **variable** name as the **name** of the **input field**] --> Then provide the name and the function code to the buttons (**Button name:** Pushbutton1,2,3, 			**Text:** SAVE, CLEAR, BACK, **Function Code:** SAVE, CLEAR, BACK) --> **SAVE** --> **ACTIVATE**





















