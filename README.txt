## README.txt

*Name of Project:*  
Procedural Spider Animation in Unity

*Name of Team Members:*  
- Dhruvrajsinh Zala [223066]  
- Vijay Khokhar [223131]

*How to Run the Project / Project Structure:*  
1. Open the project in Unity.  
2. Open the main scene located in the `Scenes` folder.  
3. Press Play to see the procedurally animated spider in action.  
4. Scripts are located in the `Code` folder; spider models and prefabs are in the `Prefabs` folder.

*Summary of Development/Research:*  
Most of our time was spent understanding and adapting the inverse kinematics (IK) system used for procedural animation of spider legs. We explored how to make the spider move realistically over uneven terrain and experimented with parameters like step distance, leg count, and body orientation.

*Challenges and Solutions:*  
- *Challenge:* Understanding and customizing the IK solver for multiple legs.  
  *Solution:* Studied open-source IK implementations and gradually adapted the logic for our spider model.
- *Challenge:* Achieving smooth, believable leg movement.  
  *Solution:* Tweaked stepping thresholds and lerp functions, and visualized leg targets to debug movement.
- *Challenge:* Integrating the procedural animation with Unity’s physics and navigation systems.  
  *Solution:* Used Unity’s built-in components and adjusted the animation update loop for compatibility.

*Lessons Learned:*  
- Procedural animation requires a good grasp of both mathematics and Unity’s scripting API.
- Debugging visualizations (like gizmos) are invaluable for understanding complex animation systems.
- Open-source projects and community tutorials can accelerate learning and problem-solving.

*References:*  
- Daniel Erdmann’s Fast IK solver (used for leg movement)
- Unity Asset Store: Free spider model
- Unity Documentation and community forums for troubleshooting

*Link to Short Feature Video (about 90s):*  
https://drive.google.com/file/d/1jkwX0g-4hgSXOmlXPFtLVmTU_4l7p-rR/view?usp=sharing

*Link to Project Files (if >100MB):*  
https://github.com/dhruvrajsinh9/procedural-animation-spider

*If Not Presented Live: Video Presentation (12–17 min):*  
https://drive.google.com/file/d/1EswSoKoDwRmRStNmL6c9eQNYoX9jGdwW/view?usp=sharing

*Presentation PPT Link:*
https://www.canva.com/design/DAGrX6LReyg/4VTb0KSaVjkqfDwzV2a-jQ/edit?utm_content=DAGrX6LReyg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
