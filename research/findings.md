# Research Findings

This document contains the factual platform research behind the product study. Interpretations and product decisions are documented separately in the Product Reasoning Log.

## Xbox Achievements and Gamerscore

### Individual achievements

Xbox games define individual Achievements with specific unlock requirements.

Achievements can award Gamerscore, and Xbox allows developers to assign different Gamerscore values to different Achievements.

For current Xbox certification requirements, a base game generally launches with 1,000 Gamerscore distributed across 10–100 Achievements. A single Achievement cannot exceed 200 Gamerscore.

Microsoft's requirements also state that Achievements should represent meaningful exploration of or engagement with game content rather than being unlockable with little or no player input.

### Lifetime aggregation

Gamerscore is cumulative across the Xbox ecosystem.

Microsoft describes it as a single common gaming score for a player. When a Gamerscore-bearing Achievement is unlocked, its value is added to that player's existing Gamerscore.

This means a player's visible Gamerscore can accumulate across many games and years of play rather than resetting for each title.

### Social comparison

Gamerscore is part of Xbox's social player data.

Players can compare Achievements with friends through profiles, while the aggregate Gamerscore provides a single value representing Achievement score accumulated across Xbox games.

### Completion

Gamerscore and completion are related but not identical.

A player can accumulate substantial Gamerscore without earning every Achievement in every game.

In 2026, Xbox began testing additional Achievement presentation features, including highlighting games where a player has earned all available Gamerscore.

Xbox also began testing the ability to hide individual games from the Achievement history displayed on a profile while keeping the Gamerscore earned from those games in the player's total.

This creates an important distinction between:

**system record:** what the player actually earned

and

**profile presentation:** which parts of that history the player chooses to display.

---

## PlayStation Trophies

### Individual trophies

PlayStation uses four trophy grades:

- Bronze
- Silver
- Gold
- Platinum

Sony describes the grades, from highest to lowest, as Platinum, Gold, Silver and Bronze.

The number of trophies, their grades and their unlock requirements vary by game.

### Platinum

Platinum occupies a distinct position in the system.

Rather than simply being another common trophy grade, it is commonly used as the capstone trophy associated with obtaining the required trophy set for a game.

This makes completion particularly legible within PlayStation's trophy system.

### Trophy rarity

PlayStation also communicates how commonly an individual trophy has been earned.

Sony currently uses four rarity categories:

- Ultra Rare
- Very Rare
- Rare
- Common

Rarity is determined by how many players have earned the same trophy.

This means rarity remains attached to the individual accomplishment rather than becoming a universal player-level mastery score.

### Trophy Level

PlayStation also has a cumulative Trophy Level.

In 2020, Sony redesigned Trophy Level from the previous 1–100 scale to a 1–999 scale.

Sony stated that the revised calculation:

- allows faster progression through earlier levels
- produces more consistent level progression
- gives Platinum trophies greater weight toward level progression

A player's exact level depends on the number and grades of trophies they have earned.

Previously earned trophies continue contributing to the player's Trophy Level.

### Social visibility and comparison

Earned trophies can appear on a player's PlayStation profile, subject to privacy settings.

On PS5, another player can navigate to a profile, select Trophies from the Overview tab, and inspect trophies by game.

PlayStation also supports direct trophy comparison between players.

### Trophy tracking vs. profile curation

PS5 allows players to pin up to five trophies per game.

However, this feature is designed for tracking progress toward trophies during play.

It is not the same as selecting accomplishments to feature publicly as part of a persistent player profile.

---

## What the two systems have in common

The initial assumption behind this study was that Xbox and PlayStation used fundamentally different accomplishment systems.

Research showed considerably more overlap.

Both systems support:

- individual game accomplishments
- different values or grades for accomplishments
- accumulation across games
- lifetime progression
- social visibility
- player comparison
- game-level completion information

The meaningful product differences therefore cannot be explained simply as:

> Xbox has lifetime progression while PlayStation does not.

Both do.

The systems package and present that information differently.

---

## What the metrics can establish

### Gamerscore

Gamerscore reliably establishes the amount of Gamerscore a player has accumulated through Xbox Achievements.

It does not independently establish:

- player skill
- game difficulty
- perfect completion
- time played
- why an Achievement mattered to the player

### Trophy Level

Trophy Level reliably establishes accumulated weighted trophy progression under PlayStation's leveling system.

It does not independently establish:

- player skill
- game difficulty
- time played
- mastery of particular mechanics
- which accomplishments matter most to the player

### Platinum count

Platinum trophies provide a particularly legible completion signal.

They still do not independently describe every meaningful accomplishment within the underlying play history.

