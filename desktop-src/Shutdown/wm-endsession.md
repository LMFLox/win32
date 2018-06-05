---
Description: The WM\_ENDSESSION message is sent to an application after the system processes the results of the WM\_QUERYENDSESSION message. The WM\_ENDSESSION message informs the application whether the session is ending.
ms.assetid: 9bf04f24-da1e-4680-a47b-28e9c500635e
title: WM\_ENDSESSION message
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# WM\_ENDSESSION message

The **WM\_ENDSESSION** message is sent to an application after the system processes the results of the [**WM\_QUERYENDSESSION**](wm-queryendsession.md) message. The **WM\_ENDSESSION** message informs the application whether the session is ending.

A window receives this message through its [**WindowProc**](https://www.bing.com/search?q=**WindowProc**) function.


```C++
LRESULT CALLBACK WindowProc( 
  HWND hwnd,      // handle to window 
  UINT uMsg,      // message identifier 
  WPARAM wParam,  // end-session option 
  LPARAM lParam   // logoff option
);
```



## Parameters

<dl> <dt>

*hwnd* 
</dt> <dd>

A handle to the window.

</dd> <dt>

*uMsg* 
</dt> <dd>

The **WM\_ENDSESSION** identifier.

</dd> <dt>

*wParam* 
</dt> <dd>

If the session is being ended, this parameter is **TRUE**; the session can end any time after all applications have returned from processing this message. Otherwise, it is **FALSE**.

</dd> <dt>

*lParam* 
</dt> <dd>

This parameter can be one or more of the following values. If this parameter is 0, the system is shutting down or restarting (it is not possible to determine which event is occurring).



| Value                                                                                                                                                                                                                                           | Meaning                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="ENDSESSION_CLOSEAPP"></span><span id="endsession_closeapp"></span><dl> <dt>**ENDSESSION\_CLOSEAPP**</dt> <dt>0x1</dt> </dl>        | If *wParam* is **TRUE**, the application must shut down. Any data should be saved automatically without prompting the user (for more information, see Remarks). The Restart Manager sends this message when the application is using a file that needs to be replaced, when it must service the system, or when system resources are exhausted. The application will be restarted if it has registered for restart using the [**RegisterApplicationRestart**](https://msdn.microsoft.com/windows/desktop/f4cd25b3-2aee-460f-9f9f-b45ecded094f) function. For more information, see [Guidelines for Applications](https://msdn.microsoft.com/windows/desktop/97b1df63-65a9-47b4-891b-e4a754882b89). <br/> If *wParam* is **FALSE**, the application should not shut down.<br/> |
| <span id="ENDSESSION_CRITICAL"></span><span id="endsession_critical"></span><dl> <dt>**ENDSESSION\_CRITICAL**</dt> <dt>0x40000000</dt> </dl> | The application is forced to shut down.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| <span id="ENDSESSION_LOGOFF"></span><span id="endsession_logoff"></span><dl> <dt>**ENDSESSION\_LOGOFF**</dt> <dt>0x80000000</dt> </dl>       | The user is logging off. For more information, see [Logging Off](logging-off.md).<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |



 

Note that this parameter is a bit mask. To test for this value, use a bit-wise operation; do not test for equality.

</dd> </dl>

## Return value

If an application processes this message, it should return zero.

## Remarks

Applications that have unsaved data could save the data to a temporary location and restore it the next time the application starts. It is recommended that applications save their data and state frequently; for example, automatically save data between save operations initiated by the user to reduce the amount of data to be saved at shutdown.

The application need not call the [**DestroyWindow**](https://www.bing.com/search?q=**DestroyWindow**) or [**PostQuitMessage**](https://www.bing.com/search?q=**PostQuitMessage**) function when the session is ending.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps \| UWP apps\]<br/>                                                       |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps \| UWP apps\]<br/>                                              |
| Header<br/>                   | <dl> <dt>WinUser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

[Logging Off](logging-off.md)
</dt> <dt>

[Shutting Down](shutting-down.md)
</dt> <dt>

[**DestroyWindow**](https://www.bing.com/search?q=**DestroyWindow**)
</dt> <dt>

[**PostQuitMessage**](https://www.bing.com/search?q=**PostQuitMessage**)
</dt> <dt>

[**SetProcessShutdownParameters**](https://msdn.microsoft.com/windows/desktop/c467950e-31e1-4608-a08a-0736a5524e0e)
</dt> <dt>

[**WM\_QUERYENDSESSION**](wm-queryendsession.md)
</dt> </dl>

 

 



