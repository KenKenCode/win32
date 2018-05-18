---
title: CopyRootCauseInfo function
description: Creates a copy of a RootCauseInfo structure.
ms.assetid: '6bcd1341-657a-40c1-bebd-1c0f780ae337'
keywords: ["CopyRootCauseInfo function NDF"]
topic_type:
- apiref
api_name:
- CopyRootCauseInfo
api_location:
- ndattributils.h
api_type:
- HeaderDef
---

# CopyRootCauseInfo function

The **CopyRootCauseInfo** function creates a copy of a [**RootCauseInfo**](rootcauseinfo.md) structure.

## Syntax


```C++
HRESULT CopyRootCauseInfo(
  _Out_�������RootCauseInfo *Dest,
  _In_��const RootCauseInfo *Source
);
```



## Parameters

<dl> <dt>

*Dest* \[out\]
</dt> <dd>

Type: **[**RootCauseInfo**](rootcauseinfo.md)\***

The structure to be updated.

</dd> <dt>

*Source* \[in\]
</dt> <dd>

Type: **const [**RootCauseInfo**](rootcauseinfo.md)\***

The existing structure to be copied.

</dd> </dl>

## Return value

Type: **HRESULT**

Possible return values include, but are not limited to, the following.



| Return code                                                                                   | Description                                                                 |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | The operation succeeded.<br/>                                         |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | One or more parameters has not been provided correctly.<br/>          |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | There is not enough memory available to complete this operation.<br/> |



�

## Requirements



|                                     |                                                                                            |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�8 \[desktop apps only\]<br/>                                                 |
| Minimum supported server<br/> | Windows Server�2012 \[desktop apps only\]<br/>                                       |
| Header<br/>                   | <dl> <dt>Ndattributils.h</dt> </dl> |



## See also

<dl> <dt>

[**RootCauseInfo**](rootcauseinfo.md)
</dt> </dl>

�

�




