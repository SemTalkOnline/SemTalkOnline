SemTalk Online allows storing files in different ways

* Locally on the computer
* In SharePoint libraries
* In a MongoDB

# Storing files locally on the computer

Users have the option to save model files on their own computer and open them from there.

As soon as the checkboxes for MongoDB and Microsoft Graph are disabled in the SemTalk Online options and the user is not working in a SharePoint context, SemTalk Online switches to local mode. In this case, when clicking on "Save" or "Save As", the current model file is automatically stored in the user’s Downloads folder.
The Open dialog then allows the user to select a file from this folder for editing by automatically opening the file explorer.

![Graph and MongoDB disabled](./images/GraphMongoDisable.png)

![Opening local file](./images/dateioeffnenlokal.png)


But even if MongoDB or Microsoft Graph are enabled, files can still be stored locally. For this, the Save dialog provides a "Download" button, and the Open dialog offers a "Browse" button.

![Browse or download files](./images/filebrowsedownload.png)


# Storing files in SharePoint libraries

## Advantages
If users have access to a SharePoint server, they can store the files directly in SharePoint libraries. The advantage of this is that SemTalk Online can be seamlessly integrated into the company’s existing file structure, and user and access management can be organized via existing Microsoft 365 accounts and the corresponding permissions in Teams or SharePoint.

In addition, all functionalities of SharePoint file management can also be used for SemTalk Online files, such as versioning, metadata columns, etc.


## Login process
If the use of Microsoft Graph is enabled or SemTalk Online is used in a Microsoft SharePoint context, files can be stored in SharePoint libraries. However, users must be logged in with their Office 365 account.

If SemTalk Online is run as a Teams tab or otherwise within the Microsoft 365 environment, users are already logged in, and SemTalk Online uses the user’s account and granted permissions to access files via Microsoft Graph.
In exceptional cases, it may be necessary to log in again using the M365 Login button from the user menu.

![Log In with Microsoft 365 Account](./images/m365login.png)

When using the SemTalk Online web application, after activating Microsoft Graph, a login with the user’s Microsoft 365 account is mandatory. It is also required again for each session, since the web application runs outside the user’s Microsoft 365 environment.

## Using a predefined fixed library

SemTalk Online can be operated with a fixed, predefined SharePoint library for all users. This makes sense especially when several modelers are working together on model files in a structured way over a longer period of time.

This scenario is possible when SemTalk Online is used as a tab in Microsoft Teams, as a SharePoint WebPart, or as a web application with access to a SharePoint server.

In the SemTalk options, under the Microsoft 365 tab, this configuration can be viewed. In the example image, the library is named "SDX" and is located on a site called "Modellierung". A folder could also be specified. The user must, of course, have read/write permissions for the SharePoint site in order to open and save files in the given library.

![SemTalk options for fixed library](./images/fixedlibrary.png)

A user with administrative rights can change these settings for all other users and set them as default.
When SemTalk Online is used as a tab in Microsoft Teams, the library name and SharePoint site must be entered directly in the tab configuration when it is created.

## Working without a fixed library

It is also possible to work in a mode where the file storage location can be chosen for every save or open operation. This can be enabled by disabling the "fixed library" option in the SemTalk Online settings.

All users can then freely decide where to store or open files from.
When SemTalk Online is used as a personal app, this mode must be used by default, since there is no way to predefine settings information — a personal app does not exist as a SharePoint structure like a team and therefore has no libraries or other storage locations available.

In the SemTalk options, the use of a fixed SharePoint library can be disabled.

![SemTalk options: fixed library disabled](./images/withoutfixedlibrary.png)

In the Open as well as in the Save dialog, a SharePoint site must then always be selected. This is done by entering the name or part of the name of a SharePoint site (of which the user is a member) into the search box of the dialog and starting a search. SemTalk Online will show all matching SharePoint sites and allow the user to navigate within them and select a specific library for saving.

![File open without fixed library](./images/withoutfixedlibraryopen.png)


# Storing files in a MongoDB

## Advantages
A MongoDB is well-suited as a database for SemTalk Online because it offers a flexible, document-oriented structure. Model information, metadata, and user interactions can be stored directly as JSON-like documents without requiring a rigid schema. This simplifies the management of complex and variable model contents.

MongoDBs can be hosted in the cloud as well as on your own servers, making them flexible and quick to set up.

MongoDB was therefore chosen as the database system for SemTalk Online outside of the Microsoft environment.

When SemTalk Online is used with MongoDB, all users must create an account on this database and log in before they can work with it.

## Creating and setting up a MongoDB

On request, Semtation GmbH supports new customers in setting up a MongoDB server. However, every customer also has the option to take care of it independently and operate and manage the server themselves.

A MongoDB can be booked in the cloud, for example via https://account.mongodb.com/
.
It can also be created and operated directly in Microsoft Azure.
If your organization has its own server infrastructure, MongoDB can also be installed locally: https://www.mongodb.com/docs/manual/installation/

Once the MongoDB server has been set up, the server connection string must be converted into an encrypted token, which must then be stored in SemTalk Online.

In the SemTalk Online options, under the MongoDB tab, you will find guidance for the final setup of your database.

![SemTalk Optionen: Neue Datenbank einrichten](./images/copydb.png)

- Select Copy database or repository
- Paste the server’s connection string into MongoDB Server
- Click Encode and store the generated connection token in a safe place (this token can later be entered in the MongoDB Connection field to connect to your DB)
- In the field Type, select Library
- Under Source, select empty. This represents an empty DB that serves as a template for the new database
- Under Target, enter the name of the new database collection, e.g. semtalkonline. This collection will be created on the server during the copy process and filled with the corresponding database tables
- Finally, click Copy. The new database will now be initialized with the basic information.


## Storing the MongoDB connection token
How the MongoDB token is stored in SemTalk Online depends on the type of SemTalk Online application.

In the web application, the token can be inserted into the MongoDB Connection field in the options under the MongoDB tab, but more importantly it can be entered on the SemTalk Online start page. There, the Connection button must be used to store the token. When the SemTalk Online application is started for the first time, SemTalk Online will immediately load the corresponding MongoDB server.

![Add MongoDB Token](./images/MongoDBToken.png)

![Add MongoDB Token](./images/MongoDBToken2.png)

![Add MongoDB Token](./images/MongoDBToken3.png)

If you want to set up a MongoDB while SemTalk Online is hosted in a Microsoft 365 environment, please refer to the corresponding Wiki pages for more information.







