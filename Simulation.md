# Simulation

![alt text](images/SimStartEventAll.png)

SemTalk Online includes the ability to use special simulation-specific properties to analyze process flows. Behaviors of specific objects, or of execution flows, are analyzed to estimate variables such as waiting times and costs. Users can also customize these attributes to execute more sophisticated calculations, or to create custom dialogs related to dynamic behavior. 

EntryPoint Simulation Properties:
* Process Start and End Times
* Priority
* Distribution Type
* Jobs
* Period
* WorkTime
* WorkTime2

Task Simulation Properties
* CostDriver
* Priority
* Distribution Type
* WorkTime
* WorkTime2

SequenceFlow Association Simulation Properties
* TransportationTime
* FixedCost
* VariableCost
* Probability
* ConditionExpression
* Restart

Buffer Simulation Properties
* Capacity
* FixedCost
* InitialContents
* FlushTime
* FlushNumber

HumanResource Simulation Properties (Simulation Properties are edited in the OrgChart)
* Capacity
* Strategy
* SetUpTime
* FixedCost
* VariableCost

Right mouse click on an **EntryPoint, Task, Buffer or Association Object** in a Business Process and select **Properties** to access **Simulation Properties**. Right mouse click on a **HumanResource** in an **OrgChart** to open **HumanResource SimulatiomProperties**.

![alt text](images/SimulationHumanResources.png)