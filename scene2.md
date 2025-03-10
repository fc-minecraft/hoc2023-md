### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Газонокосилка

## Step 1
Нажми зеленую стрелку, чтобы протестировать код Умной Газонокосилки. Она повреждает поливочные головки? Сейчас она не выглядит такой уж умной! Давай сделаем её безопасной и надежной, изменив код так, чтобы она проверяла наличие поливочных головок ДО того, как начнет косить траву.

#### ~ tutorialhint 
Замени блок ``||hoc2023Objectives:cut grass||`` одним из других блоков.

```ghost
    hoc2023Objectives.scene2_GrassCut()
    hoc2023Objectives.scene2_CheckSprinklerGrassCut()
    hoc2023.scene2_LawnmowerNextRow()
    hoc2023.scene2_LawnmowerMoveForward()
//
```
```template
    for (let i = 0; i < 8; i++ ) {
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerMoveForward()
        hoc2023.scene2_LawnmowerNextRow()    
    }  
//
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```