### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Yellow Pillar

## Step 1
This program won't get you to the Yellow Pillar. When you use it, you'll see what happens to the AGENT as it tries to make a bridge with blocks. Watch how the agent places the blocks and the mistakes it makes. Then, check the program and fix those mistakes.

#### ~ tutorialhint 
It looks like the agent is placing some of the blocks in the wrong direction.

```ghost
hoc2023Objectives.pillar_AgentMove()
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock()
```
```template
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Up)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Up)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Up)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)
hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Down)

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```