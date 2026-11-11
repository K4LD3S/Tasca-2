# Kill the Avocado 2

**Activity 2 – Meta XR Building Blocks** · *Entorns de Realitat Virtual*
Grau en Disseny, Animació i Art Digital · UPC (Universitat Politècnica de Catalunya) · 2026-2027

Kill the Avocado 2 is a Virtual Reality / Mixed Reality application built with **Unity** and the **Meta XR SDK** for **Meta Quest 3**. It integrates, in a single project, the three activities required by the assignment: grab + locomotion, passthrough + hand tracking, and an additional Building Block.

## Authors

| Name | GitHub |
|---|---|
| Isaac Oliver Monells | `@isaacolivermonells` |
| David Pau Caldés Bou | `@K4LD3S` |

**Tutor:** Marc Galvez

## Download

Everything is in the **[Releases page](RELEASE_LINK_HERE)**:

- APK for Meta Quest 3
- Demo video recorded from the headset (shows the three activities)
- `KillTheAvocado2_Documentation.pdf`

## Activities

### Activity 1 – Grab and Locomotion
The user can grab, move and release 3D objects with the **controllers**, and move around the virtual environment using **teleport**.

| Building Block | Use |
|---|---|
| Grab Interaction | Grab, move and release objects with the controllers |
| Teleport Interaction | Locomotion method for moving around the virtual space |

**Teleport:** a **thumbs up** gesture enters teleport mode, an arc is shown with a marker where you will land, and lowering the thumb teleports you to that point.

### Activity 2 – Passthrough and Hand Tracking (MR)
The user sees the real room through the headset with virtual objects placed in it, and can interact with them using their **bare hands**. In-app buttons control the passthrough and switch between the VR environment (virtual background) and the mixed reality view.

| Building Block | Use |
|---|---|
| Passthrough | Shows the real room through the headset; buttons to toggle VR ↔ MR |
| Hand Tracking | Grab, move and release objects without controllers |

### Activity 3 – Additional Building Block
| Building Block | Use |
|---|---|
| Spatial Anchor Core | Anchors virtual content in the real space |
| Sample Spatial Anchor Controller | Used to make the avocado appear |

## Implementation overview

All features were implemented with the Meta XR SDK Building Blocks menu: the blocks were added to the scene and their configuration was adjusted to fit the project.

- **Passthrough:** Passthrough block added to the scene, plus buttons to control it and switch between the virtual environment and mixed reality.
- **Teleport Interaction:** block added and configured so the user can move around the scene (arc + landing point, thumbs-up gesture to activate).
- **Hand Tracking:** block added so the user can interact without controllers.
- **Grab Interaction:** block added to the sword.
- **Spatial Anchor Core & Sample Spatial Anchor Controller:** used to spawn the avocado.

## Development process

The project started in class, where both members did the initial Unity + Meta XR SDK setup together. Afterwards, one member took care of the assets and the documentation, and the other handled the finalization of the program, integrating and adjusting the features so they work together in the final application.

## Problems and solutions

- **Problem:** we had no physical HMD available for testing, which made it hard to check that the features worked.
- **Solution:** we used the **Meta XR Simulator** to test the application without a headset, which let us validate most of the features.
- **Limitation:** the Meta XR Simulator does not allow testing teleport, but it had already been tested beforehand.

## Team contributions

**Isaac Oliver Monells**
- Initial project setup (together with David)
- Application assets
- Documentation

**David Pau Caldés Bou**
- Initial project setup (together with Isaac)
- Program finalization (integration and final adjustments)

## Requirements

- Unity (version: `6.4.9 F1`)
- Meta XR SDK (Building Blocks)
- Meta Quest 3

## Installing the APK

1. Download the APK from the [Releases page](RELEASE_LINK_HERE).
2. Enable developer mode on your Quest 3.
3. Sideload the APK (e.g. with `adb install KillTheAvocado2.apk` or SideQuest).
4. Launch it from *Unknown Sources* in the Quest library.

## Documentation

The full documentation is available in [`KillTheAvocado2_Documentation.pdf`](RELEASE_LINK_HERE) (in the Release and uploaded to Atenea).
