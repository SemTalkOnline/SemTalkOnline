# Settings

Settings are used to structually and visually customize SemTalk Online.

Settings have multiple functions. For example, they:
 
  * Show what is shown or hidden in the modeling environment,
  * Set the **Shape**, **Navigation** and placement options on **Diagrams**,
  * Customize **Pull-Down Menues & Layout**,
  * Determine relevant **Properties** for each **Object** type, and
  * Link models to external content and tools, 

**General - Settings - Pull-Down Menu**

Click on the gear icon ![alt text](images/SettingsIcon1.png) found to the far right of the Pull-Down menu to open General Setting.

![alt text](images/SettingsIcon2.png)

The following **General Settings** Window will open.

![alt text](images/Settings_General_1.png)


### Settings - General: ###

  * **Ribbon**: Shows or hides Toolbar
  * **Show Toolbar**: Shows or hides Toolbar
  * **BreadCrumb Navigation**: Shows the Breadcrumb Diagram Navigation Bar under the Toolbar. This allows users to quickly navigate to connected higher and lower process **Diagrams**.
  * **BreadCrumb Navigation (even if a single page)**: Shows Diagram Name for single, unlinked pages



  * **Anchor** Commands: Used to show or hide **Pan & Zoom**, **Stencil**, **Properties**, **ChatBot** and **Navigation** Windows. 

 **NOTE**: Modeling tool windows are generally turned on and off when working between the modeling enviroment and showing model data to end-users.
  * **Marker at Hyperlinks**: Shows Hyperlink markers on Objects with linked Documents and Pages.
  * **Underline Refinements**: Underlines the Object's name to show that the Object has an associated **Refinement**.
   * **Left, Right or Floating**:  **Pan & Zoom**, **Stencil**, **Properties**, **ChatBot** and **Navigation** windows can be anchored to the Left or Right or they can be floated on top of the open Diagram
  * **SemTalk CoPilot**: Integrates model data with CoPilot features that are able to suggest next steps or to replace existing model data with data linked via BPMN models. If there is not associated **BPMN** model data, external Object data can be integrated via **Knowledge Graphs**.

![alt text](images/SettingsGeneral_2.png)

**Quick Shapes**: Modelers can rapidly add Objects and Connectors directly from existing **Business Process Diagram Objects** onto the active **Diagram**. Available **Objects** and **Connectors** are shown when the cursor is hovered over an existing **Business Process Diagram Object**. **Quick Shape** features and **Style** can be activated for all future **Business Process Diagram Objects** by turning on **Quick Shapes inherits Style**.

![alt text](images/SettingsGeneral_3.png)

  * **Property Dialog**: Sets the **Format** and **Style** of **Properties**
  * **Allow Negative Coordinates**: Allows 
  **Diagram Objects** to be visualized without Page Layout constraints. 

  ![alt text](images/SettingsGeneral_4.png)

 
  * **ChatGPT API**: Allows modelers to add an access key for their ChatGPT app
 * **Intro Screen**: Turns on and off the **Welcome Screen** that appears when SemTalk Online opens
 * **Namespace**: Adds the **Namespace** Adds a '#' plus Object type abbreviation before an Object's name. This is used primarily when creating Ontologies.

 * **Dialog View**: 
* **Font (Parameters)**: Selects Font, Font Size, Height, and Width for scaling to other applications (e.g. SharePoint)
**Symbol Scale Factor**: Scales all symbol shapes in the model
* **Resize**: Allows all shapes to allow users to determine their shape size. When selected, Style Resize is set to 'on'.

#### Additional Customization General Settings:

![alt text](images/SettingsGeneral_5.png)

  * **SplitEnable**: Allows modelers to add Objects between two Objects on a Process Diagram so that the new Connectors are generated automatically
  * **RotationEnabled**: When enabled, individual Objects can be rotated. Click on an Object and a blue dot will appear. Click on the blue dot and rotate the Object as needed. NOTE: After turning on RotationEnabled, refresh your model to activate.
  * **UMLClass Shape in Ontologies**: Allows Class models to be shown as standard UML class representations.
  * **Auto Save png**: Saves added .png files that can be used by other modelers. Caution must be used when this setting is turned on because it greatly increased the model file size.
  * **Export to Repository after each 'Save**: This setting is used by Model Administrators and Editors to upload Objects into a general shared Repository

