### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Food Dispenser

## Step 1
جهاز توزيع الطعام لا يتمكن من التعرف على بعض الطلاب لأنه لا يستطيع رؤيتهم بشكل صحيح. اضغط على السهم الأخضر. انتبه إلى كيفية بحث الذكاء الاصطناعي عن الطلاب والتعرف عليهم. بعد ذلك، عد إلى الكود واجعله عادلا وشاملا بحيث يتمكن من التعرف على الطلاب من جميع الأطوال.

جرب إعدادا مختلفا للبلوك ``||hoc2023Objectives:scan <type>||`` .
#### ~ tutorialhint  
جرب إعدادا مختلفا للبلوك ``||hoc2023Objectives:scan <type>||`` .


```ghost
    hoc2023.scene1_LunchTime()
    hoc2023.scene1_DetectStudent()
    hoc2023Objectives.scene1_Scan()
    hoc2023.scene1_ServeLunch()
    hoc2023.scene1_WaitStudent()
```
```template
    while (hoc2023.scene1_LunchTime()) {
        hoc2023Objectives.scene1_Scan()
        if (hoc2023.scene1_DetectStudent()) {
            hoc2023.scene1_ServeLunch()
        }
        hoc2023.scene1_WaitStudent()
    }
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```