# Search

**Search** is used to find Objects that are used throughout the model. Search is paticularily helpful in models with many Diagrams or when searching for specific Tasks, Events, or Gateways.

Select **Search** from the  **Home** pull-down menu to open the **Search** dialog.

![Open Search Panel](images/searchopen.png)

Select an Object on your open Diagram. **Search** automatically searches for all Objects in the currently opened process model that contain the same **Name**. If no **Object** is selected, select a desired Search term from the available Object Names shown of all of the Search terms in the opened model. Enter the desired Search term into the Search dialog box. **Search** will show all Objects that contain the selected Name.
![Search Panel UI](images/searchpanel.png)

## Using Search

Objects matching the Search term will be shown in a Table that consists of:
* Object Name, 
* Diagram Name and 
* Additional Attribute data depending on the Object type selected. 

1. Click on the column header to sort and filter content.
2. Click on the row of the Search terms shown to navigate to the associated Diagram. The selected Object will be highlighted with a blue frame. Users can then easily navigate through the found objects and/ or jump to the place in the Process where the object is used.
3. Use the **All** pull-down menu in the top left of the **Search** window to filter Objects by Object type.  This  shows all Object classes in the model. If an Object type is selected, only those objects belonging to that Class will be shown. e.g. Tasks or Events.
![Search: Switch Class](images/searchselecttype.png)
4. Search for a specific word by entering the word into the Search dialog box.
5. **Start** and **Stop** can trigger a new search or stop the current Search process.
6. **Excel** option exports a list of found Objects to an Excel file.
7. **Save** writes found Objects items to a JSON file.
8. If you want to Edit the Name of one of the found Objects in your model, double-click on the row of the Object where it is shown in Serch to open the Diagram where it is used. 

If the Object Name was created using the Vocabulary naming option, change the name by selecting the Vocabulary icon shown to the right of the Object Name and select the desired Object Name and Method or create new Names as needed. If the Name was not created using the Vocabulary option, simply change the Name and click on the Save icon.
