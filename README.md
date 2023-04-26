# Assignment 3.1

- Everything mentioned in the assignment has been implemented.
- **Bonus** :
    - King’s Leviathan Axe has also been implemented.
    - Dragon Character has been added, it can fly over walls.
    - Queen's Eagle Arrow has been added.
    - Movement avoiding walls has also been implemented.

- To run the game : `python3 game.py`
- To view replays : `python3 replay.py`  and select the replay you want to watch according to mentioned date and time.
- For Victory : All buildings apart from walls get destroyed from the map in all three levels.
- For Defeat : If all troops and King die before destroying all buildings apart from walls.

## Controls :

### Hero :

- w : move up
- a : move left
- d : move right
- s : move down
- 1 : Special Attack
- space : Normal Attack

### Barbarian :

- z : spawn at point 1
- x : spawn at point 2
- c : spawn at point 3

### Dragon :

- v : spawn at point 1
- b : spawn at point 2
- n : spawn at point 3

### Archer :

- i : spawn at point 1
- o : spawn at point 2
- p : spawn at point 3

### Balloon :

- j : spawn at point 1
- k : spawn at point 2
- l : spawn at point 3

### Stealth Archer :

- t : spawn at point 1
- y : spawn at point 2
- u : spawn at point 3

### Healer :

- m : spawn at point 1
- , : spawn at point 2
- . : spawn at point 3

q : Quit Game

## Assumptions :

- Rage and Heal Spell can be applied multiple times.
- The limit for troops in each level is as follows :
    - Barbarians : 10
    - Dragon : 7
    - Balloon : 5
    - Archer : 3
    - Healer : 4
    - Stealth Archer : 3
- You have to choose the type of troop movement at start of the game.
- You have to choose the hero after each level.
- Barbarian, Archer, StealthArcher and Hero are grounded i.e, they can't jump over walls.
- Dragon, Balloon and Healer are aerial troops i.e, they can only be attacked by the Wizard Tower and can jump over walls.
- Stealth Archer will be invisible for the first 10 seconds i.e, it will not be attacked by any cannon or wizard tower but it may take damage in its invisible state if its in range of some AOE attack.
- Level 3 Walls will explode with a radius of 2 tiles causing an AOE damage of 200 to all the grounded troops(Barbarian, Archer, StealthArcher, Hero) in its vicinity.
- Rage Spell will increase the healing power of the healer by 2 times.
- Level of each building will be the same level as that of the village.
- Health of each building w.r.t their levels:
    - TownHall : 100 + 10*level
    - Hut : 40 + 10*level
    - Cannon : 60 + 30*level
    - Wizard Tower : 60 + 30*level
    - Wall : 100 + 40*level
- Attack Power and Range of Cannon and Wizard Tower w.r.t their levels:
    - Cannon : Power => 4 + level, Range => 5 + (level//2)
    - Wizard Tower : Power => 4 + level, Range => 5 + (level//2)