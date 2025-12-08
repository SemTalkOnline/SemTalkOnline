# Working With Ontologies

## Introduction

SemTalk Online is able to create knowledge models in the form of **Ontologies**. **Ontological Classes** are groupings of **Objects** that have common **Properties**, or they are **Classes** within specific **Domains**. 

**Objects** modeled using **Ontologies** are integrated into the picklists used when modeling. These picklist **Objects** inherit the **Properties** defined in the **Ontology**.

Ontologies can be modeled independently in an **Ontology Template Models** or they are created within  **Business Process** and **EPC Models** when using the **Vocabulary** function when naming process flow Objects. 

**NOTE**: If an **Ontology Model** exists, the Objects in the Ontology Model can be integrated into **Business Process** and **EPC Models** using the Meta Model that is used to share process model data in all modeling activities within an organization.

## Create an Ontology Model

 Select the **Ontology Modeling Template** option when creating a **New Model**. 

**Class Representation**

SemTalkOnline distinguishes between two types of representations: Ontological **Classes** and **Instances of Classes**.

![alt](images\Ontology1.png)

In the above example, **Classes** are represented as white ellipses, while **Instances** are represented by gray ellipses.

Ontological Classes can also be represented as rectangles in accordance with the UML standard. These UML views show associated **Method** names in addition to the **Class** names. Please refer to the Showing/ Hiding Attribute section shown below.

**NOTE:** The default color scheme for Ontology Objects can be changed using **Style**.

## Create an Ontology in Process Models

**BPMN or EPC** SemTalk Online versions can add ontological components by integrate **Ontology Diagrams** into models. 

Select **Diagram - New - Ontology**. 

**NOTE**: If **Diagram - New - Ontology** is not shown in the **Diagram - New** pull-down menu, please contact the model's **Administrator** to add the Ontology function to the model.

![alt text](images/BPMNOntologyNew.png)

SemTalk Online's Ontology Diagram's default name is **Ontology-1**. Users can rename the Diagram but it is helpful to give the Diagram a new name that differentiates it as an **Ontology Diagrams**.

**Working with Ontology Diagrams**

**Ontology Diagrams** have specific associated **Object** shapes in their **Stencil**.
* **Class**
* **Instance**
* **Comment**
* **Text**
* **Image**

## QuickShapes

**QuickShapes** allow modelers to quickly create linked **Objects** by hovering the mouse over an existing shape and then choosing the desired Object type that should be connected.

 **QuickShapes** modeling elements:
* Instance (gray box): Creates an instance of the Class
* Superclass (arrow): Relationship of the class to a superclass
* Association (angled line): Relationship between two classes

## Showing/ Hiding Attributes

SemTalk Online allows existing Class Attributes to be displayed in Ontologies by activating UML Shapes in **Settings - General - UML Class Shape in Ontologies**.

![alt text](images/UMLCheckbox.png)

Once activated, users right-click on a Class to open **Attributes**. Click on the **Attribute** name to Show or Hide the Attribute.

It is possible to change an Ontology Object from a Class to an Instance or an Instance to a Class.  **Classes** or **Instances**. 

Right mouse click on a Class or Instance and select **To Instance** or **To Class**.

![alt text](images/Class2Instance.png)

The **Color and Properties** of the Object will change accordingly.

### Connectors

Relationships between **Ontology Classes** are created using the angled QuickShape arrow to creat a **Consist of** relationship. 

Select the Class's **Quickshape** and drag the angled arrow to the desired target Object. SemTalk Online automatically names the relationship **Consists of** according to the default settings.

For example, a 'Car' **Consists of** a  'Axel', which **Consists of** 'Wheels'. If the model requires a different relationship, such as, 'Wheels' make contact with the road. Create the new relationship by double-clicking on the **Consists of** relationship between the two Objects and change its name to 'has contact with' and adds the new relationship to the model. Available relationships are listed in **Explorer - Associations**. It shows the **Associations** and shows that it is linked to the **Class** 'Wheel'. 

**NOTE**: Relations are directed, which can be seen from the angles in front of the relation name in the tab. In the graphical representation, relations are shown as arrows with a direction. 
