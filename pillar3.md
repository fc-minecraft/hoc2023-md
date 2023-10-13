### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Green Pillar

## Step 1
Use code to get to the top of the green pillar Run the code first to see how it works, and then modify it to complete the bridge.

#### ~ tutorialhint 
It seems like the Agent is placing some of the blocks in the wrong direction.

```ghost
hoc2023Objectives.pillar_AgentMove()
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock()
for (let i = 0; i < 8; i++ ) {}
```
```template
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)
for (let i = 0; i < 3; i++ ) {
    hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
    hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Up)
    hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
}
for (let i = 0; i < 3; i++ ) {
    hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
    hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.54
```