# Terms

This file describes terminology that comes with the game. Similar to `keywords.md`, but for concepts.

## Arguments

Keywords and targeting abilities have the following keyword syntax:

T is a text string such as a card type.
N is a number such as an amount of something.
L is a limiter, for example in "Target human creature", the 'human creature' bit is the limiter.
S is a selector, for example "Destroy target human creature", "target human creature" is the target, where "human creature" is the limiter of the target and "target" is the method. 
Z is a zone for example the graveyard.
M is an amount of mana.
X doesnt specify kind and is a tool to link abilities so that they share a value.

S can be further specified with:

* <numbers> to specify how many. Number is always a prefix. Suffix numbers are there to separate similar targets.
* c for creature
* p for permanent
* m for momentary
* a for attachment

If type is not specified, card is assumed. If amount isn't specified it is assumed that any amount works.

## Play order

A way to sort players. The first player is the one whose turn it is and after that players go in the order the table rotates in.

## Offset play order

Same as play order, but current player is moved last.

## Turn owner

The player whose turn it is. Priority is not a turn.

## Total damage

Total damage is the amount of damage a creature would do given infinite turns.

## Ability

Activatable ability is an ability that has costs that can be paid. If they are, the ability is put onto the stack.

Triggered ability is an ability that has a condition such as 'start of your turn' and when that trigger is hit, the ability automatically goes onto the stack.

An ability can be both a triggered and an activatable ability by having both a trigger that needs to be hit and a cost that needs to be paid. These abilities count as both an activated and a triggered ability and are put onto the stack only if both the activation cost is paid and the trigger is present.

## Zone

In short, a zone is a gameplay area where cards can exist. All existing zone types are listed below. Amount of cards in a zone is public information, but the cards themselves are often not.

Shorthands:

* Ordered
	* Order of cards in this zone matters.
* Unordered
	* Not ordered
* Public
	* Specific cards in a zone are public information. For example the board.
* Hidden
	* Not public

### Deck

Ordered hidden zone.
Zone you use to store cards. Provides a random element to the game. Cards you aquire go to the top, sometimes cards go to the bottom.
All access to the deck is relative to either the top or the bottom. A card can be placed in the deck Nth from the top, but not 'in the middle'

### Hand

Unordered hidden zone.
Zone you use to store cards you can play. A source of hidden information and psychology.

### Board

Unordered public zone.
Zone you use to store 'active' cards you control

### Market

Ordered public zone.

### Graveyard

Unordered public zone.
All cards that get destroyed or in the case of momentaries, used go to the common public grave.

### Obliterate

Unordered public zone.
Cards moved to this zone are gone. They cannot be accessed and their abilities cannot be used. There is nothing that can ever bring them back. The zone is personal for sorting purposes.

### Stash

Stashes can be ordered or unordered, public or hidden.
The stash isn't a singular zone, but a collection of zones that are mostly used to temporarily remove things from play.

## Turn

'Turn' within ability text refers to a single player's turn. So in a four player game, something that can be used once per turn can be used once on your turns and three times between your turns.
