---
title: DTN\_DATETIMECHANGE notification code
description: Sent by a date and time picker (DTP) control whenever a change occurs. This notification code is sent in the form of a WM\_NOTIFY message.
ms.assetid: 65cdd8fb-1f07-4447-b503-d40fdfa37202
keywords:
- DTN_DATETIMECHANGE notification code Windows Controls
topic_type:
- apiref
api_name:
- DTN_DATETIMECHANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# DTN\_DATETIMECHANGE notification code

Sent by a date and time picker (DTP) control whenever a change occurs. This notification code is sent in the form of a [**WM\_NOTIFY**](wm-notify.md) message.


```C++
DTN_DATETIMECHANGE

    lpChange = (LPNMDATETIMECHANGE) lParam;
```



## Parameters

<dl> <dt>

*lParam* 
</dt> <dd>

A pointer to an [**NMDATETIMECHANGE**](/windows/desktop/api/Commctrl/ns-commctrl-tagnmdatetimechange) structure containing information about the change that took place in the control.

</dd> </dl>

## Return value

The owner of the control must return zero.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




