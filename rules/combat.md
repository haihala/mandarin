# Combat

Implicit abilities for attacking and blocking can be found `implicit.md`

## Process structure

1. A player uses the implicit ability of creatures and attacks an another player.
2. Defending player receives a trigger for being attacked and may use the hybrid ability to block.
3. Fights happen for each defender that is defending in the order the abilities went onto the stack.
4. If a blocker was present and attacker doesn't have trample, remove the attack ability from the stack. If no blocker was present or the attacker has remaining damage and trample, the remaining total damage is dealt to the receiving player.

## Fight structure

When a fight happens, both creatures deal their damage to one another. If a creature does multiple attacks, every Nth attack happens at the same time. Creatures' damage value can be a single integer. This means that the creature attacks once with the given amount of damage. Cards may also have a series of comma separated numbers. This is to denote how much damage is done in each step. Patterns can repeat. Paranthesis must be used when this is done. Second example shows how.


Cards cannot be played nor abilities can be activated during a fight.

Example fight:

Two creatures, one(A) does 20x1 damage, the other(B) does 2x3 damage. A has 7 health and B has 9 health. 

First, both creatures hit each other for the first time. A deals 1 damage to B, leaving B at 8 health. At the same time B deals 3 damage to A, leaving A at 4 health.
Since both parties are still alive, second round of damage happens. A deals 1 damage to B, leaving them at 7 health. B deals 3 damage, A is at 1.
Both alive, but B is out of attacks, so only A will attack now. A deals 1 damage, B is at 6.
B is still out of attacks, A deals 1, B at 5.
B at 4
B at 3
B at 2
B at 1
B at 0, dead.
Fight is over. Even though A still has 13 attacks left, they won't happen. A survived the fight with 1 health, B died.

Since A was attacking, if there is another blocker, A will start the fight with the second blocker with 13 attacks left.

Another example:

This time A is a creature with damage value of "5x(0, 2x9, 0)" and a health of 21. B is a creature with damage value of "10x2" and a health of 19.

|Round|A's damage|A's health(before damage)|B's damage|B's health(before damage)|
|:---:|---|---|---|---|
| 0|0|21|2|19|
| 1|9|19|2|19|
| 2|9|17|2|10|
| 3|0|15|2| 1|
| 4|0|13|2| 1|
| 5|9|11|2| 1|
| 6|9| 9|2| 0|
| 7|0| 7|2| 0|
| 8|0| 5|2| 0|
| 9|9| 3|2| 0|
|10|9| 1|0| 0|
|11|0| 1|0| 0|

This fight would end on round 6 as B dies, but as you can see, even if B couldn't die, A would never lose since B runs out of damage.
