**SemTalk Online** integrates seamlessly into the Microsoft 365 environment. This allows organizations to use SemTalk Online directly within familiar Microsoft environments such as Microsoft Teams, Outlook, and other Office 365 services. By embedding into the existing Microsoft environment, users benefit from a unified workspace where process modeling, collaboration, and knowledge management are fully connected with the tools they use every day.

# SemTalk Online App as a Personal Tab in the Microsoft 365 Environment

Users can set up SemTalk Online as a personal tab in Microsoft products such as Teams or Outlook Online. To do this, the SemTalk Online App must be selected from the "More Apps" menu of the respective Microsoft application.

This scenario is particularly suitable for modeling by individuals who do not need to manage large amounts of models.

For personal apps, there is no separate settings screen in the Teams or Outlook environment, no SharePoint site in the background, and no caching of personal settings. Therefore, it is recommended to work without a fixed model library.
More details can be found under [File storage options](https://github.com/SemTalkOnline/SemTalkOnline/wiki/SemTalk-Online-Options-for-file-storage) genaueres gelesen werden.

SemTalk Online App as a Microsoft Teams Tab

# SemTalk Online can be added as a tab in a Microsoft Teams channel.

This scenario provides the optimal way to use SemTalk Online as a shared modeling solution for a group of people working together on projects. All authorized users of the respective team have access to the same app with the same settings and configurations.
In addition, all functionalities of Microsoft Teams can be used to make the modeling experience more efficient and collaborative, e.g., chat function, integration of related libraries and other information. Data storage for SemTalk Online can also be specifically set to a library within the respective team. Other settings can also be predefined by a SemTalk Online administrator for all users of the SemTalk Online instance.

This is the recommended option for creating and managing larger and more detailed model landscapes with multiple modelers over the long term.

## Adding the App as a Teams Tab

The SemTalk Online App can be added to a Microsoft Team in a channel as a tab using the standard mechanisms, making it available to all members of the channel.

When first setting up, the user is prompted to fill in the tab configuration.

## Configuring the Tab

The configuration screen of the SemTalk Online App provides the user with numerous basic setting options to preset the application for different use cases.
The settings made there apply to all users of the tab, unless individual users change their personal settings and thereby override the tab defaults.

![Tab Konfiguration](./images/Tabconfig1.png)

- Tab Name: The name that should be displayed in the tab title.
- Role: The role in which the app should run.
- SharePoint Site URL: If a fixed library is to be used for storing files, the URL of the SharePoint site must be specified here.

![Tab Konfiguration](./images/Tabconfig2.png)

- Library: The name of the fixed library. This must exist on the previously specified SharePoint site.
- Folder: If desired, a specific folder from the library can be specified here.
- Shared Library: If an additional library is required as an extra storage location for shared processes, it can be specified here. This must have a different name than the regular model library.
- Repository: If modeling with SemTalk Repository, the SharePoint site where the repository is located must be specified. For more information about the repository, see: Wiki Page: Repository

![Tab Konfiguration](./images/Tabconfig3.png)

- UI Language: The language in which the SemTalk Online interface is displayed.
- Current Language: The language in which model content will be created.
- Use Microsoft Graph: Must be enabled if SharePoint libraries are to be used as a file storage location.
- Use MongoDB: If a MongoDB is to be used as a model database, MongoDB must be enabled and Microsoft Graph disabled.
- Enable Single Sign-On for MongoDB: Microsoft 365 accounts can be registered in MongoDB and then used for login.
- MongoDB Token: If MongoDB is used, the token for the database is required.
- Settings String: SemTalk Online allows all option settings to be exported as a JSON string. This string can be entered in this field to provide the same default settings for all users.

![Tab Konfiguration](./images/Tabconfig4.png)

- Enable Portal Mode: SemTalk Online can also be used as a portal in the future. This must be activated here.
- Start File: Which model file should be the starting point of the portal?
- Start Diagram: Which diagram should be the start diagram of the portal?
- Subsite Prefix: Each SemTalk Online App gets an individual prefix. This is used to cache user-specific settings on the computer for each portal instance.


# File Storage Options in the Microsoft Environment

More detailed information about SemTalk Online’s file storage concept can be found on the page [File storage options](https://github.com/SemTalkOnline/SemTalkOnline/wiki/SemTalk-Online-Options-for-file-storage).
There you can also find information about the available options in the Microsoft 365 environment.



