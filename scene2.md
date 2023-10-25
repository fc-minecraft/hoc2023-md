### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Lawnmower

## Step 1
Oops! The Smart Lawnmower isn't too smart right now. It's running over sprinkler heads and causing damage. Let's make it smarter by changing some parts of the code. You'll replace certain blocks with new ones so that the lawnmower first checks for sprinkler heads before it starts cutting the grass.

#### ~ tutorialhint 
Remove the cut grass block with one of the other blocks in the tool box.

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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```