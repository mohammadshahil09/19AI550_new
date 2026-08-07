# Ex.No: 3  Basic movements in Unity 
### DATE: 7.08.2026                                                                          
### REGISTER NUMBER : 212224240184
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NewBehaviourScript : MonoBehaviour
{
    // Start is called before the first frame update
    public Transform o1;
    public Transform o2;
    public Transform o3;
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKeyUp(KeyCode.W))
        {
            o1.Translate(2f,0f,0f);
        }
        if (Input.GetKeyDown(KeyCode.A))
        {
            o2.localScale += new Vector3(0f,0f,0.2f);
        }
        if (Input.GetKeyDown(KeyCode.D))
        {
            o3.Rotate(0f,100f,0f);
        }
    }
}

```
### Output:

<img width="1915" height="1140" alt="image" src="https://github.com/user-attachments/assets/be73d242-1080-4f02-8441-c2a83f2bd0c9" />







### Result:
Thus the basic movement is learned through scripting
