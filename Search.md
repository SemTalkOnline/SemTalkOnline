# Search

**Search** is used to find Objects that are used throughout the entire model. This is paticularily helpful in models with many Diagrams or when searching for specific Tasks, Events, or Gateways.

In the main **Home** pull-down menu, select **Search** to open the **Search** dialog.

![Open Search Panel](images/searchopen.png)

**Search** automatically triggers a search for all Objects in the currently opened process model that contain the same Object name shown in the selected Object. If no object is selected, Search will show all Objects that have the given Search term.
![Search Panel UI](images/searchpanel.png)

## Using Search

Objects matching the Search terms will be shown in a Table, which consists of:
* Object name, 
* Diagram name and 
* Other attributes depending on the selected object type. 

1. Click on the column headers to sort and filter content.
2. Clicks on a row to highlight the Object with a blue frame on its Diagram. This allows users to easily navigate through the found objects and to jump to the place in the process where the object is used.
3. Use the **Select** command on the top left to switch between Object types. This  shows all Object classes that are represented in the Process. If an Object type is selected, only those objects belonging to that Class will be shown. e.g. Tasks or Events.
![Search: Switch Class](images/searchselecttype.png)
4. Search for a specific word by entering the word into the Search text option box.
5. The menu items **Start** and **Stop** can trigger a new search or stop the Search process.
6. **Excel** option exports a list of found Objects to an Excel file if a specific Class was selected beforehand.
7. **Save** writes found Objects items to a JSON file.
