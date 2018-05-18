---
title: IAgentCommandsEx SetVoiceCaption
description: IAgentCommandsEx SetVoiceCaption
ms.assetid: 'f13c9ca5-70c9-42d0-b53c-45dc8980a24c'
---

# IAgentCommandsEx::SetVoiceCaption

\[Microsoft Agent is deprecated as of Windows 7, and may be unavailable in subsequent versions of Windows.\]

``` syntax
HRESULT SetVoiceCaption(
   BSTR bszVoiceCaption  // voice caption text
);
```

Sets the [**VoiceCaption**](voicecaption-property.md) text displayed for the [**Command**](https://msdn.microsoft.com/library/windows/desktop/ms696441) object.

-   Returns S\_OK to indicate the operation was successful.

<dl> <dt>

<span id="bszVoiceCaption"></span><span id="bszvoicecaption"></span><span id="BSZVOICECAPTION"></span>*bszVoiceCaption*
</dt> <dd>

A BSTR that specifies the text for the [**VoiceCaption**](voicecaption-property.md) property for a [**Command**](https://msdn.microsoft.com/library/windows/desktop/ms696441).

</dd> </dl>

If you define a [**Command**](https://msdn.microsoft.com/library/windows/desktop/ms696441) object in a [**Commands**](https://msdn.microsoft.com/library/windows/desktop/ms695971) collection and set its [**Voice**](voice-property.md) property, you will typically also set its [**VoiceCaption**](voicecaption-property.md) property. This text will appear in the Voice Commands Window when your client application is input-active and the character is visible. If this property is not set, the setting for the [**Caption**](caption-property.md) property determines the text displayed. When neither the **VoiceCaption** or **Caption** property is set, the command does not appear in the Voice Commands Window.

## See Also

[**IAgentCommandsEx::GetVoiceCaption**](iagentcommandsex--getvoicecaption.md)


 

 



