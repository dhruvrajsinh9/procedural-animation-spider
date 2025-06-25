# Procedural Spider Animation in Unity

*Example of procedural spider movement*

## Project Overview

This Unity project implements **procedural animation for spiders** using inverse kinematics (IK) to create realistic leg movement. The spider dynamically adapts to terrain without pre-made animations.

## Team Members

- Dhruvrajsinh Zala [223066]
- Vijay Khokhar [223131]


## Project Structure

```
Assets/
├── Code/               # C# scripts
│   ├── BodyManager.cs  # Controls spider body movement
│   └── LegController.cs # Handles individual leg logic
├── Prefabs/            # Spider models and prefabs
├── Scenes/             # Unity scene files
│   └── MainScene.unity # Primary demonstration scene
```


## How to Run

1. Open project in **Unity 2021.3+**
2. Load `Scenes/MainScene.unity`
3. Press **Play** to start simulation
4. Control the spider using:
    - **WASD**: Movement
    - **QE**: Rotation
    - **R**: Reset scene

## Development Summary

| Focus Area | Details |
| :-- | :-- |
| **Core Research** | Inverse kinematics implementation for multi-legged creatures |
| **Key Parameters** | Step distance, leg count, body orientation, terrain adaptation |
| **Testing** | Over 50 iterations refining movement smoothness |

## Challenges \& Solutions

| Challenge | Solution |
| :-- | :-- |
| IK implementation for multiple legs | Adapted Daniel Erdmann's Fast IK solver |
| Unnatural leg movement | Implemented sine-based stepping algorithm |
| Physics integration | Custom update loop synced with Unity's physics |

## Lessons Learned

- 🧮 **Mathematics is crucial** for realistic procedural animation
- 👁️‍🗨️ Debugging visualizations are essential for IK systems
- 🤝 Open-source resources accelerate development
- ⚙️ Parameter tuning requires extensive iteration


## References

- **IK Solver**: Daniel Erdmann's Fast IK
- **Spider Model**: Unity Asset Store (free)
- **Unity Documentation**: Animation Rigging package



## Technical Highlights

```csharp
// Simplified leg stepping logic (LegController.cs)
IEnumerator Step() {
    while(Vector3.Distance(target, steppingPoint) > 0.6f) {
        target.position = Vector3.MoveTowards(...);
        SineStep(steppingPoint); // Custom curve-based motion
        yield return new WaitForSeconds(Time.deltaTime);
    }
}
```
---
*Project created for educational purposes - June 2025*

