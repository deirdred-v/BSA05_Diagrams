# Modelings and diagrams

Summary:
Introduction to the concept of requirements modeling, basic models and representations. Building a data flow diagram, a swimlane diagram, a state diagram, and how to use decision tables.

## Contents

1. [Chapter I](#chapter-i) \
   1.1. [Task 1. Haircut Appointement](#41) \
   1.2. [Task 2. Delivery of Orders](#42)
2. [Chapter II](#chapter-ii) \
   2.1. [Exercise 00 — Building DFD, Level 0](#51) \
   2.2. [Exercise 01 — Building a Swimlane Diagram](#52) \
   2.3. [Exercise 02 — Extending the Swimlane Diagram](#53) \
   2.4. [Exercise 03 — State Diagram](#54) \
   2.5. [Exercise 04 — State Table](#55)

## Chapter I <div id="chapter-i"></div>

### Description of tasks

### Task 1. Haircut Appointment <div id="41"></div>

The management of a chain of barbershops decided to implement an online booking system. The main objective is to develop the business by expanding the customer base through the possibility of online registration, as well as to reduce employee labour costs and manual labour by automatically informing customers through communication channels. 

Both registered and unregistered visitors can book an appointment on the website. When making an appointment, they can select the type of service: hairdressing or cosmetology, as well as the service itself, the master and the time from the available intervals. The system should provide automatic sending of reminders to clients through the communication channel chosen by the client (Telegram, WhatsApp, VK, SMS) according to the schedule set by the manager. After receiving a service, the system offers the client to evaluate the service and write suggestions on how to improve the work.

The schedule of masters and the services provided by each master should be entered by the manager, who may be more than one person. This person is also responsible for keeping the schedule up to date and adjusting it if necessary, communicating with customers manually, marking the service, charging and accepting payment, sending the payment data to the accounting department. The manager can also receive reports on completed services and view customer feedback.

Each master has the ability to view the schedule and appointments for their services, as well as customer reviews.

### Task 2. Delivery of Orders <div id="42"></div>

During the lockdown, many grocery stores and food companies dramatically increased their online sales and the need for quick delivery of small quantities to individual customers increased. 

A group of students got together and decided to create a delivery service startup. The idea is to quickly receive information about orders, pickup location and time, delivery location, desired delivery dates, and distribute this information to couriers who will pick up the order at the pickup location and deliver it to the delivery location. They decided to develop an online system where orders could be collected and quickly sorted for delivery by couriers.

The first step was to collect orders from stores and caterers in any way possible and have the operator enter them into the system in a consistent format, as well as developing a mobile application for the courier. The courier should be able to view order information, select an order from those available, book it, pick it up at the collection point and deliver it to the customer. The result of the courier's actions should be immediately reflected in the system via a mobile application. The system should also include a dispatcher who controls the couriers and reassigns orders if necessary. Information on received orders should be sent to the accounting department (to another IT system) to calculate delivery charges with order suppliers. Order delivery information should also be sent to the accounting department to calculate payment to couriers. Accrued payment should be transferred to the system and displayed in the courier's personal account. And there should also be an administrator's workstation, where couriers are registered and access rights are assigned to all of them.

## Chapter II <div id="chapter-ii"></div>

### Exercise 00 — Building DFD, Level 0 <div id="51"></div>

**For each task:**
Build a Level 0 Data flow diagram:

1. Specify the purpose of the diagram.
2. Specify the area of consideration: As-Is or To-Be.
3. Show the external entities that interact with the system in the rectangles on the diagram.
4. Show the processes (stakeholder actions on the data) in ovals.
5. Show the content of the information flows on the arrows.
6. Show the data stores and the content of the information stored in the system in parallel line segments.
7. Follow the rules:
   1. All processes (ovals) must be numbered. On a level 0 diagram — in whole numbers.
   2. The processes are named: verb+object.
   3. Comprehensible domain names (not technical names of system database entities) are used to identify the object.
   4. Processes do not interact with each other directly, but through data stores.
   5. Data flows between stores and external entities or between each other through a process (not directly).
   6. The diagram does not show the sequence of processes and actions.
   7. The diagram must be readable.
8. Indicate your answers in the turn-in file ex00\_<product prefix>\_dfd.xxx (xxx is an extension).

### Exercise 01 — Building a Swimlane Diagram <div id="52"></div>

**For each task:**

Build a swimlane diagram:

1. Specify the purpose of the diagram.
2. Specify the area of consideration: As-Is or To-Be.
3. Select roles for the diagram: stakeholders, divisions, external systems. 
4. Show the lanes for the roles in the diagram.
5. Show the process steps as rectangles.
6. Show the process steps performed by the role on the corresponding track.
7. Show transitions between process steps with arrows.
8. Show the solutions in rhombuses.
9. Show the solutions on the arrows coming out of the rhombus.
10. Show the beginning and end of the process with a start/finish circle.
11. Indicate your answers in the turn-in file ex01\_<product prefix>\_swd.xxx (xxx is an extension).

### Exercise 02 — Extending the Swimlane Diagram <div id="53"></div>

**For each task** add the created artifacts to the swimlane diagram:

1. Copy the swimlane diagram, change the name.
2. Specify the purpose of the diagram.
3. Specify the area of consideration: As-Is or To-Be.
4. Add to each role in the swimlane diagram the artifacts it creates: documents, developed code, logged bugs, queries, etc.
   1. Show artifacts for each role on the lane that are developed or adjusted by the role representatives, show it on the role lane;
   2. Specify with a dotted line for each artifact the relationship to the source where the artifact is created/corrected;
   3. It is acceptable to group artifacts, i.e., to specify multiple artifacts in the same pool if they are created by the same role in the same process (or when performing the same action).
5. Indicate your answers in the turn-in file ex02\_<product prefix>\_adswd.(xxx is an extension).

### Exercise 03 — State Diagram <div id="54"></div>

**For each task:**

1. Select an object (domain entity) that has a life cycle. In task 1 — excluding the object Service request.
2. Specify the purpose of the diagram.
3. Specify the area of consideration: As-Is or To-Be.
4. Build a state diagram of the selected object:
   1. Select the names of the object states;
   2. Indicate each state of the object in the diagram;
   3. Connect the previous and next object states with arrows;
   4. Indicate the event (action) next to the arrow that transforms the object from one state to another;
   5. Specify the initiator of each event (action);
   6. Specify conditions if there are branches;
   7. Specify the beginning and end of the object life cycle.
5. Indicate your answers in the turn-in file ex03\_<product prefix>\_dst.xxx (xxx is an extension).

### Exercise 04 — State table <div id="55"></div>

**For each task** build a table of object states:

1. Select objects (domain entities) that have a life cycle.

For an object for which no complete state diagram of the object has been built:

1. Specify the object.
2. Specify the purpose of the diagram.
3. Specify the area of consideration: As-Is or To-Be.
4. Build a state table:
   1. Select names of object states.
   2. Specify in the table row:
      1. previous and subsequent states of the object;
      2. an event (action) that transforms an object from a previous state to a subsequent state;
      3. the initiator of each event (action);
      4. conditions, if there are branches.
   3. Specify the beginning and end of the object life cycle.
5. Indicate your answers in the turn-in file ex04\_<product prefix>\_tst.xxx (xxx is an extension).
