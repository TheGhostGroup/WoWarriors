# Level Scaling

### what you have to do
* Clone the Reposetory.
* Open the LEVEL SCALING.md with a text editor of your choice.
* Gether the Id´s of every npc, thats not scaled correctly.
* Add a line to the template below
* Make a pull request


### SQL template
```SQL
INSERT INTO creature_template_scaling (`Entry`, `LevelScalingMin`, `LevelScalingMax`)
VALUES
(525, 1, 60),
(50039, 1, 60)
--Copy the entry above and fill them like this ("mob id", "Intended minimal level", Intended maximal level")
ON DUPLICATE KEY UPDATE Entry=VALUES(Entry),
Entry=VALUES(Entry),
LevelScalingMin=VALUES(LevelScalingMin),
LevelScalingMax=VALUES(LevelScalingMax)
```
