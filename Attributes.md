**Attributes** are a set of system or user-defined properties related to an Object. 

Add the Attribute tab to your Object using Customization.

Open the Object's Properties using your right click menu and select Attributes and then select New.

![](https://github.com/SemTalkOnline/SemTalkOnline/blob/main/images/Attributes2.png)

**Object - Properties - Attributes**:  SemTalk allows users to add Attributes to Objects. As Attributes are added, they will be stored in your Respository. They can be created or managed in:

* Object - Properties - Attribute tab, 
* Using the Worksheet option, or 
* When naming Object using the Vocabulary naming function.

In SemTalk, there are two Attribute types:

* **System Defined Attributes**, which represent the standard GUI views for Objects, and 
* **User-Defined Attributes** which are created by users for their currently active model. 

Both Attribute Types have variables with associated values. System-Defined Attributes are the standard entries shown in the Properties tabs. Only SemTalk product developers are able to change System Defined Attributes. The SemTalk GUI can be customized using Attributes and configurable layout features.

![](https://github.com/SemTalkOnline/SemTalkOnline/blob/main/images/Attributes1.png)


In the above example, the 'Product' Object has been given the Attribute 'Delivery Date'. 'Delivery Date' consists of a Date variable extracted from a calendar. Variables can also be a pick list such as 'Currency Type' (e.g. a picklist with US Dollars, Euros, Pounds etc.) or it could have a fixed range such as from 5-100. 'Delivery Date' variables are defined as Attributes in the superclass 'Product'. 'Product' subclasess are all available products such as 'Product X'. Users create User-Define Attribute would be assigned to the class 'Product' and 'Product X' would inherit the Attribute 'Delivery Date'. Specific Values are set within the individual Products appear when these object are in a process flow. 'Product X' is set to Delivery Date = June 27th, 2022. 

Once a User-Defined Attribute has been created, it can be assigned to other Objects by choosing it from a picklist when the Attribute tab is selected. 

