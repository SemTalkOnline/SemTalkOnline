
## Introduction

SemTalkOnline integrates a shared knowledge platform using **Ontologies**. Ontological **Classes**, or concepts, are groupings of things with common **Properties** that describe the **Objects** that exist within a specific **Domain**. Objects that have been modeled in an Ontology are shown in picklists that are shown when modeling. When modelers choose an Object from a picklist it automatically shows the Object's **Properties** that were defined when creating the Ontology.

Ontologies can be modeled independently in an **Ontology Model** or they are created within  **Business Process** and **EPC Models** when using the **Vocabulary** function when naming process flow Objects. 
NOTE: If an **Ontology Model** exists, the Objects in the Ontology Model can be integrated into **Business Process** and **EPC Models** using the Meta Model that is used to share process model data in all modeling activities within an organization.

Select the **Ontology Modeling Template** when creating a new Ontology model. 

**Class Representation**

SemTalkOnline distinguishes between two types of representations: Ontological **Classes** and **Instances of Classes**.

![alt](Wikis\images\Ontology1.PNG)

In the above example, Classes are represented as white ellipses, while instances are represented by gray ellipses.
However, classes in ontologies can also be represented as rectangles in accordance with the UML standard, which also allows you to see the associated method names in addition to the class names.
To obtain this representation (UML notation), the checkbox “UML Class Shape in Ontologies” must be selected in the general options.
Note: The default color scheme can be changed by the user at any time.

##Creating New Ontologies

**Create a New Ontology Model**

* Select **File -> New** from the main menu.

Select the ‘Ontology’ option and confirm with “OK.”

SemTalk Online will open the appropriate Diagram with the corresponding Ontology Objects. NOTE: only ontologies can be created as additional diagrams/drawing sheets in an ontology model. This is different for business process models. In these, ontologies can also be included as additional diagrams alongside business processes.

#Creating Ontology Models for Business Process Models

SemTalkOnline offers users the option of creating an Ontology for existing Business Process Models so that modelers can integrate existing knowledge in a structured, integrated manner. 

* Select the **Diagram - New** in the main pull-down menu.
* Then select the “Ontology” template. SemTalkOnline responds immediately and suggests the name “Ontology-1” in the **Name** field. Users should edit this name to the name of their choice and then select **OK**.

**Working with Ontology Diagrams**

* When selecting an Ontology as a model template this option also determines the type of Diagram that SemTalkOnline uses to provide the user with the Object shapes used for modeling.

Simply drag and drop these Object shapes onto your **Diagram**.

Editor level Modelers will see the following Object shapes:
•	Class
•	Instance
•	Comment
•	Text
•	Image

**QuickShapes**

QuickShapes allow modelers to quickly create linked Objects by hovering the mouse over an existing shape and then choosing the desired Object that should be connected to the selected Object.

These modeling elements can be selected from the QuickShapes
•	Instance (gray box)
•	This creates an instance of the relevant class.
•	Superclass (arrow)
•	This establishes the relationship of the class to a superclass.
•	Relation (angled line)
•	This establishes a relationship between two classes.
Showing and hiding attributes
SemTalkOnline allows class attributes to be displayed in ontologies, provided that attributes have been defined. To do this, however, it is necessary to first set the display type to “UML Class Shape” in the options.
The user can then right-click on a class to open the context menu, which contains the “Attributes” entry. By clicking on “Attributes,” the attribute names for a class can be shown or hidden.
Switching between classes and instances
SemTalkOnline offers the option of switching back and forth between classes and instances in an ontology. If you start with a class, you can call up the “Make instance” function in the context menu.
As a result, the class has now been converted into an instance (gray oval) that has taken on the same name as the class.
By calling up the context menu again, you can turn the instance back into a class by selecting the “Make Class” function.
If the class already has one or more attributes, these attributes are retained.
Relations
To establish a relationship between two classes in an ontology, use the “angled line” QuickShape (see section on QuickShapes above). To do this, activate the “Relation” QuickShape on the class from which the relation is to originate and ‘drag’ the arrow that appears to the class to which the relation is to be formed. SemTalkOnline then names the relation according to the default setting (in the example, “consists of”).
A car consists of, among other things, the chassis, which in turn consists of, among other things, wheels. If you now want to express that the wheels make contact with the road, this must be expressed by another relation (such as “has contact with”). To do this, you first establish a relationship between a “wheel” and the “road surface,”
but then you have to change the name of the relationship. To do this, double-click on the relationship and you can then change its name.
SemTalkOnline stores the new relationship in the model, which the user can easily check in Explorer (-> Objects) (see screenshot). Here you can see all relations (tab “Associations”) that are linked to the class “Wheel.” The additional relation “has contact with” is highlighted in yellow.
Note: Relations are directed, which can be seen from the angles in front of the relation name in the tab. In the graphical representation, relations are shown as arrows with a direction.
Linking ontologies with business process models
General remarks
SemTalk Online makes it possible to store additional knowledge about objects that are handled in business processes in the form of ontologies. However, this requires that the objects in a business process have been previously stored in the database using the vocabulary function. You can check this by selecting a task in a business process and then applying the vocabulary function to it. If the fields in the dialog box that appears are filled in, the object (and method) have been correctly stored separately in the database. If the relevant fields are empty, there are no corresponding entries for the object or method.
If you open the Object Explorer, you will not find any entries.
Note:
The task already exists, of course, but can be found elsewhere in the Object Explorer, namely when you expand the Explorer in this order: “Flow object” -> ‘Activity’ -> “Task” ->
Selecting an existing object for referencing in an ontology
First, make sure that the current drawing sheet/diagram belongs to an ontology. Then right-click anywhere on the drawing sheet. In the context menu that appears, select the “Insert” function.
A comprehensive selection dialog will then appear, from which you can select the desired objects by checking the boxes.
Note:
It is also possible to restrict the selection list to objects only. To do this, set the filter in the “Metamodel” column to “Object.”

Finally, click on “Insert” (at the top left of the dialog box) to make the selected objects visible in the ontology.

