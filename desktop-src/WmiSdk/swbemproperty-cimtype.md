---
Description: 'The CIMType property of the SWbemProperty object is an integer that can be used to determine the CIM type of this property. This property is read-only.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: 'fb570ba4-6ce3-4131-8088-2761110033ba'
ms.prod: 'windows-server-dev'
ms.technology: 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: 'SWbemProperty.CIMType property'
---

# SWbemProperty.CIMType property

The **CIMType** property of the [**SWbemProperty**](swbemproperty.md) object is an integer that can be used to determine the CIM type of this property. This property is read-only.

For an explanation of this syntax, see [Document Conventions for the Scripting API](document-conventions-for-the-scripting-api.md).

This property is read-only.

## Syntax


```VB
SWbemProperty.CIMType As Integer
```



## Property value

## Remarks

For more information about valid types for this property, see [**WbemCimtypeEnum**](wbemcimtypeenum.md).

Instances of embedded objects are stored in composite objects as properties of type **CIM\_OBJECT**. To determine the class of an embedded object in an instance of a composite class, you must examine the **CIMType** qualifier of the **CIM\_OBJECT** type property.

The object references in an association class are stored in properties of type **CIM\_REFERENCE**. To determine the actual object paths you must examine the **CIMType** qualifier of the **CIM\_REFERENCE** type property.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server�2008<br/>                                                          |
| Header<br/>                   | <dl> <dt>Wbemdisp.h</dt> </dl>   |
| Type library<br/>             | <dl> <dt>Wbemdisp.tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | CLSID\_SWbemProperty<br/>                                                         |
| IID<br/>                      | IID\_ISWbemProperty<br/>                                                          |



�

�



