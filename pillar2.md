### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Желтая платформа

## Step 1
Этот код не приведет тебя к желтой платформе. Нажми зеленую кнопку и посмотри, как АГЕНТ строит. Обрати внимание на ошибки, которые допускает АГЕНТ. Исправь эти ошибки и заставь АГЕНТА построить мост.

#### ~ tutorialhint 
Похоже, что агент не завершает строительство моста.

```ghost
for (let i = 0; i < 3; i++ ) {}
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