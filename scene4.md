### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Smart Doorlock

## Step 1
Anyone can see the records of who has been using the doorlocks, which is a big problem for privacy and safety. You should change the code so that only administrators can look at the event logs.

#### ~ tutorialhint 
Change the part of the code where it checks what kind of user you are. Only administrators should be allowed to access it.

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
            hoc2023.scene4_UnlockDoor()
            hoc2023.scene4_LogAuthorizedEvent()
        } else {
            hoc2023.scene4_LogUnauthorizedEvent()
        }
        if (hoc2023.scene4_DoorClosed()) {
            hoc2023.scene4_WaitMinutes(5)
            hoc2023.scene4_LockDoor()
        }
    }

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```