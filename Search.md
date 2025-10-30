# Search Panel

Search is used to find Objects that are used throughout the entire model. This is paticularily helpful in models with a large number of Diagrams or when searching for specific Tasks, Events, or Gateways.

In main menu entry "Home" select "Search" to open the search panel.
![Open Search Panel](images/searchopen.png)

The search panel will automatically trigger a search for all objects in the opened process model and, depending on the object the user selected on the drawing page, will show all objects filtered to this object type. If no object is selected the panel will show all found objects.
![Search Panel UI](images/searchpanel.png)

## Using the search panel

All found objects will be shown in a table, which consists of object name, diagram and some other attributes, that depend on the selected object type. 

1. By clicking on the column headers the user can sort and filter the content.
2. If a user clicks on a row, SemTalk will highlight the object with a blue frame on its diagram. That way the user can navigate through the found objects and can jump to the process positions where the object is used.
3. To switch between object types the user can use the select control on the top left. It will show all object classes that are represented in the process file. By selecting on of those classes the user view only objects the belong to thos class, e.g. tasks or events.
![Search: Switch Class](images/searchselecttype.png)
4. To search for a specific word the user can use the search text box.
5. The menu items "Start" and "Stop" can trigger a new search or stop the search process.
6. The "Excel" item will export a list of found objects to an Excel file, if a specific class was selected beforehand.
7. "Save" will write als items from the panel to a JSON file.
