### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Yellow Pillar

## Step 1
This code won't get you to the Yellow Pillar. Press the green button and watch the AGENT build. Notice the mistakes the AGENT makes. Fix those mistakes and get the AGENT to build a bridge that you can cross to the Yellow Pillar.

#### ~ tutorialhint 
It looks like the agent is not completing the bridge.

```ghost
hoc2023Objectives.pillar_AgentMove()
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock()
```
```template
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