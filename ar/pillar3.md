### @flyoutOnly true
### @hideIteration true
### @explicitHints true

# Green Pillar

## Step 1
استخدم هذا الكود لبناء جسر يصل إلى العمود الأخضر. اضغط على الزر الأخضر لترى ما سيحدث. عد وأجرِ التعديلات اللازمة لإكمال بناء الجسر. يحتوي هذا الكود على بعض الأجزاء الخاصة المعروفة باسم "تكرار"، مما يعني تكرار نفس العملية لعدد معين من المرات.

#### ~ tutorialhint 
حاول تغيير الرقم داخل بلوك "تكرار".

```ghost
hoc2023Objectives.pillar_AgentMove()
hoc2023Objectives.pillar_AgentPlacePinkWoolBlock()
for (let i = 0; i < 3; i++ ) {}
```
```template
for (let i = 0; i < 3; i++ ) {
    hoc2023Objectives.pillar_AgentMove(ForwardBackUpDown.Forward)
    hoc2023Objectives.pillar_AgentPlacePinkWoolBlock(UpDown.Up)
}

```

```package
hoc2023-ts=github:ReWrite-Media/hoc2023-ts
```