## **BPMN Overview**

Business processes are described graphically in SemTalkOnline using the standardized “Business Process Model And Notation.” BPMN provides a set of Business Process modeling Objects along with guidelines for their use. SemTalkOnline incorporates these BPMN rules into a set of drawing Diagrams, each with an associated Stencils that contain relevant Object types that can be dragged and dropped onto the Diagram (drawing sheet). 
BPMN is currently published as Object Management Group (OMG) [BPMN 2.0](https://www.omg.org/spec/BPMN/2.0/).

**Core elements**

The following is a brief description of the “core elements” used in a Business Process Diagram.
* Events:  Events describe singular occurrences that control a Business Process flow. These include Inputs (start), Outputs (end) and intermediary events that end or interrupt a process flow.
* Tasks:  Tasks are the specific activities executed in the process flow. Except for the first and last Tasks (process start and end events), there are always preceding and successor modeling elements defined for each Task. Generally, Task names are a combination of a noun (Object) and a verb (Method). NOTE: When modeling with SemTalkOnline, the Vocabulary naming function is used to create a reusable picklist of Nouns and Verbs. This function keeps model information consistent throughout the organization.  
* Gateways:  Gateways are the branch Objects used to change the direction of the process flow. The process flows from the Gateway to different Tasks depending on the information sent by the proceeding Object. Modelers set the conditions in the Gateway to trigger the appropriate successor task. 
* Flows:  Process Flow Objects are the directional arrows that connect Objects to one another to show the direction of the process flow and to determine what is transferred to successor Objects. Flow arrows define the order in which individual Tasks are processed.
* Swimlanes: Swimlanes represent an overarching view of the Participants  (Jobs/ Org Units etc.) that perform the Tasks shown in the process flow.  Process flow arrows show the handoff between the Tasks done by each Participant Swimlane. NOTE: Each Participant is assigned its own independent Swimlane so that it is clear which Tasks are performed by each group.

**Example:**

The following is an example of a BPMN Business Process Diagram:

![alt text](images/BPMN_Overview.png)

Business Processes are generally read from left to right. 
A process begins with initial input Events and ends with pre-defined output Events. Between the two are a defined process sequence of Tasks (process steps) with directional arrows showing the process Flow. Tasks can be followed by Gateways that show branches that occur in the process flow based on incoming conditions. The example Gateways show above relate to the completion of testing results.  “Is the complete?”. If ‘Yes’ go to the end Event “All Tests Complete”, if ‘No’ go to “Perform Test’.”
Process flows are embedded in Swimlanes to show the how different Participants interact within a Swimlane or in other Swimlanes that are working on the same process.