### **Setting - Collaboration**

![alt text](<images/Settings Collaboration.png>)

* Auto Checkout
* Auto Save
* Coauthoring
* Change Log

### **Settings - Process**

![alt text](images/SettingsProcess.png)

* BPMN Rules
* BPMN Dialog
* BPMN Sequence Flow/ Message Flow Rules
* BPMN Event Type
* Refine Creates Multiple Entry/ Exit Objects
* Simulation Dialog
* Object Flow
* Direction
* Swimlane Labels
* Swimlane Labels in Breadcrumbs
* Swimlane Spacing
* Planner Integration

### **Settings - View**

![alt text](<images/Settings View 1.png>)

**Language Settings in SemTalk Online**: SemTalk differentiates between the User Interface language and the model's Document Language used for naming Objects and Connections. 

  ![alt text](images/SettingsView_1.png)
  
  **User Interface Language**: SemTalk Online supports the following 9 languages.

![alt text](images/UserInterfaceLanguages.png)

**User Interface Language** Settings are SemTalk Online Commands. Edits are managed by the SemTalk Online development team.


* **Current Document Language**: The Document Language is the language used when naming Objects, 
Diagrams and other content such as Comments. Multiple Document Languages are managed via Reports that can have columns of multiple langages that can be imported to show content based on the local language of the readers.
* Drawing Size
* Landscape
* Header & Footer
* Auto-Complete


![alt text](images/SettingsView_2.png)

User Interface **Font** Settings:
* User **Interface Font**
* User **Interface Icon Color**

**Fluent UI Themes**: Structured, design-token-based parameters used to define the visual appearance of an application that include colors, typography, and spacing—of Objects across the modeling environment.

* **User Interface Theme**: SemTalk Online includes the following Theme options. Modelers can adjust available Themes using the **User-Defined Theme** function.

![alt text](images/SettingViewThemes.png)

* **Drawing Background Color**: This is the default color for Diagram backgrounds
* Text Color
* **User-Defined Theme**: If modelers or organizations have defined Themes, code for predefined  **Themes**, can entered here. Luent UI Themes can be created https://fluentuipr.z22.web.core.windows.net/heads/master/theming-designer/index.html

![alt text](images/SettingView_3.png)

* Icon Height
* Icon Width
  
### **Settings - Cloud**

![alt text](images/SettingsCloud.png)

**Settings - Cloud** is used to
set external connections to and from SemTalk Online, define backup options, copy database and repository information and to Use Microsoft Graph
* **MongoDB**: MongoDB is the standard format for Object
* **Activate Single Sign On for MongoDB**: Allows users to access MongoDB with their Microsoft account
* Keep me signed in
* **MongoDB API**: Pathname to MongoDB
* **Repository**: Name of the associated Repository
* **Number of Backup Versions**: Determines how many backups should be saved centrally. Generally limited to 15

### **Settings - Viewer**

![alt text](images/SettingsViewer1.png)

Settings - Viewer sets the Portal Start File and it contains relevant Portal Settings.


* **Activate Portal Mode**: Activates the model's Portal site
* **Force use of specified start process**: Overrides other setting to fix which Diagram will open as the Start Page for the Portal
* **Start File**: Link to the specific SemTalk Online file
* **Start Diagram**: Link to the default Diagram that opens on start
* **Refine on Click**: Sets the navigation paraemter for opening Refinements
* **Portal Mongo DB Connection**: Link to the Portal's MongoDB
* **Portal DB**: Shows the DB associated with the Portal
* **Portal Library**: Link to the Library associated with the Portal
* **Portal Backend**: Backend for Portal Administrator
* **Ribbon**: Sets which Pull-Down bars and Toolbar tools are visible
