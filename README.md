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
