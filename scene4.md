### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Умный дверной замок

## Step 1
Любой может видеть отчет о доступе, показывающий, кто использовал дверные замки, что является большой проблемой для конфиденциальности и безопасности. Нам нужно изменить код так, чтобы отчеты могли видеть только нужные люди, такие как администраторы.

Порпобуй ПОСЛЕ ПРОВЕРКИ РАЗРЕШЕНИЯ добавить блок "ЕСЛИ РАЗРЕШЕНИЯ ИГРОКОВ РАВНЫ" и выбрать, игроки с каким разрешением получат доступ.
ОТКЛЮЧИ просмотр журнала тем игрокам, которые НЕ ДОЛЖНЫ получить доступ.

#### ~ tutorialhint 
Измени часть кода, где проверяется, какой ты пользователь. "ЕСЛИ РАЗРЕШЕНИЯ ИГРОКОВ РАВНЫ АДМИНИСТРАТОР", ТО ВКЛЮЧИТЬ ПРОСМОТР. ИНАЧЕ - ВЫКЛЮЧИТЬ.

```ghost
hoc2023.scene4_HumanDetected()
hoc2023.scene4_UserAuthorized()
hoc2023.scene4_UserPermissions()
hoc2023.scene4_DoorClosed()
hoc2023Objectives.scene4_UserAdmin()
hoc2023.scene4_CheckUserPermissions()
hoc2023.scene4_EnableLogViewing()
hoc2023.scene4_DisableLogViewing()
hoc2023.scene4_LogUnauthorizedEvent()
hoc2023.scene4_LogAuthorizedEvent()
hoc2023.scene4_LockDoor()
hoc2023.scene4_UnlockDoor()
hoc2023.scene4_WaitMinutes(5)
    while (hoc2023.scene4_HumanDetected()) {
        if (hoc2023.scene4_UserAuthorized()) {
            hoc2023.scene4_CheckUserPermissions()
            if (hoc2023.scene4_UserPermissions() == hoc2023Objectives.scene4_UserAdmin())  {
                hoc2023.scene4_EnableLogViewing()
            } else {
                hoc2023.scene4_DisableLogViewing()
            }
        }
    }
```
```template
    while (hoc2023.scene4_HumanDetected()) {
        if (hoc2023.scene4_UserAuthorized()) {
            hoc2023.scene4_CheckUserPermissions()
            hoc2023.scene4_EnableLogViewing()
        }
    }

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```