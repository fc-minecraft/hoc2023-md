### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Sound Detector

## Step 1
SMART DOORLOCK

```ghost
hoc2023.scene3_HumanDetected()
hoc2023.scene3_UserAuthorized()
hoc2023.scene3_UserPermissions()
hoc2023.scene3_DoorClosed()
hoc2023.scene3_Admin()
hoc2023.scene3_CheckUserPermissions()
hoc2023.scene3_EnableLogViewing()
hoc2023.scene3_DisableLogViewing()
hoc2023.scene3_LogUnauthorizedEvent()
hoc2023.scene3_LogAuthorizedEvent()
hoc2023.scene3_LockDoor()
hoc2023.scene3_UlockDoor()
hoc2023.scene3_WaitMinutes(5)
```
```template
    while (hoc2023.scene3_HumanDetected()) {
        if (hoc2023.scene3_UserAuthorized()) {
            hoc2023.scene3_CheckUserPermissions()
            if (hoc2023.scene3_UserPermissions() == true) {
                hoc2023.scene3_EnableLogViewing()
            } else {
                hoc2023.scene3_DisableLogViewing()
            }
            hoc2023.scene3_UlockDoor()
            hoc2023.scene3_LogAuthorizedEvent()
        } else {
            hoc2023.scene3_LogUnauthorizedEvent()
        }
        if (hoc2023.scene3_DoorClosed()) {
            hoc2023.scene3_WaitMinutes(5)
            hoc2023.scene3_LockDoor()
        }
    }

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts#v0.0.8
```