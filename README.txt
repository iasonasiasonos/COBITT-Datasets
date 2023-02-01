This document describes two (2) COBITT scenarios that can be simulated/emulated using two (2) sets of datasets, respectively. 

- Scenario 1: A production pipeline that utilises four (4) IoT/Robotic/CNC machines, which is in line with the production pipeline of a small factory (e.g., Capsule Skateboards Limited).

- Scenario 2: A production pipeline that utilises twelve (12) IoT/Robotic/CNC machines, which is in line with the production pipeline of a large factory.


Both datasets include two (2) types of csv. files: 

- A (x1): encapsulates information about the orders placed through the COBITT Web App.

- B (x4 and x12, respectively): encapsulates logging information regarding individual machines operating at the factory level (as collected through the COBITT Rose-AP). 

Both types of files are described below: 
- A (Orders): 

	OrderDate	
	-----------------
	The date/time indicating when an order has been created/added in the system.

	Name	
	-----------------
	The name of the order.

	OrderStatus	
	-----------------
	The status of the order, i.e., if it is Pending, Failed or Successful.

	MachineTimestamp	
	-----------------
	The timestamp indicating when a machine has started, was working or has finished its task.

	MachineStatus	
	-----------------
	The active status of the machine (i.e., Started, Cutting, Trimming, Moving, Finished).

	DeviceName	
	-----------------
	The name of the machine.

	MachineType
	-----------------
	The type of the machine (i.e., 3-Axis, 5-Axis, ROS2 Robot).

- B (Devices): 
	recvTime	
	-------------------
	The timestamp indicating when a machine has received a command or when a machine has sent data to FIWARE.

	fiwareServicePath	
	-------------------
	The service path of FIWARE, which is "/" by default.

	entityId	
	-------------------
	The unique ID of the entity/machine

	entityType	
	-------------------
	The type of the entity/machine (namely, either IOT or ROS2).

	attrName	
	-------------------
	The name of the attribute (i.e., the name of a command or a property like start, stop)

	attrType	
	-------------------
	The type of the attribute (e.g., Text, Number).

	attrValue
	-------------------
	The value of the attribute, denoting the status of a machine (Trimming, Cutting, Started, Finished).
