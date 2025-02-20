### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Yellow Pillar

## Step 1
هذا الكود  لن يوصلك إلى العمود الأصفر. اضغط على الزر الأخضر وراقب كيفية بناء الروبوت للجسر. انتبه للأخطاء التي يرتكبها الروبوت، ثم قم بتصحيحها حتى يتمكن من بناء جسر يمكنك عبوره إلى العمود الأصفر.

#### ~ tutorialhint  
يبدو أن الروبوت لا يكمل بناء الجسر.

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