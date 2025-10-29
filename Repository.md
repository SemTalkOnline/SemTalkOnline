# SemTalk Object Repositories

Repositories are the SemTalk database libraries where the names of Objects, Methods, States, Human Resources and Attributes are managed. They can be used across document and also for multiple SemTalk Online instances to share predefined company vocabulary everywhere its needed.

Repositories provide predefined modeling objects that are designed to keep model data consistent throughout the model landscape. Users insert those objects from picklists that are integrated with the **Select** and **Vocabulary** functionality of Semtalk. 

A new file will be automatically connected to the Repository, if it is set up correctly in the settings of the user or for the App instance. It can also be used for multiple SemTalk Online instances.

For learning more about how to use those functionalities and Repository objects read more in [Wiki page: Vocabulary](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Vocabulary) or [Wiki page: Working with objects](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Working-with-Objects)

## Content of a Repository

A Repository consists of some lists to store the vocabulary, connections and translations. Those list typically are:
- Objects: Contains the business objects for the vocabulary. Information about class structures, connected methodes or states is included as well in this list.
- Methode: Contains the methods that can be used for the vocabulary.
- State: Contains the states that can be used for the vocabulary.
- HumanResources: Roles are stored in this list.
- PhysResources: Ressources als listed here.
- Buffers: Buffers are the systems that can be used to visualize data storage.
- AttributeType: Attribute types can be listet here.


## Setting up a Repository

Repositories can be hostet with Microsoft Sharepoint or MongoDB databases and mandate different steps to set the Repository up for use. 
If the default and test database on semtalkonline.semtalk.com is used, a repository is already integrated and the setup steps are not needed anymore.

### Setting up a Repository in SharePoint for SemTalk Online in Microsoft365

A Repository for the Microsoft365 environment is stored on a SharePoint site that comes with Microsoft Teams and SharePoint. 

To set up a new Repository a user with admin rights needs to use SemTalk Online functionality to create aforementioned lists on an existing SharePoint site.

Open SemTalk Options --> Microsoft365 --> Button "Create Repository"
![Create Repository](images/repository/createrepository.png)

A new panel opens, which shows all lists that will be created on a selected site. The user needs to select a Teams site/Sharepoint site and afterwards click the "M365 Export" button. SemTalk Online will create all lists an the choosen site. This concludes the setup process for Repositries in Microsoft365.

![Create Repository Panel](images/repository/createrepository2.png)

The created Repository needs to be configured in SemTalk Online options. Open SemTalk Options --> Microsoft365 --> Repository. The site of the Repository need to be entered in a specific way to be used to access it via Microsoft Graph.

* * /sites/<domain>.sharepoint.com:/sites/<sitename>:/ * *

Add the domain of your organization and the selected site name to the template string and add it to the field "Repository"

![Add Repository to settings](images/repository/repositoryoption.png)

### Setting up a Repository in MongoDB

## Using the Repository

### UI and functionality of the Repository

Open the Repository with menu entry "Home" --> Repository

![Open Repository](images/repository/openrepositoryopen.png)

Initially the Repository will be empty and should like in this screenshot.
![Repository UI](images/repository/repositoryemptyui.png)

The menu of the panel gives the user multiple option to view or extend the vocabulary of the Repository.

- Selectbox: Lets users choose with kind of object they want to look at. Business Object, Human Ressources, Buffers etc. After a type is selected the table will show all objects of the selected type that are stored in the Repository.
![Repository select type](images/repository/repositorycategories.png)
- Add: Lets the user add an object to the selected type. After clicking the "Add" button the user can enter a name of a new object and need to complete the transaction with the "Ok" button. If a process model has objects that are not in the Repository, the dialog will let the user select from a list of those objects to add to the Repository.
![Repository add Object](images/repository/repositoryadd.png)
Afterwards the new object will be inserted in the Repository.
![Repository Object is added](images/repository/repositoryadded.png)
- Delete: Lets the user delete an object from the Repository. After clicking the button the user get a list from which they can choose one or more entry to delete. Those object will then be deleted from Repository but not from all model files where are used.
- Link to Repository: If a Repository and a process file have used the same objects but these objects are not linked, the user can use this function to link the Repository object to the objects from the process file. Otherwise a export to the Repository would lead to redundencies.
- Export to Repository: By clicking this button users will export all objects from their model to the Repository. Users need to treat carefully to avoid inserting wrong or redundant objects.
- New List: Adds a new List to the Repository for cases where other objects then the default objects are needed. This functionality will only be for users with admin permissions.
- New Column: Lets users create more columns for existing lists. This functionality will only be for users with admin permissions.
- Export Excel: Exports Repository ojects to an Excel file
- Import Excel: Imports an Excel file and creates Repository objects out of the providied data

### Using Repository objects in process models

To demonstrate how to use Repository objects take a look at the following scenario:

The Repository consists of a few objects, methods and roles.
![Repository: Objects](images/repository/repositoryobjects.png)
![Repository: Methods](images/repository/repositorymethods.png)
![Repository: Roles](images/repository/repositoryroles.png)

Now these elements will be used in a fresh BPMN process file. First object and methode will be added to a task by right clicking on the task and selecting "Vocabulary" from the context menu. A new panel will open.
The selectbox for object and method will show the vocabulary from the Repository and can be used from the user.
![Repository: Objects in Vocabulary](images/repository/repositoryobjectsvocab.png)

The vocabulary menu is available forevents and gateways as well, but in this case the user will select an object and a state.

For roles it works by using the "Select" menu. This is available by right clicking on the role item. In BPMN this is the swimlane. The panel show the role objects from the Repository.
![Repository: Roles in Select menu](images/repository/repositoryrolesvocab.png)

For more information about objects in read [Wiki page: Working with objects](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Working-with-Objects).

### Editing objects and refresh model content

Object in the Repository can be edited directly in each cell.
![Repository: Roles in Select menu](images/repository/repositoryobjectchange.png)

**Please note:** A change in the Repository will not automatically change the process files, in which the object is used. To refresh the objects in the model as well the user needs to select the object and then click "Refresh" in main menu entry "Object" --> "Repository".
![Repository: Roles in Select menu](images/repository/repositoryobjectchange2.png)
![Repository: Roles in Select menu](images/repository/repositoryobjectchange3.png)











