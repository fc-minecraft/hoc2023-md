### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Smart Lawnmower

## Step 1
Oh no! The Smart Lawnmower isn't too smart! It's running over sprinkler heads breaking them! Read through the code and update it so the lawnmower will first check for sprinkler heads before continuing.

```ghost
    hoc2023.scene2_GrassCut()
    hoc2023.scene2_CheckSprinklerGrassCut()
    hoc2023.scene2_LawnmowerNextRow()
    hoc2023.scene2_LawnmowerMoveForward()
```
```template
    for (let i = 0; i < 4; i++ ) {
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_GrassCut()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_GrassCut()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_GrassCut()    
        hoc2023.scene2_LawnmowerNextRow()    
    }  
```

```package
artemis-ts=github:ReWrite-Media/hoc2023-ts#v0.0.2
```