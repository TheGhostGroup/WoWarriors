
INSERT INTO creature_template_scaling (`Entry`, `LevelScalingMin`, `LevelScalingMax`)
VALUES

-- Elwynn Forest --
(525, 1, 60), -- Elwynn Forest | mangy-wolf
(49874, 1, 60), -- Elwynn Forest  | Blackrock Spy
(49871, 1, 60), -- Elwynn Forest  | Blackrock Worg
(42937, 1, 60), -- Elwynn Forest  | Blackrock Invader
(42938, 1, 60), -- Elwynn Forest | Kurtok the Slayer
(50039, 1, 60) -- Elwynn Forest | Goblin Assassin
(113, 1, 60), -- Elwynn Forest | Sronetusk Boar
(330, 1, 60), -- Elwynn Forest  | Princess
(97, 5, 61), -- Elwynn Forest  | Riverpaw Runt
(478, 3, 60), -- Elwynn Forest  | Riverpaw Outrunner
(100, 10, 62), -- Elwynn Forest | Gruff Swiftbite  
(119, 9, 21), -- Elwynn Forest | Longsnout
(285, 1, 60), -- Elwynn Forest | Murloc
(735, 4, 61), -- Elwynn Forest |Murloc Streamrunner
(1922, 3, 60), -- Elwynn Forest | Gray Forest Wolf
(40, 3, 60), -- Elwynn Forest | Kobold Miner
(476, 5, 61), -- Elwynn Forest | Kobold Geomancer
(524, 3, 60), -- Elwynn Forest | Rockhide Boar
(117, 5, 60), -- Elwynn Forest | Prowler
(116, 5, 60), -- Elwynn Forest | Bandit
(822, 4, 61), -- Elwynn Forest | Young Forest Bear
(30, 3, 60), -- Elwynn Forest | Forest Spider

-- Deadwind Pass --

(51983, 55, 56, -- Deadwind Pass | Deadwind Widow

-- Blasted Lands --

(5985, 40, 60), -- Blasted Lands | Snickerfang Hyena
(5992, 40, 60), -- Blasted Lands | Ashmane Boar
(5977, 40, 60), -- Blasted Lands | Dreadmaul Mauler
(5978, 40, 60) -- Blasted Lands | Dreadmaul Warlock

ON DUPLICATE KEY UPDATE Entry=VALUES(Entry),
Entry=VALUES(Entry),
LevelScalingMin=VALUES(LevelScalingMin),
LevelScalingMax=VALUES(LevelScalingMax)

