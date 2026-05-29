# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspire board](https://docs.google.com/drawings/d/1mpULZLPGO37q1OejrTyFs27elkWl5H7usuhXWBBRUzo/edit)
1. I tend to gravitate toward positive, uplifting things—nothing too gloomy. I really enjoy simulation games; shooting and combat games are just too violent for my taste. I’m particularly fond of animal-themed and pixel art games, and fascinated by the visual appeal of expansive, open-world settings.
2. Tina We don’t really have a specific style we both like, but we both love animals.
3. We rendamly picked one of the LA, Eric, he likes shooters and multiplayer games that require teamwork, such as Overwatch. Unfortunately, I don't share his tastes at all. :(

### Activity 2
2.1. 2D platformer
2.2. Each map has an entrance and an exit, and players must defeat bosses and collect the necessary materials to complete the level.
[Break-down](https://docs.google.com/drawings/d/1yYa-e13dwjo4l-MoDIiCSl77PLDO4tB7qFhnd5R_6Y4/edit)
## W4
### Activity 1: playtest
Playtesting goal:
1. Player can move and jump smoothly.
2. After picking up items, player can get new skill.
Playtesting team: Yan Zhang, Tina Meng, Xichan Zheng, Alex Ding, Jingyi Bi
Jumping makes you take off. This is a bit tricky for people without a mouse. Can't enter the tree hollow on the left, and the jump feels a bit awkward, it's too low.
### Activity 2
Yes. Because the dialogue system uses ScriptableObjects to store data, the text and narrative flow are completely separated from the actual logic and code. A writer can simply right-click in the Project window to create new instances of the Dialogue Node assets, type the dialogue into the text fields, and connect them by dragging and dropping them into the reply option slots in the Unity Inspector. They never have to open a C# script or the Visual Scripting graph.
Practically, there is no limit. The writer can create as many Dialogue Node ScriptableObject assets as they want, limited only by the computer's hard drive storage space and memory. The code is designed to dynamically read whatever node is passed to it, so it scales infinitely without needing any logic modifications.
The Regenerate Nodes button forces Unity Visual Scripting to scan the project's C# codebase and update its internal database of visual nodes. When a programmer writes a new custom script, Visual Scripting doesn't automatically know about it. Clicking this button translates the new C# code into visual blocks so that they can be searched, dragged, and connected inside the Script Graph editor.
## W5
### Activity 1
Branching dialogue
The system will use Scriptable Objects to manage branching dialogues and will use the Dialogue Controller to track and trigger the “Tame” or “Defeat” branching logic.
Basic steps:
1.Write the logic for the Dialogue Controller and design the data structures.

2.Create the dialogue UI and link it to the dialogue text and options in the Scriptable Objects.

3.Use the Dialogue Controller to update the game and mission states based on the player's choices. 
Detailed steps:
Create a Scriptable Object to store dialogue text, NPC information, and branching options for “taming” or “defeating.”  

Add state control logic to the player script to ensure that the player's movement and jumping are locked when they enter the dialogue state.  

Implement NPC interaction prompts and key triggers: When the player approaches an NPC and a prompt appears above their head, press the “Q” key to initiate dialogue.  

Write a Dialogue Controller to read the current dialogue node and first output text via the Console’s debug logs to test the data sequence.  

Build the UI, including a dialogue box that displays the NPC and player dialogue content.  

Implement branch logic for mouse click selections, allowing the player to decide between “Tame” or “Defeat” by clicking the UI.  

Write code to update the Quest UI description based on the player’s click selection and activate the corresponding game state.

Build and test only one dialogue state transition at a time until all dialogue paths have been verified in-game.


