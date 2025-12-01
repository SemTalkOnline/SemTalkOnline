
# Working with Ontologies

## Introduction

SemTalk Online is able to create knowledge models in the form of **Ontologies**. **Ontological Classes** are groupings of **Objects** that have common **Properties** or they show the subsets of Classes within a specific Domains. 

 **Ontologies** can be created in **Ontology Diagrams** in BPMN and EPC models or they can be created independently using SemTalk Online's **Ontology** model template.

## Class Representations

SemTalk Online distinguishes between two types of Ontological Class representations. The first is the standard Class representation that shows  geneneral ontological concepts and their relationships to one another. The second is for the specific Instances of those Classes.

Classes are generally represented as white ellipses with thicker grey frames and Instances are shown as ellipses with thinner grey frames. 

Ontological Classes can also be represented in accordance with UML standards as rectangles. The rectagular option shows both the Class Object (nouns) and the Methods (verbs) associate with the Class.

Select the **Settings - General - UML Class Shape in Ontologies** to use UML Notation.

**NOTE:** The default color scheme can be changed at any time using **Style**.

## Create an Ontology

**BPMN or EPC** Ontologies are modeled on **Ontology Diagrams**. If **Diagram - New - Ontology** is not shown in the **Diagram - New** pull-down menu, please contact the model's **Administrator** to add the Ontology function to the model.

![alt text](images/BPMNOntologyNew.png)

SemTalk Online will suggest to name the Diagram **Ontology-1**. Users can rename the Diagram but it is helpful to give the Diagram a new name that differenciates **Ontology Diagrams** from other **Object Diagram** types.

Ontologies can also be created in **Ontology** model templates. These models do not have process flow representations, they only contain ontological information. 

Select **File -  New** from the main pull-down menu. Then select **Ontology** as the new model type and select **New**.

SemTalk Online will open the **Ontology** model template with the standard default Class representations or with the **UML** representation if it was selected in **Settings - General**.

![alt text](images/UMLClassShape.png)

## Working with Ontology Model Templates

In **Ontology** template models, the following **Ontology Stencil Shapes** can be dragged and dropped onto the Diagram:
- Class
- Instance
- Comment
- Text
- Image

## Modeling with QuickShapes

![alt text](images/QuickShapeOntology.png)

**Quickshape** allows users to directly model related Objects and Connectors by hovering the cursor over an existing source shape and selecting one of the following Shapes:

#### Circles Used to Create New Objects with Associated Connectors:
- Dark Grey Circle: Creates an Instance of the source Class
- Light Grey Circle: Creates a new source Object Superclass

#### Connectors to Link Existing Objects:
- Straight Line Arrow: Creates Subclass/ Superclass relationships between Subclass source Objects and Superclass target Objects.
- Perpendicular Line: Creates a default **Consists of** is a default association name used as a placeholder designation for user-defined associations. Just click on the **Consists of** relationship to edit it.

**NOTE**: When using Quickshapes to add Objects, Object placement is limited to a parallel or lower position than the position of the Superclass. 

## Showing/ Hiding Attributes

SemTalk Online allows existing Class Attributes to be displayed in Ontologies by activating UML Shapes in **Settings - General - UML Class Shape in Ontologies**.

![alt text](images/UMLClassShape.png)

Once activated, users right-click on a Class to open **Attributes**. Click on the **Attribute** name to Show or Hide the Attribute.

It is possible to change an Ontology Object from a Class to an Instance or an Instance to a Class.  **Classes** or **Instances**. 

Right mouse click on a Class or Instance and select **To Instance** or **To Class**.

![alt text](images/Class2Instance.png)

The **Color and Properties** of the Object will change accordingly.

### Connectors

Relationships between ontology classes are created using the perpendicular QuickShape arrow (Refer to the QuickShapes section above). 

Select the Class' **Quickshape** and drag the arrow that appears to the Class to the desired target Object. SemTalkOnline automatically names the relationship according to the default settings.

For example, a 'Car' **Consists of** a  'Axel', which **Consists of**  'Wheels'. If you what to model that 'Wheels' make contact with the road, it requires another relationship, such as 'has contact with'. This requires creating a new relationship between a 'Wheel' and the 'Road surface'. Add this new relationship by double-clicking on the **Consists of** relationship between the two Objects and change its name to 'has contact with'.

SemTalk Online then stores the new relationship in the model and it will be visible in **Explorer - Associations** that shows Associations linked to the class 'Wheel'. 


**NOTE**: Relations are directed, which can be seen from the angles in front of the relation name in the tab. In the graphical representation, relations are shown as arrows with a direction.

## Linking Ontologies with Business Process Models

SemTalk Online is able to integrate Business Process Object knowledge with  **Ontologies**. This integration uses the Vocabulary naming structure for business process **Task/ Event** Objects and Methods. 

Check to see if a model is built using Vocabulary by opening a Business Process Diagram, right mouse click on an Task and select Vocabulary. When Vocabulary is used, the Object Name and the Method  will be shown. If those fields are blank, it is not a Vocabulary model. 

Select **Diagram - New - Ontology**. If Ontology is not listed in the **Diagram - New** menu, contact the model's Administrator to turn on the Ontology feature. Then open a new Ontology  Diagram, right mouse click anywhere on the Diagram, and select **Insert**.

A dialog will appear with available **Objects**. These **Objects** can then be **Inserted** onto the Ontology Diagram.

**NOTE**: In order to only insert Objects, set **Metamodel** column to “Object”.

