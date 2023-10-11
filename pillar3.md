### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Green Pillar

## Step 1
Use code to get to the top of the green pillar

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
    hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.40
```