### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Smart Doorlock

## Step 1
Anyone can access the event logs on the doorlock causing a major privacy and security issue. We need to update the code to make sure only admins can access the event logs.

#### ~ tutorialhint 
Update where the code compares the user permissions. Only admins should have access. 

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
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.51
```