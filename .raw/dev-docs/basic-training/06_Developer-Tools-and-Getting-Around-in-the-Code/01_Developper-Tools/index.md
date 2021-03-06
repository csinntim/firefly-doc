﻿## Developer Tools and Getting Around in the Code


1.	In this lesson, we will open your migrated code for the first time, and see what tools we’ve got to help us getting around in the code.
2.	First, we’ll see the tools we have in a deployment machine.
3.	Later we’ll discuss the solution architecture and see how to find things easily in the code.
4.	This part will be demonstrated on the customer code !

### Developer Tools

1.	Run the application and **right click the status bar** to see the Developer Tools menu.
2.	Note that this menu is available only with **administrator** rights and only when the application was built in **debug mode**
  
#### 1. About Firefly
1.	Open the **About Firefly** window.
2.	This window replaces the About Magic and contains the version number and data of all the dlls that are used by the application.
3.	This screen is in the ENV project and **can be modified** if you wish to do so.
#### 2. Call Stack
1.	Open Programs-> Orders
2.	Open Developer Tools - > Call Stack window.
3.	This window shows the **current location** in the code in 3 different ways:
    a.	Last menu path
    b.	.NET style call stack
    c.	Application call stack (using the “Prog” function)
4.	Finally, the **version number** appears.
5.	This window is available to end users by pressing **CTRL+F12**, so that when they report issues, they can send you useful information about their location and version number.
 
#### 3. Application Call Stack

1.	Open Developer Tools - > Application Call Stack window.
2.	This window shows the Active tasks and some details about each task like the activity, transaction and locking strategies.
3.	Right click on the task will enable us to see the following:
    a.	**Columns** – current active columns and their info: value, type, entity, db name.
    b.	**DataView** – a list of the entities that are used by the program. Each entity data can be viewed by right clicking or pressing enter on the entity line.
For each entity we can see the following data:
    i.	The type (if this entity is the main (from) one or a relation.
    ii. RelationType (find, join, insert etc.), in case of a related entity.
    iii. Found- in case of a relation we want to know if a row was found, according to the relation filter.
#### 4. Browse Entity Data
1.	Open Developer Tools -> Browse entity data window.
2.	This option is equivalent to Data Sources Repository in Magic.
3.	Each table can be viewed and edited by pressing “Enter”.
4.	An SQL script for creating the table can be generated by right clicking on it.
5.	This window can be opened by **SHIFT+F2**.

#### 5. Run a Program
1.	Open Developer Tools -> Run a Program window.
2.	This window allows you to run a program directly, like F7 in Magic.
3.	Run program #4 (ShowProducts). Notice that some programs accept parameters and even have several options to call them (with or without parameters). In this case a preceding screen will be opened to allow you to choose the option you want to call the program (There is no need to write a test program).
4.	This window can be opened by SHIFT+F3.
5.	Exercise: Developer Tools
