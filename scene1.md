### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Автомат для выдачи еды

## Step 1
Автомат с едой не находит некоторых учеников, потому что не может их хорошо рассмотреть.

Давай исправим это! Когда время обеда - сканируй ученика. Затем добавь условие "ЕСЛИ НАЙДЕН УЧЕНИК", чтобы подавать обед.

#### ~ tutorialhint 
Попробуй использовать другую настройку для блока "scan".

```ghost
    hoc2023.scene1_LunchTime()
    hoc2023.scene1_DetectStudent()
    hoc2023Objectives.scene1_Scan()
    hoc2023.scene1_ServeLunch()
    hoc2023.scene1_WaitStudent()
        while (hoc2023.scene1_LunchTime()) {
        hoc2023Objectives.scene1_Scan()
        if (hoc2023.scene1_DetectStudent()) {
            hoc2023.scene1_ServeLunch()
        }
        hoc2023.scene1_WaitStudent()
    }
```
```template
    while (hoc2023.scene1_LunchTime()) {
        hoc2023.scene1_WaitStudent()
    }
```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```