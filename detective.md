Detective Game – Case Study

Goal

Design an immersive, narrative-driven mystery game where the user plays the detective. The objective was to create a simulation that felt real and interactive, avoiding simplistic yes/no mechanics while ensuring AI could maintain consistent world logic without breaking immersion.

Challenges

Creating an investigation experience that felt like genuine detective work rather than a binary guessing game.

Ensuring AI could hold consistent information throughout the game while not revealing it prematurely, only surfacing details when the user actively engaged with a character, location, or object.

Preventing AI from drifting into preexisting game formats where the plot advanced automatically, regardless of what the user uncovered.

Maintaining immersion by avoiding meta-language (no “game engine,” “dungeon master,” or “story narrator” framing).

Solutions

First iteration resembled Clue, relying on binary answers like “does this suspect have the murder weapon?” This proved quite unengaging, so the second iteration shifted toward descriptive, narrative evidence that gave players clues to interpret rather than definitive answers.

Reframed the AI’s role as a simulation engine: the world was static until the player interacted with it, at which point AI revealed only relevant details. This prevented premature plot advancement and preserved immersion.

Grounded the mystery in a reference document that contained all core story details (characters, locations, evidence). This ensured consistency while allowing the user to play without spoilers, since the document could be stored out of sight but still accessible to AI.

Built interactions around exploration, interrogation, and examination, so the player actively uncovered the truth instead of passively receiving it.


Insights

The development of this case study shows how a narrative agent can evolve from a rigid guessing game into a living mystery simulation. Early attempts, patterned after Clue, quickly highlighted the limits of binary responses, which stripped away tension. By moving to descriptive, narrative-driven evidence, the game began to mirror real detective work, where interpretation, intuition, and detail matter. The major breakthrough came when AI was instructed not to act as a narrator or game master, but as a static world simulation that only came alive through interaction. This shift not only fixed consistency issues but also unlocked a style of play where players felt like genuine detectives—immersed in a story that existed independently of them, waiting to be uncovered.

[See a short walkthrough video of the Immersive Detective Game](https://youtu.be/U45wFHBqhMg?si=68QpQxbHLZLE1GCj)

[Try the immersive detective game live as a Gem!](https://gemini.google.com/gem/ae487de5237a)
