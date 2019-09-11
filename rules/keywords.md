# Keywords

This file describes various keywords the game uses to function.

## Move S Z

Remove cards matching selector S from their current zone and add them to Z.

## Draw

Same as 'draw 1'.

## Draw N

Take N cards from the top of your deck and move them to your hand. 
They all move simultaniously and effects have to explicitly state if they wish to trigger for each card drawn.

## Destroy S

Move target card to the graveyard

## Obliterate S

Move target card to the obliterate zone.

## Recycle S

Move target card to the bottom of it's owner's deck.

## Flip S

Turn a card face-down. Face down cards are still cards, but don't have a type, text or costs.

## Tap S

Turn a card sideways. This card is now 'tapped out' and cannot be tapped again until untapped. A tapped permanent is an illegal target for abilities that tap the permanent.

## Untap S

Turn a tapped card straight. It can now tap again.

## Crew N

Select a set of creatures so that their combined 

## Attach T1 to a T2

Place T2 with all its previous attachments on top of T1. T1 is now an attachment of T2. Text in T1 that refers to host now refers to T2 for as long as neither is destroyed nor T1 is attached elsewhere. Text on T2 that refers to attachments now refers to T1.

## Pay (M|N gold)

Owner loses either M mana or N gold, depending on the effect.

## Gain (M|N gold)

Opposite of `pay`. Owner gets either M mana or N gold.

## Attack P with T

More on this in `combat.md`. T deals it's total damage to P.

## Fight T1 T2

More on this in `combat.md`. T1 deals combat damage to T2 and vice versa until one of them dies or both run out of damage.
