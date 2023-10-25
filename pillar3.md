### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Green Pillar

## Step 1
Use this code to make a bridge and get to the top of the green pillar. First, run the instructions to see what happens, and then make changes to finish building the bridge. This code has some special parts called "repeat" blocks, which means it does the same thing a number of times.

#### ~ tutorialhint 
It looks like the agent is placing some of the blocks in the wrong direction.

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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```