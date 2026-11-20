# Character Controller & Hero Mechanic Prototype

A third-person character controller and combat prototype built in Unity 6.3 LTS (6000.3.10f1). Developed in a grey-boxed test gym, the project focuses on game feel, responsive movement, animation blending, and an interactive hero ability featuring projectile combat, visual effects, audio feedback, and health systems.

## Showcase

- **Milestone 1 Video:** https://drive.google.com/file/d/1lejf5UWYw5rFNi1aHRzwxmjI6V3nKUcD/view?usp=sharing
- **Milestone 1 Build:** https://github.com/shezajsyed/milestone1/releases/tag/v1.0
- **Milestone 2 Video:** https://drive.google.com/file/d/1ScnQzkU4wYgCIlq3RkmVgAzv-RyOicm3/view?usp=sharing

## Controls

| Action | Keyboard & Mouse | Gamepad |
|---|---|---|
| Move | WASD | Left Stick |
| Look | Mouse | Right Stick |
| Sprint | Left Shift | Left Stick Press |
| Jump | Space | Button South |
| Crouch (hold) | C | Button East |
| Cast Fireball | F | Right Trigger |

## Features

### Character Controller & Movement
- **Input:** Unity's New Input System with keyboard, mouse, and gamepad support.
- **Animation:** Custom Animator Controller with 2D blend trees for locomotion, including idle, walk, run, strafe, jump, and crouch states.
- **Camera:** Cinemachine camera setup with state-driven blending between standing and crouching cameras, breathing noise, and landing impulses.
- **Game Feel:** Coyote time, jump buffering, landing audio synced with camera shake, and a crouch collider that resizes with a headroom check.
- **Environment:** Grey-box gym with dedicated movement challenges for jumping, crouching, sprinting, and the hero mechanic.

### Hero Mechanic: Fireball Combat
- **Ability Configuration:** ScriptableObjects used to centralize fireball attributes, including damage, speed, lifetime, cooldown, audio, and impact VFX references.
- **Casting Animation:** Animator-triggered casting animation integrated with projectile spawning.
- **Projectile System:** Rigidbody-based projectile movement and collision detection.
- **Visual Effects:** Fireball particle effects, smoke trails, sparks, and impact explosions.
- **Audio Feedback:** Casting and impact sound effects with randomized pitch and volume for variation.
- **Combat Feedback:** Enemy damage system with health tracking and a health bar.
- **HUD:** Player health bar and fireball cooldown meter communicate player state and ability availability.

### Health & Damage Systems
- **Player Health:** ScriptableObject-based health data with event-driven UI updates.
- **Damage Zones:** Trigger-based damage system capable of applying damage at timed intervals.
- **Enemy Health:** Damage handling, health tracking, and defeat behaviour for test enemies.

## Gym Stations

- Stepping stones — jump
- Pipes — crouch
- Stairs — climb
- Floors — sprint

## Technical Implementation

| System | Implementation |
|---|---|
| Engine | Unity 6.3 LTS (6000.3.10f1) |
| Input | Unity Input System |
| Camera | Cinemachine |
| Environment | ProBuilder |
| Animation | Animator Controller & 2D Blend Trees |
| Combat Architecture | ScriptableObjects & C# scripts |
| Projectile Physics | Rigidbody & Colliders |
| Visual Effects | Particle Systems |
| Audio | Audio Sources with randomized pitch and volume |
| UI | Unity UI (health & cooldown indicators) |

## How to Run

**Build:** Unzip the downloadable build and run the executable.

**Editor:** Open the project in Unity 6.3 LTS (6000.3.10f1), open `Assets/Scenes/SampleScene`, and press Play.

## Credits and References

### Character
Erika Archer. Mixamo (Adobe), https://www.mixamo.com. Accessed 9 October 2026.

### Animations
All animations applied to Erika Archer are sourced from Mixamo.

**Milestone 1:** Unarmed Idle, Walking, Running, Running Backward, Right Strafe, Right Strafe Walk, Left Strafe, Left Strafe Walk, Jump, Crouch Walk Right, Crouch Walk Left, Crouch Walk Forward, Crouch Walk Back, and Crouch Idle.

**Milestone 2:** Magic Heal.

### Audio

"Classic Footstep SFX" by Matthew Anett. Unity Asset Store, version 1.0 (released 3 July 2020).

https://assetstore.unity.com/packages/audio/sound-fx/classic-footstep-sfx-173668

Licensed under the Standard Unity Asset Store EULA. Accessed 10 October 2026. Landing sound uses the clip "Floor_step16.wav" from this pack.

"Powerful Magic Fireball Impact" by mikiko850. Freesound.

https://freesound.org/people/mikiko850/sounds/848736/

"Boom Explosion" by BennettFilmTeacher. Freesound.

https://freesound.org/people/BennettFilmTeacher/sounds/523783/

### Materials & Visual Effects

"[Free Asset] VFX Particles: Fireball Pack" by SOLODREAM CREATION. Unity Asset Store, version 1.0.1 (released 21 November 2023).

https://assetstore.unity.com/packages/vfx/particles/fire-explosions/free-asset-vfx-particles-fireball-pack-263814

Licensed under the Standard Unity Asset Store EULA.

### Software and Packages

Unity 6.3 LTS (6000.3.10f1); Cinemachine; Input System; ProBuilder; Recorder.

### Original Work

Animator Controller and blend trees, PlayerMovement script, Cinemachine camera setup, grey-box gym geometry, fireball combat scripts, health systems, ScriptableObject configurations, and UI integration were created by the author.

### License Note

Mixamo characters and animations are used under Adobe's Mixamo terms. Third-party assets are credited to their respective creators and used under their applicable licenses.

## Reflection

See `Reflection.pdf` in this repository.
