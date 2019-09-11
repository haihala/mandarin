# Implicit

This file describes the implicit actions players and cards have.

## Player

### Buying cards

Players can spend money to buy cards. Cards bought are usually put to the top of the buyer's deck.

### Playing cards

Players may play cards by paying their mana costs and any additional costs the card has. After that the card goes to the top of the stack. More on the stack in `stack.md` and `terms.md` stack zone part.

### Obliterate cards

Players can choose to simply annihilate any cards they are holding in their hands. This serves a two-fold purpose. The first one is to compensate the tendency of 'the discard color' being quite strong in deckbuilders, since your starting deck is purposefully bad and thus getting rid of it makes the rest of your deck better. The second purpose is as a method of handling misplay. When a card is illegally revealed from hand, the revealing player has two options. Pay the costs of the card and take it back into their hand (works when the problem was targeting) or they may obliterate the card. A method of punishing misplay is needed, since it will make nobody seem like the asshole when demanding others to play according to the rules.

### Pass priority and their turn

If a player has priority, they can choose to simply to not act and pass the priority to the next player.
If it's their turn and the stack is empty, they may freely choose to end their turn

## Creatures

### Attacking

All creatures have an implicit activatable ability 'attack':

tap self: attack target player with self

### Defending

All creatures have an implicit hybrid ability 'block':

if a creature owner doesn't control is attacking, tap self: X is target attack ability on stack. counter X, fight source of X.

### Untapping

All creatures have an implicit triggered ability:

"start of your turn: untap self" 

Please note that only creatures have this ability. A post must be crewed to untap.

## Post crewing

Posts have an implicit activated ability:

tap any number of creatures with a sum of total damage and health equal to or more than self's crew amount: untap self


