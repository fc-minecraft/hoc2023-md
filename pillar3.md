### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Зеленый столб

## Step 1
Используй этот код, чтобы построить мост, который достигает Зеленого Столба. Нажми зеленую кнопку, чтобы увидеть, что произойдет. Вернись и внеси изменения, чтобы завершить строительство моста. В этом коде есть специальные части, называемые "повторить" блоками, которые означают, что одно и то же действие повторяется несколько раз.


#### ~ tutorialhint 
Попробуй изменить число внутри блока "повторить".

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