A player can complete difficult optional content without earning a Platinum, while another player may earn a Platinum through a different combination of behaviors.

This distinction between **what a metric measures** and **what another player infers from it** became central to the product study.

---

## Profile representation precedent

### Steam

Steam provides a useful precedent for separating verified platform data from player-controlled presentation.

Steam profiles support customizable showcases.

Steam documentation explicitly identifies achievements as one of the types of content that can be displayed through profile showcases.

Steam also supports achievement-oriented profile surfaces including Achievement, Completionist and rare-achievement showcases.

The underlying Achievement history remains platform data, while the profile gives players greater control over what becomes prominent.

### Xbox

Xbox's 2026 Achievement changes provide another relevant precedent.

Players testing the feature can hide games from the Achievement history displayed on their profile without removing the Gamerscore those games contributed.

The underlying record and the public presentation therefore remain separate.

This does not provide the same functionality as the Featured Accomplishments concept proposed in this study.

It does demonstrate a current platform direction toward greater player control over how verified accomplishment history appears publicly.

---

## Key findings that informed the product decision

### 1. Xbox and PlayStation are more mechanically similar than the starting observation suggested

Both have individual accomplishments and lifetime aggregation.

The research therefore moved away from trying to explain the preference through mechanics alone.

### 2. Completion and accumulated accomplishment are different signals

Gamerscore can continue accumulating without perfect game completion.

PlayStation provides both cumulative Trophy Level and a highly legible Platinum completion signal.

Neither representation captures every dimension of player accomplishment.

### 3. Rarity can provide evidence without requiring a universal mastery score

PlayStation already associates rarity with individual trophies.

This allows an accomplishment to carry additional context without claiming that the player's entire gaming identity can be represented by a mastery number.

### 4. Platforms already separate system truth from presentation

Steam profile showcases allow verified platform information to become part of player-controlled profile presentation.

Xbox's 2026 Achievement changes similarly allow players to alter which games appear publicly without changing their underlying Gamerscore.

This suggested a smaller intervention than redesigning PlayStation's existing Trophy system.

### 5. The platform does not need to decide what a player's most meaningful accomplishment is

The platform can verify what happened.

The player can decide which verified accomplishments they want to emphasize.

That distinction became the foundation for the Featured Accomplishments concept.

---

# Sources

## PlayStation

**PlayStation Support: How to earn trophies on PlayStation consoles**  
https://www.playstation.com/en-us/support/games/how-to-earn-trophies-on-playstation--consoles/

Used for:
- trophy grades
- trophy rarity
- profile visibility
- trophy comparison
- pinned trophy behavior

**PlayStation Blog: Upcoming Trophy levelling changes detailed**  
https://blog.playstation.com/2020/10/07/upcoming-trophy-levelling-changes-detailed/

Used for:
- Trophy Level redesign
- 1–999 scale
- Trophy Level calculation principles
- increased Platinum weighting

## Xbox / Microsoft

**Microsoft Learn: Configure Xbox achievement rewards**  
https://learn.microsoft.com/en-us/gaming/gdk/docs/services/player-data/achievements/title-managed/concepts/live-achievement-rewards

Used for:
- Gamerscore as an Achievement reward
- single cumulative Gamerscore across Xbox
- Achievement reward behavior

**Microsoft Learn: Xbox Achievements and Gamerscore requirements**  
https://learn.microsoft.com/en-us/gaming/gdk/docs/store/policies/pc/live-policy-tests-pc

Used for:
- base-game Gamerscore requirements
- Achievement count/value constraints
- requirement that Achievements represent engagement with game content

**Microsoft Learn: Overview of Social features**  
https://learn.microsoft.com/en-us/gaming/gdk/docs/services/community/live-social-overview

Used for:
- Gamerscore as accumulated Achievement score
- profile/social comparison behavior

**Xbox Wire: New Improvements to Achievements, April 2026**  
https://news.xbox.com/en-us/2026/04/08/xbox-insiders-may-2026-console-features/

Used for:
- hiding games from profile Achievement history
- retaining hidden games' Gamerscore
- highlighting 100% completed games

## Steam

**Steam Support: Steam Levels and XP**  
https://help.steampowered.com/en/faqs/view/1F74-BE45-3AAC-1B47

Used for:
- profile Showcase functionality
- achievements as supported Showcase content

**Steam Support: Steam Private Games**  
https://help.steampowered.com/en/faqs/view/1150-C06F-4D62-4966

Used for:
- relationship between game privacy and Achievement/profile showcases
- evidence that Achievement information can participate in configurable profile presentation

---

*Platform behavior was researched in September 2026. Platform features may change over time.*