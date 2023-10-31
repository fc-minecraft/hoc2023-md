### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Lawnmower

## Step 1
Press the green arrow to test the Smart Mower's code. Running over sprinkler heads and causing damage? It isn't looking too smart now! Let's make it Safe and Reliable by changing its code so that it checks for sprinkler heads BEFORE it starts cutting the grass.

#### ~ tutorialhint 
Remove the ``||hoc2023Objectives:cut grass||`` block with one of the other blocks in the tool box.

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