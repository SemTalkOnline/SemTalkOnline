## Working with Objects

SemTalk Online is built using object-oriented modeling concepts. All SemTalk Online versions contain Class **[Diagrams](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Diagram-Overview)** where core modeling elements and their their **[Properties](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Properties)**  and **[Associations](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Associations)** are modeled, along with any associated **[Object Properties](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Properties)**. **Objects** in **Object Diagrams** are presented to modelers as **Object Picklists** when modeling process flows.

**NOTE**: The SemTalk Online **[Ontology](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Workin-With-Ontologies)** version only contains Object Diagrams. 

Process flow SemTalk versions, such as **BPMN 2.0 and EPC**, contain separate **Object Diagrams**. Objects in Object Diagrams become **Object, Method and State** Picklists used when **[Vocabulary](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Vocabulary)** is used to model process flows. Nouns are entered as **Objects**, verbs are entered as **Methods** and the state conditions are modeled as **States**.

When **New Objects** are added as a process flow is being modeled (as new nouns and verbs and states are added via the **[Vocabulary](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Vocabulary)** dialog), those **New Object Names** are automatically added the **Object Class Picklists**. These newly defined Objects can be added to the Object Class Diagram via the right mouse click Insert command in an **Object Diagram**. 

Central management of core **Objects** allow modelers to add **[Object Properties](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Properties)** (e.g. Comments, Attributes, or embedding links) to the **Object** in the **Object Diagram** that will be inherited by all Instances of the Object in all process flow Diagrams. 

SemTalk Online's object-oriented concepts improve overall model accuracy, decrease modeling time, minimize redundancies (e.g.modeling the same objects using different names) and greatly improve the overall usefulness of models due to centralized management of associated documents and links.

Object-based elements include, among others:
* Roles/process participants (BPMN)
* Systems/data storage (BPMN)
* Data objects (BPMN)
* Organizational units
* Services (EPC)
* Material resources (EPC)
* Class (EPC)
* Technical terms (EPC)

Important tips when working with **Objects**:

**Create an Object**:
* Drag and drop Objects from the **Stencil**
* Import Objects from **Excel** or from a **Repository**

**Name an Object**:
* Double click on the **Object**, 
* Open the Object's right-mouse click menu
* Use the **[Vocabulary](https://github.com/SemTalkOnline/SemTalkOnline/wiki/Vocabulary)** naming option 

**Connect Objects**:  
* Hover your cursor over the center of an Object until the hand icon appears. Hold down your cursor and draw the connection to the next object. 
* Right mouse on an Object and select a target Object

Connection types are dependent on the **Diagram Type**. Users are able to create user-defined connectors but it is generally not recommended because user-defined connectors are not considered when running process flow consistency checks.
