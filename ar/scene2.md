### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Lawnmower

## Step 1
اضغط على السهم الأخضر لاختبار كود جزازة العشب الذكية لقص العشب. هل تتسبب في دهس رؤوس الرشاشات وإحداث أضرار؟ يبدو أنها ليست ذكية تماما! لنجعلها آمنة وموثوقة من خلال تعديل كودها ليتحقق من وجود رؤوس الرشاشات قبل أن تبدأ في قص العشب.

#### ~ tutorialhint  
قم بإزالة البلوك ``||hoc2023Objectives:cut grass||`` واستبدله بإحدى البلوكات الأخرى الموجودة في صندوق الأدوات

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