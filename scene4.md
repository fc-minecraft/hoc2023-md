### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Smart Doorlock

## Step 1
Anyone can see the access report showing who has been using the door locks, which is a big problem for privacy and security. We should change the code so that only the right people, such as admins, can see the reports.

#### ~ tutorialhint 
Change the part of the code where it checks what kind of user you are. Only admins should be allowed to access it.

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