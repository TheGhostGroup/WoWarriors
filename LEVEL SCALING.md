# Level Scaling

### What will you get?
Every contributer will get an Ingame reward, but i do not know what, will think about that later

### what you have to do
* Clone the Reposetory.
* Open the LEVEL SCALING.md with a text editor of your choice.
* Gether the Id´s of every npc, thats not scaled correctly.
* Add a line to the template below
  * Pull request without the zone and mob name will not be merged
* Make a pull request


### SQL template
```SQL
INSERT INTO creature_template_scaling (`Entry`, `LevelScalingMin`, `LevelScalingMax`)
VALUES
(525, 1, 60), -- Elwynn Forest | mangy-wolf
(50039, 1, 60) -- Elwynn Forest | Goblin Assassin
--Copy the entry above and fill them like this ("mob id", "Intended minimal level", Intended maximal level") And make a comment which zone and which mob
ON DUPLICATE KEY UPDATE Entry=VALUES(Entry),
Entry=VALUES(Entry),
LevelScalingMin=VALUES(LevelScalingMin),
LevelScalingMax=VALUES(LevelScalingMax)
```
### How to Make a Pull request
the simplest way is to:

Find a project you want to contribute to
Fork it
Clone it to your local system
Make a new branch
Make your changes
Push it back to your repo
Click the Compare & pull request button
Click Create pull request to open a new pull request
