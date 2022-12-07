# Nirvana

Nirvana is a 3D pseudo-realistic game
about escaping a confusing space of afterlife
by solving puzzles and finding memory pieces.

## Game Trailer

[![Link to Trailer](https://img.youtube.com/vi/adYjZbpEzuc/0.jpg)](https://youtu.be/adYjZbpEzuc)

## Game Overview

Nirvana is a first-person puzzle-solving and adventure PC game.
In the game, the player acts as the protagonist - Zapot,
and the goal is to collect all memory pieces to escape the confusing afterlife space. 
The player is first trapped in the pseudo-realistic world (e.g. in a residential house),
where the player has to find the memory pieces and find the way out.
But on the way, to collect more memories,
the player also has to enter realms of buddhist reincarnation
through certain unexpected portals in the pseudo-realistic world.
When the player enters any of the realms,
the player will have to survive and run to the end of the realm,
in order to successfully collect a memory at the end of the realm.
A series of puzzles is also involved in entering the realms
and finding the way out in the afterlife space.

Inside the pseudo-realistic world in the afterlife space,
it requires the player to explore and pay attention to details in the environment for puzzle solving,
while having the immersive experience of a dream-like disorienting directional space
(such as rotated rooms, objects against gravity).
The puzzle solving could be as complex as finding several clues to unlock one door
or solving one puzzle to enter another puzzle.
Inside the realms,
it also requires the player to run on a mis-angled path as fast as possible
while jumping, getting dizzy, and trying to balance across narrow winding roads.
The paths in the realms will provide more difficulty
by having monsters of the realm attacking the player
and road types that hinders the movement of the player,
such as sluggish mud road, slippy ice road, etc.

By the end of the game,
the memories will be pieced together and become a full narrative story
that explains why the victim dies and enters the afterlife.

## Installation

This game is developed using [Unreal Engine](https://www.unrealengine.com/) 5.0.3.
Please make sure you have the correct version installed
before importing the game project.
To download Unreal Engine,
please follow the [instructions](https://www.unrealengine.com/download).
After successfully opening the project
and compiling the shaders in Unreal Engine,
you can build the project to experience our prototype.

Alternatively, you may download a PC version of our prototype in 
[Releases](https://github.com/diceyecid/Nirvana/releases/tag/v0.1.0).

## Usage

If you are not using a 16:9 display,
please do not play in full screen
as some UIs are not optimized for other aspect ratios.
You may escape out of full screen
by using `Alt + Enter` or `F11`.

The control of the game works as follows:
- `Mouse Movement` for character camera movement
- `W`, `A`, `S`, `D` for character movement
- `Space` for character jump
- `C` for switching perspectives (between 1st person and 3rd person)
- `E` for picking up prop
- `F` for interacting with object
- `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, and `Mouse Wheel` for switching focus of prop bar

## File Structure

Most of the directories under `Content` folder are art assets,
except for the following:

- `Blueprints` contains all the custom blueprints made for the game,
  including pickable props and interactable objects.
- `InventorySystem` contains everything related to our prop bar.
  It is customized for our game based on
  [this inventory system](https://www.unrealengine.com/marketplace/en-US/product/inventory-system).
- `Levels` contains all the scenes in our game.
  The scenes involved in our prototype are
  house, realm, and four different orientations of rotated room.
- `Movies` contains the game start up clip.
- `UMG` contains the custom user interfaces made for the game.

## Known Issues

Please be mindful that this project is a game prototype,
there are still some flaws and minor issues existing in the game:

- Closet in the living room
  - Interaction pop up for the chest
    inside the closet appears when closet is closed
  - Closet doors closed after returning from rotated room and realm
- Rotated room door lock upstairs
  - Character has to approach from the right side
    to be able to trigger click event on the number buttons
  - Click event is triggered by double click except for the first click
    - There is a [thread](https://forums.unrealengine.com/t/an-lmb-event-is-only-triggered-with-a-double-click/357429)
      discussing a similar issue,
      but the solution did not work for us
- Noticeable lag when transition between scenes
  - Between *House* and *Rotated Room*
  - Between *House* and *Realm*

## Acknowledgement

I sincerely appreciate the incredible amount of effort my team put in for this project.
Thank you Cherry Kwong, Dong Sun, [Sarah Xu](https://github.com/SarahWeizhen)!
