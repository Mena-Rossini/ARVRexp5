# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : Mena Rossini R
### REG NO : 212222040099

```
using UnityEngine;

public class Movement : MonoBehaviour
{
   
     public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent < Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputY = Input.GetAxis("Vertical");
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputY", InputY);
        animator.SetFloat("InputX", InputX);
    }

}

```
## Output :
![5 1](https://github.com/user-attachments/assets/0a7adfc8-9399-4c71-9abf-ae4d71a77e28)

![5 2](https://github.com/user-attachments/assets/752aa0aa-302b-4b67-9855-7a8c52dc70ac)

![5 3](https://github.com/user-attachments/assets/e2ead3bf-5906-4371-bcee-df1e7657b6b5)

## Result :

An animator movement for a player using unity is developed successfully.
