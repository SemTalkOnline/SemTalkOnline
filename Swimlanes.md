## **Swimlanes and Swimlane Pools** 

**Swimlanes** and **Swimlane Pools** are used in process flow diagrams to visually and structurally show who or what is responsible for each step in a process. Process flows between Swimlanes describe how these steps interrelate based on different actions and/or actors.

**Swimlanes** show the activities and process flows that are executed by a single group.

**Swimlane Pools** contain multiple Swimlanes. Each Swimlane in the pool represents a subgroup of the higher level swimlane.  (e.g. HR, Sales and Logistics are all subunits of Corporation X. Each department has units or teams within the department that execute differt activities.)

NOTE: When working with **Swimlanes** and **Swimlane Pools** it is recommended to first create and position all Swimlanes/ Swimlane Pools before placing other Objects onto your Diagram because future editing is more complicated due to the container behavior of Swimlanes and Swimlane pools.

Create a **Swimlane**: Drag and drop the Swimlane Object from the Stencil onto the drawing sheet.

![SemTalk Online - New Swimlane](./images/Swimlane1.png)

Group multiple **Swimlanes** into a **Swimlane Pool**: Right click on the header of the **Swimlane** or **the Swimlane Pool** and select **Swimlane - New** SemTalk Online will then create a higher level new **Swimlane** that contains the selected **Swimlane** or **Swimlane Pool**.

The Pool **Semtation** contains two Swimlanes - **IT department** and **Aquisition**).

![two Swimlanes](images/swimlanes_englisch.PNG)

A single Swimlane.

![single Swimlane](images/einzelne_swimlane_englisch.PNG)

**Swimlanes and Pools** can be created by:
* Dragging and dropping a Swimlane object from your stencil icons, 
* Right mouse clicking on an existing Swimlane. In the context menu Swimlane --> New
* In the main menu "Process" --> Swimlane --> New

![new Swimlane](images/swimlane_neu_englisch.PNG)

Swimlanes can be displayed **Vertically or Horizontally**. "Horizontal" is the default setting. There are the two ways to switch from Horizontal to Vertical:

* Right click on a existing Swimlane and select **Swimlane - Vertical** 

![new Swimlane](images/swimlane1.png)

Swimlanes are collaps- and expandable:

* right click on a existing Swimlane. In context menu Swimlane --> expand or collapse
* in main menu "Process" --> Swimlane --> expand or collapse

**Caution:** If a Swimlane gets deleted, all its contained shapes will be deleted aswell. 

**Adjusting Swimlane Size**

The size of Swimlanes and Pools can be adjusted individually. Select a Swimlane by left-clicking it. The size can then be adjusted at the respective green shift points.
* move mouse cursor on shift point
* mouse cursor will turn into double arrow, wich specifys in wich direction the Swimlane can be adjusted

![size change](images/swimlane_groesse_anpassen_englisch.PNG)

If required, Swimlanes can be moved, connected to one another or added to Pools.
* hold left-click on to the edge or the header of a Swimlane to move it
* to connect Swimlanes, attach their edges to each other until a dashed red line appears and release cursor to connect them
* to add a Swimlane to a Pool, move it into the Pools header

# ResizeContainer
In SemTalk, to edit Pools and Swimlanes, the option "ResizeContainer" can be used according o preference.
* in user interface left-click on the cogwheel at the top right
* in options menu scroll down to the option "ResizeContainer"
* by default "ResizeContainer" is deactivated, to activate check the little white box with left-click

![resizeContainer](images/resizecontainer_englisch.PNG)

# ResizeContainer on
If activated "ResizeConatiner" will insure that, Pools will always adjust their size to the Swimlanes its containing, when their size is being changed.

**Important:** With "ResizeContainer" activated a Pools size can only be changed indirectly, by adjusting the size of the Swimlanes contained in it.

# ReszeContainer off
When "ResizeContainer" is deactivated Pools will not adjust themself automatically to the sizes of their contained Swimlanes. In this stage Pools sizes can be adjusted manually, however so does the size of Swimlanes.

![resizeContainer off](images/resizecontainer_aus_englisch.PNG)

**Important:** In general, when adjusting the size of Swimlanes within a Pool, it should be noted that the outer Swimlanes cannnot be enlarged or reduced via their shifting points that are located on the outside of the Pool. 
