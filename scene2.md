### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Газонокосилка

## Step 1
Газонокосилка повреждает поливочные головки? Сейчас она не выглядит такой уж умной! Давай сделаем её безопасной и надежной, изменив код так, чтобы она проверяла наличие поливочных головок ДО того, как начнет косить траву.

Сначала добавь цикл на 8 повторений. Затем перемещай газонокосилку вперед 3 раза, скашивая траву на каждом блоке. После чего переходи на следующий ряд.


#### ~ tutorialhint 
Замени блок "косить траву" одним из других блоков.

```ghost
    hoc2023Objectives.scene2_GrassCut()
    hoc2023Objectives.scene2_CheckSprinklerGrassCut()
    hoc2023.scene2_LawnmowerNextRow()
    hoc2023.scene2_LawnmowerMoveForward()
        for (let i = 0; i < 8; i++ ) {
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerNextRow()    
    }  
//
```
```template

//
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```