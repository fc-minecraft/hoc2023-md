### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Желтый столб

## Step 1
Этот код не приведет тебя к Желтому Столбу. Нажми зеленую кнопку и посмотри, как АГЕНТ строит. Обрати внимание на ошибки, которые допускает АГЕНТ. Исправь эти ошибки и заставь АГЕНТА построить мост, по которому ты сможешь перейти к Желтому Столбу.

#### ~ tutorialhint 
Похоже, что агент не завершает строительство моста.

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