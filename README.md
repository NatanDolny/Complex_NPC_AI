# Complex_NPC_AI
A tool to easily import NPCs into a bar/food stand environment. Featuring a prefab ready for quick importation into a working level. Please read 'ReadMe' for further information.

Built with Unity 2021.3.11f1



This is a developer tool meant for creating complex NPC behaviour in a pub/restaurant setting. By configuring the settings, You can change the maximum number of NPCs present, the frequency they perform their actions, and how quickly they leave the premises. They have multiple personality traits which manipulate their behaviours, for example alcohol increases confidence and confidence is for instance used to determine where an NPC will sit at a table. The tool also provides access to the environment's appearance and each object's affect on the NPCs. For ways to edit these and other important details, please see below.



There are 2 example scenes to assist you in getting familiar with the system and a simple set-up prefab, ready to import into a scene. 

Scenes are found in:	Assets/Scenes/ExampleScenes
Prefab is found in:	Assets/Prefabs/Requisites/ConfiguredSetUp.prefab



IMPORTANT
-	Before using the tool, you need to build the nav mesh map. For information on how to do this, please read: 
				  https://docs.unity3d.com/Manual/nav-BuildingNavMesh.html

The example scenes have the nav mesh map built.

If you are experiencing issues withe NPCs not moving on spawn (even after baking the nav mesh), please restart Unity after saving your progress. This is a bug caused with the nav mesh.


All objects inside the prefabs can be changed to others, however, the object tags, scripts, colliders and other components should be kept the same. 

The following object names shouldn't be changed to avoid errors (there are name checks involved):
-	NPC
-	ManPoint and WomanPoint inside the toilet prefab

Due to the chair placement method, tables should only be rotated in 90-degree intervals. This is due to how the Unity bounding boxes work as the width and length depend on the furthest x and z points. If rotated at other intervals it will create bounding boxes from the corners instead of the edges of the table.






Here are the potential customisations possible and how to perform them...

Manager:		Assets/Prefabs/Requisites/Manager
-	Max number of NPCs and frequency of spawn after prefab placement.
-	Can choose to display NPC debug table by setting 'Show Debug Chart' to true.

NPCs: 		Assets/Prefabs/Requisites/NPC
-	Appearance changed inside prefab.
-	Selection of skin tones inside prefab (add or subtract from the list).
-	Beverage collection duration changed inside prefab.
-	Consumption action duration changed inside prefab.
-	Beverage collection duration changed inside prefab.
-	Rate of consumption changed inside prefab.


Beverages:		Assets/Prefabs/Requisites/Beverages
-	Appearance changed inside representing prefabs.

Table:		Assets/Prefabs/Requisites/Tables
-	Table type (FOOD OR DRINK), can change after prefab placement.
- Table capacity, can change after prefab placement.
-	Table appearance changed inside the prefab.
-	Table chair prefab can be changed. Can change the size of the chairs too.

Chairs:		Assets/Prefabs/Requisites/Other
- Appearance changed inside prefab.

Stands:		Assets/Prefabs/Requisites/Stands
-	Appearance changed inside prefab.
-	Queue capacity and spacing inside prefab or after placement.
-	Stand type (BAR OR FOOD STAND) doesn't need to be changed as you can choose a preconfigured Bar and Food Stand.

Entrance:		Assets/Prefabs/Requisites/Entrance
-	Appearance changed inside prefab.

Toilet:		Assets/Prefabs/Requisites/Toilet
-	Appearance changed inside prefab.
-	Location of entrances (ManPoint and WomanPoint) inside prefab.

Bin:			Assets/Prefabs/Requisites/Bin
-	Appearance changed inside prefab.


There is also a platform structure available for use, found here:
Assets/Prefabs/Requisites/Structures
