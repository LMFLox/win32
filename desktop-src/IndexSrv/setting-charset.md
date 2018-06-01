---
Description: Setting Charset
ms.assetid: d2720abc-091a-48d9-b568-0fccc6deec8f
title: Setting Charset
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Setting Charset

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The **Charset** attribute is the part of the HTTP-EQUIV meta tag that specifies the character set of an HTML page. Indexing Service uses this character set to display the text in the HTML page in the proper characters. In a file written in Japanese, you would set the **Charset** to shift\_jis as shown in the following example:


```
<META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=shift_jis">
```



To find a list of recognized character set codes, see [Recognized Character Set Tags](recognized-character-set-tags.md).

 

 


