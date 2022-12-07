# Nirvana

Nirvana is a 3D pseudo-realistic game
about escaping a confusing space of afterlife
by solving puzzles and finding memory pieces.

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
Thank you Cherry Kwong, Dong Sun, Sarah Xu!
