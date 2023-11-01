### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Green Pillar

## Step 1
Use this code to make a bridge that reaches the Green Pillar. Press the green button to see what happens. Return and make changes to finish building the bridge. This code has some special parts called "repeat" blocks, which means it loops the same thing a number of times.

#### ~ tutorialhint 
Try changing the number inside the "repeat" block.

```ghost
hoc2023Objectives.pillar_AgentMove()
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock()
for (let i = 0; i < 3; i++ ) {}
```
```template
for (let i = 0; i < 3; i++ ) {
    hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
    hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```