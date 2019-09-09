# Stack

You can play a card or use an ability if:

* You can pay for the cost
* Your effect is fast enough
* You have priority

## What is fast enough?

Some cards have the 'fast' type. These cards can be played as a reaction to other cards. Some cards have the subtype 'breakneck', which is an even faster card.

Here is a table of what can react to what:

|What is on top|Can I use a basic effect|Can I use a fast effect|Can I use a breakneck effect|
|---|:---:|:---:|:---:|
|nothing|yes|yes|yes|
|basic|no|yes|yes|
|fast|no|yes|yes|
|breakneck|no|no|yes|

So basically, a card can always be played as a reaction to a slower card and non-basic cards can react to cards with the same speed.

Some activatable abilities are also fast. This is shown individually in the ability, but the default is that they are basic speed.

## Putting an effect on the stack

If legal, one can put an effect on the stack by doing the required costs. Costs are paid before the ability is on the stack.

## Priority and resolving stacks

Basically, priority is the 'permission to act'. Exactly one player has priority at a time.

When something is put on the stack, start or restart the following algorithm: 

1. Priority is passed from the player who put whatever just went on the stack there. 
2. All players get to have priority. (even the instigator)
3. The top effect resolves. If there are no more effects on the stack, turn owner gains priority and stack resolving exits.
4. Priority passes until the player whose effect is on top of the stack passes.
5. Go to step 3.

To clarify, the player who put something on the stack cannot act immediately afterwards, but gains priority before their effect resolves. 

## Important distinctions from mtg stack

### No priority on triggers

If something happens, you cannot arbitrarily react to it. Example of two players, A and B A is taking their turn and draws a card. B cannot use their cards at this moment since they don't have priority. Priority is only passed when there is a change on the stack. That being either adding or resolving a card.

As a follow up on the previous, the infamous "In your end step" -plays are impossible.

Triggered(and by extention, hybrid) abilities however still trigger when their condition is met. So if you have something that triggers at the end of each turn, you can react to your own effect with a fast ability.

### Turn owner doesn't get priority when something resolves

In mtg, whenever a card resolves the active player gets priority. Here priority doesn't really 'reset', but spins around the table continuously.

### No complete priority laps on resolution

When a card resolves, only players until the owner of the new top card can react. The other players had a window to react before. This makes it so you only have one chance to interact with each effect.


