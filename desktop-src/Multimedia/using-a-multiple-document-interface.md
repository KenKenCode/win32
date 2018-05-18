---
title: Using a Multiple Document Interface
description: Using a Multiple Document Interface
ms.assetid: 'bc59f19c-1064-4df8-8864-38e6d188f92f'
keywords: ["MCIWndRegisterClass function"]
---

# Using a Multiple Document Interface

Applications that use a multiple document interface (MDI) might need to specify window styles that are not available through the [**MCIWndCreate**](mciwndcreate.md) function. For these applications, you can register and create an MCIWnd window by using the [**MCIWndRegisterClass**](mciwndregisterclass.md) function with the [CreateWindowEx](http://go.microsoft.com/fwlink/p/?linkid=16991) function. The **MCIWndRegisterClass** function registers the MCIWND\_WINDOW\_CLASS window class and then **CreateWindowEx** creates an instance of an MCIWnd window.

 

 



