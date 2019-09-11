# Stack

You can play a card or use an ability if:

* You can pay for the cost
* Your effect is fast enough
* You have priority

When the stack is empty, all cards are fast enough. When the stack isn't empty, only cards and effects that are specially tagged as 'fast' are fast enough.

Costs count are being paid if you successfully complete all actions listed as costs.

## Priority and resolving stacks

Basically, priority is the 'permission to act'. Exactly one player has priority at a time.

When something is put on the stack, start or restart the following algorithm: 

1. Priority is passed from the player who put whatever just went on the stack there. 
2. All players get to have priority. (even the instigator)
3. The top effect resolves. If there are no more effects on the stack, turn owner gains priority and stack resolving exits.
4. Priority is passed until the player whose effect is on top of the stack passes.
5. Go to step 3.

To clarify:

* The player who put something on the stack cannot act immediately afterwards, but gains priority before their effect resolves.
* When an effect resolves, the controller of the effect doesn't instantly have to pass for the next thing in the stack.

## Triggers

Triggered (and hybrid) abilities are instantly put on the stack in ordered by owner in play order. If a player would have multiple abilities trigger at the same time, they can freely order the abilities however they like. For hybrid abilities costs have to be paid when the ability goes on the stack.

## Important distinctions from mtg stack

### No priority on triggers

If something happens, you cannot arbitrarily react to it. Example of two players, A and B A is taking their turn and draws a card. B cannot use their cards at this moment since they don't have priority. Priority is only passed when there is a change on the stack. That being either adding or resolving a card.

As a follow up on the previous, the infamous "In your end step" -plays are impossible.

Triggered(and by extention, hybrid) abilities however still trigger when their condition is met. So if you have something that triggers at the end of each turn, you can react to your own effect with a fast ability.

### Turn owner doesn't get priority when something resolves

In mtg, whenever a card resolves the active player gets priority. Here priority doesn't really 'reset', but spins around the table continuously.

### No complete priority laps on resolution

When a card resolves, only players until the owner of the new top card can react. The other players had a window to react before. This makes it so you only have one chance to interact with each effect.


