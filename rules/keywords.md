# Keywords

This file describes various keywords the game uses to function.

## Move S Z

Remove cards matching selector S from their current zone and add them to zone Z. Can be further specified such as 'top of deck'.

## Draw a card

Same as 'draw 1'.

## Draw N

Move N cards from the top of your deck to your hand. 
They all move simultaniously and effects have to explicitly state if they wish to trigger for each card drawn.

## Destroy S

Move target card to the graveyard

## Obliterate S

Move target card to the obliterate zone.

## Recycle S

Move target card to the bottom of it's owner's deck.

## Flip Sp

Turn a card face-down. Face down cards are still cards, but don't have a type, text or costs.

## Tap Sp

Turn a card sideways. This card is now 'tapped out' and cannot be tapped again until untapped. A tapped permanent is an illegal target for abilities that tap the permanent.

## Untap Sp

Turn a tapped card straight. It can now tap again.

## Crew N

Keyword on exclusively post cards.

Tap any amount of creatures so that their combined total damage is at least N: untap self

## Attach (Se) to 1Sp

If Se isn't specified, self is assumed.

Place Sp with all its previous attachments on top of Se. Se is now an attachment of Sp. Text in Se that refers to host now refers to Sp for as long as neither is destroyed nor Se is attached elsewhere. Text on Sp that refers to attachments now refers to Se in addition to other attachments that are currently attached to Sp.

## Pay (M|N gold)

Owner loses either M mana or N gold, depending on the effect.

## Gain (M|N gold)

Opposite of `pay`. Owner gets either M mana or N gold.

## Attack P with Sc

More on this in `combat.md`. Sc deals it's total damage to P.

## Sc1 fights Sc1

More on this in `combat.md`. Sc1 deals combat damage to Sc2 and vice versa until one of them dies or both run out of damage.

## Bargain

Keyword on exclusively momentary cards.

When this card resolves, instead of going to the graveyard, move it to the bottom of it's target's deck.

## Swarm N1 N2

Keyword on exclusively creature cards.

A card with swarm has a damage value of Yx(B) where Y is amount of swarm counters on the creature and B is the damage written on the card.

before self enters the board: put N1 swarm counters on self.

end of your turn: if self didn't attack this turn, remove N2 swarm counters from self.

self takes damage: remove swarm counters from self equal to the amount of damage taken instead of taking damage.

remove X>=1 swarm counters from self: create a token copy of self with X-1 swarm counters on it.

remove all swarm counters from self: put all swarm counters removed from this to an another swarm with the same name.

## Redirect

Keyword on exclusively momentary cards or abilities.

Player or the owner of a permanent that was targeted with a redirect effect may once per ability choose a new player target for it. If the same target is chosen.

## Cultivate N 1Sc

Flip S. Put N+1Sc's mana cost cultivate counters on it.

At the start of your next turn: Destroy S. You may play a creature that costs less mana than there are cultivate counters on the destroyed card without paying it's mana cost.

## Meld Sc

Create a eldritch horror token creature named 'meld' with all the types of Sc. The token's health, damage, mana cost and gold cost are all equal to the sum of Sc's. The token gains all of Sc's abilities. Obliterate Sc
