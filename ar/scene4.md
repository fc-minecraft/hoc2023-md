### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Smart Doorlock

## Step 1
يمكن لأي شخص الاطلاع على تقرير الوصول الذي يوضح من قام باستخدام أقفال الأبواب، مما يشكل مشكلة كبيرة  بالخصوصية والأمان. يجب علينا تغيير الكود بحيث يتمكن الأشخاص المناسبون فقط، مثل المسؤولين، من رؤية التقارير.

#### ~ tutorialhint  
قم بتعديل جزء الكود الذي يتحقق من نوع المستخدم. يجب أن يسمح فقط للمسؤولين بالوصول إليه.

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