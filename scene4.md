### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Умный дверной замок

## Step 1
Любой может видеть отчет о доступе, показывающий, кто использовал дверные замки, что является большой проблемой для конфиденциальности и безопасности. Нам нужно изменить код так, чтобы отчеты могли видеть только нужные люди, такие как администраторы.

#### ~ tutorialhint 
Измени часть кода, где проверяется, какой ты пользователь. Только администраторам должно быть разрешено получать доступ к отчету.

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
```
```template
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

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```