# Resolving

## Format

Static abilites are plain statements that either prohibit something or change numbers. Both "Players can't play momentaries" and "All creatures you control have +1 health" are viable static abilities. Static abilities cannot be resolved, but passively influence the game state.

All non-static abilities are of form `costs: effects`. Costs section can include triggers such as 'start of your turn'. All of the following are viable abilities:

* Start of your turn: Draw
* Tap self: Gain 2 gold
* Start of turn, tap self, pay 1 mana: skip your turn

Abilities with both a trigger and cost actions are hybrid abilities. Hybrid abilities count as both, an activatable and a triggered ability. They can be used only as the trigger is present and are used by paying the costs. A player doesn't have to use a hybrid ability when the trigger is present.

## Effects

This file describes how effects resolve. Note, that this file doesn't concern itself on how multiple effects interact, only on how to 'run' a single card text. In short, if an action cannot be completed, it can be ignored and moved on. Each effect is completed as far as it can be.

For example, if you have 2 cards in your deck, but an effect states 'draw 3. destroy target human'. You will draw the two cards in your deck and get to destroy a human, even though the draw did not 'complete'. But if the same text was a cost, you wouldn't get to destroy target human, since the resolving stopped after drawing failed to complete.


