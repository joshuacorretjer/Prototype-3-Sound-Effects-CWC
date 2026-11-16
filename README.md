# Prototype 3 – Sound & Effects

## Overview

A Unity 3D endless side-scrolling runner game developed as part of the **Create with Code Live – Spring 2020** course. The objective is to jump over incoming obstacles to avoid collisions and keep the player running.

The project focuses on enhancing gameplay through physics-based player movement, animation, audio, particle effects, and dynamically repeating backgrounds. It also introduces script communication and state management to coordinate gameplay behavior, particularly when the game ends.

## Features

- **Player Jumping:** Implemented physics-based jumping using Rigidbody forces and configurable gravity.
- **Jump Restrictions:** Added ground detection and boolean flags to prevent double jumping and unlimited jumps while airborne.
- **Endless Background:** Created a continuously scrolling background that resets its position to simulate an endless running environment.
- **Obstacle System:** Implemented obstacle movement and coordinated spawning throughout gameplay.
- **Collision Detection:** Used tags and collision detection to identify obstacle interactions and trigger the game-over state.
- **Animation System:** Integrated character animations using Unity Animator Controllers, animation triggers, and boolean parameters.
- **Particle Effects:** Added particle effects that synchronize with character animations and gameplay events.
- **Audio Integration:** Implemented background music and sound effects for jumping and collision events.
- **Game State Management:** Used script communication and boolean flags to stop background movement, obstacle movement, and spawning when the game ends.

## What I Learned & Implemented

### Player Movement and Physics
- Used `GetComponent()` to access and manipulate GameObject components through scripts.
- Implemented player jumping using Rigidbody's `AddForce()` method.
- Applied `ForceMode.Impulse` to create an instantaneous force for jumping.
- Modified global gravity using `Physics.gravity` and configured gravity and jump force variables to achieve suitable jumping behavior.
- Used boolean variables and conditional statements, including the logical AND (`&&`) operator, to control gameplay conditions.
- Implemented jump restrictions using a boolean flag to prevent additional jumps while the player is airborne.
- Configured Rigidbody constraints to restrict movement along specific axes and prevent the player model from falling over.

### Endless Environment and Gameplay Management
- Created a continuously scrolling background using a movement script and a Box Collider to determine when the background should reset its position.
- Used Unity tags to identify GameObjects and determine how collision events should be handled.
- Implemented script communication to access variables and methods from other scripts.
- Used boolean flags to track the game-over state and coordinate the behavior of multiple gameplay systems.
- Stopped background movement, obstacle movement, and obstacle spawning when the game-over condition was triggered.

### Animation and Particle Effects
- Explored Unity's Animator Controller and implemented basic animation state management.
- Configured a default animation and triggered other animations using `Animator.SetTrigger()`.
- Used `Animator.SetBool()` to maintain the character's game-over animation state.
- Adjusted animation playback speed to better match the character's movements and gameplay.
- Attached particle effects as child GameObjects to coordinate their positions with the character.
- Controlled particle systems through scripts, playing and stopping effects to synchronize them with character animation states.

### Audio Integration
- Worked with Unity Audio Sources and Audio Listeners to implement background music.
- Added sound effects triggered by player actions, including jumping.
- Integrated explosion sound effects with particle effects when the player collided with an obstacle.

## Technologies & Tools

- **Game Engine:** Unity
- **Programming Language:** C#
- **IDE:** Visual Studio
- **Concepts:** Rigidbody Physics, ForceMode, Player Jumping, Physics.gravity, Endless Backgrounds, Collision Detection, Tags, Script Communication, Animator Controllers, Particle Systems, Audio Sources, Audio Listeners, Game State Management

## Course

**Create with Code Live – Spring 2020**

A remote Unity course taught by professionals working at Unity, focused on learning game development and programming through hands-on projects.
