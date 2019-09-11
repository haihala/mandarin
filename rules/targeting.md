# Targeting

This document describes shorthands used in targeting.

In short, all targeting is done in two parts, the method and the limiter. The method dictates how many and the limiter defines qualities the individual selected objects must have.

## Methods

### self

Self is an exception selector method. It can't have a limiter. Self always refers to the card that the effect originates from.

Example 1: A creature has an ability that calls to "Tap self". In this case 'self' refers to the creature that has the ability.
Example 2: A creature is given an ability by an attachment. The given ability calls to "Tap self". In this case, 'self' also refers to the creature, since even though the attachment is giving the ability to the creature, it is the creature that is 'using' it.

### all

There is no choice, the effect selects all entities matching the description.

### target

Select one of the entities the limiter permits.

### up to N

Select N or fewer objects.

### at least N

Select N or more objects.

### between N1 and N2

Select N1 or more, but N2 or fewer objects.

### any number of

Freely select how many and what you target.

## Limiters

### types

Simply stating a type like "target creature" or "all humans" matches super and subtypes.

### in Z

Used to define 

### with S

Dynamic comparations. S can be pretty much anything, but an easy to understand example could be "3 or less health"
