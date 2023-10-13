### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Sound Detector

## Step 1
Oh no! The Smart Lawnmower isn't too smart! It's running over sprinkler heads breaking them! Read through the code and update it so the lawnmower will first check for sprinkler heads before continuing.

#### ~ tutorialhint 
Make sure the lawnmower is checking to see if there's a sprinkler before cutting the grass.

```ghost
    hoc2023Objectives.scene2_GrassCut()
    hoc2023Objectives.scene2_CheckSprinklerGrassCut()
    hoc2023.scene2_LawnmowerNextRow()
    hoc2023.scene2_LawnmowerMoveForward()
//
```
```template
    for (let i = 0; i < 8; i++ ) {
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023Objectives.scene2_GrassCut()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023Objectives.scene2_GrassCut()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023Objectives.scene2_GrassCut()    
        hoc2023.scene2_LawnmowerNextRow()    
    }  
//
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.51
```