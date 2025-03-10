### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Автомат для выдачи еды

## Step 1
Автомат с едой не находит некоторых учеников, потому что не может их хорошо рассмотреть. Нажми зеленую стрелку. Обрати внимание, как ИИ ищет и распознает учеников. Затем вернись к коду и сделай его справедливым и инклюзивным, чтобы он находил учеников ВСЕХ ростов.

Попробуй использовать другую настройку для блока ``||hoc2023Objectives:scan <type>||``.
#### ~ tutorialhint 
Попробуй использовать другую настройку для блока ``||hoc2023Objectives:scan <type>||``.


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