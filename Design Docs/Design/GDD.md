# MawBound

## 1. Game Overview

**Genre:** Action / Exploration / Survival
**Perspective:** 2D Side-View / Side-Scrolling with Free Vertical Movement
**Engine:** Godot

### Core Concept

The player starts as a **baby Livyatan**, an enormous underwater creature larger than a Blue Whale.

However, the player is cursed:

> **You become what you eat.**

Eating another creature transforms the player into that creature. The player must adapt to each new form, use its abilities, explore areas that their current size allows them to access, and eventually find and defeat the Shaman responsible for the curse.

---

## 2. Core Gameplay

The main gameplay loop is:

**Explore → Hunt → Fight → Eat → Transform → Adapt → Explore**

The player must:

* Swim through an interconnected underwater world.
* Manage hunger and energy.
* Hunt or fight other creatures.
* Eat creatures to survive.
* Transform into whatever creature they eat.
* Adapt to the new creature's size, stats, movement and attack.
* Use different creature forms to reach new areas.
* Find a way into the Shaman's hideout.
* Defeat the Shaman.
* Escape before transforming back into a creature too large to leave the hideout.

---

## 3. Core Design Pillars

### Transformation

Eating is more than a way to deal damage.

**Eating a creature changes the player's entire form.**

The new form changes the player's abilities, size, stats and attack.

### Adaptation

Every transformation creates a new gameplay situation.

The player must learn how the current creature behaves and decide what to hunt or avoid next.

### Size Matters

Creature size affects both combat and exploration.

* Large creatures can overpower smaller creatures.
* Smaller creatures can access areas that larger creatures cannot.
* **Only Tiny creatures can enter the Shaman's hideout.**

### Risk vs Reward

The player can choose different approaches:

* Play safely and prioritize survival.
* Take risks by fighting stronger creatures.
* Move quickly between forms.
* Hunt opportunities when they appear.

The game should allow these approaches to emerge through gameplay rather than forcing one strategy.

---

## 4. Game Progression

### Beginning — Deep Trench

The player begins as a baby Livyatan deep underwater.

The creature is too large to enter the surrounding cave structures, so the initial route is upward toward the surface.

Hunger introduces the need to keep moving and eventually teaches the player to use boost.

### Surface — Whale Territory

The player encounters two Blue Whales.

The first whale teaches hunting and combat.

After eating it:

**Baby Livyatan → Blue Whale**

The second whale then attacks the player, teaching combat using the newly acquired form.

### Open Ocean

The player explores a larger interconnected underwater world.

Different creature sizes, enemies and areas introduce new challenges.

### Smaller Creature Areas

The player eventually needs to transform into smaller creatures to access areas that larger forms cannot reach.

Different creature forms provide different combat and movement possibilities.

### Tiny Creature Access

Tiny creatures can enter narrow cave structures inaccessible to larger creatures.

The player must eventually obtain a Tiny form to enter the Shaman's hideout.

### Shaman Hideout

The Shaman is responsible for the curse.

Only Tiny creatures can enter the hideout, creating a size-based progression requirement.

The player can use different Tiny creature forms to approach the fight in different ways.

### Ending — Escape

After defeating the Shaman, the curse is released.

The player begins returning toward their original huge form.

An escape timer begins.

The player must escape the Shaman's hideout and return toward the original trench before becoming too large to fit through the cave.

If the player becomes too large before escaping, they become trapped and the run ends.

A checkpoint is placed after defeating the Shaman so the escape sequence can be retried without repeating the entire game.

---

## 5. Checkpoints

The game will contain **multiple checkpoints throughout the world**.

If the player dies, they can continue from a previous checkpoint instead of restarting the entire game.

Exact checkpoint locations will be decided during level design and playtesting.

---

## 6. Win / Lose Conditions

### Win

* Find the Shaman.
* Defeat the Shaman.
* Escape the hideout.
* Return to the original trench/home.

### Lose

* Player HP reaches zero.
* Hunger reaches its critical state.
* Player fails the final escape sequence and becomes trapped.

---

## 7. Must Have

* 2D underwater side-view movement
* Free vertical swimming
* Swimming boost
* Energy system
* Hunger system
* Creature hunting
* Combat
* Eating creatures
* Transformation system
* Multiple creature forms
* Different creature sizes
* Size-based exploration
* Interconnected underwater map
* Multiple checkpoints
* Shaman encounter
* Shaman defeat
* Final escape sequence
* Basic ending

---

## 8. If Time Allows

* Mythical creature encounter
* Anti-curse / Tiny creature eggs
* More creature forms
* More environmental interactions
* More complex Shaman encounter
* Additional transformation effects
* More detailed ending sequence
* Additional areas and exploration routes

---

## 9. Development Philosophy

The exact numbers for health, damage, hunger, energy, speed, enemy frequency and other balancing values will not be finalized purely on paper.

The intended process is:

**Design → Build → Play → Observe → Adjust → Play Again**

Values and mechanics should be changed based on actual gameplay and playtesting.
