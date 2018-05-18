---
Description: 'Handle to the local Policy object.'
ms.assetid: 'f5878d27-558b-4ef1-9401-1277e740c61d'
title: 'LSA\_HANDLE'
---

# LSA\_HANDLE

The **LSA\_HANDLE** data type is a handle to the local [**Policy**](policy-object.md) object.


```C++
typedef PVOID LSA_HANDLE, *PLSA_HANDLE;
```



## Remarks

Before you can use the local policy API your application must open a handle to a [**Policy**](policy-object.md) object. To do this, call [**LsaOpenPolicy**](https://msdn.microsoft.com/library/windows/desktop/aa378299). This function returns a handle that your application can then specify in subsequent LSA policy function calls.

Each handle has an associated set of permissions that determine the operations your application can perform on the [**Policy**](policy-object.md) object by using the handle. Your application can open more than one handle to the **Policy** object at a time. When a handle is no longer required, your application should close it by calling [**LsaClose**](lsaclose.md).

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Ntsecapi.h</dt> </dl> |



## See also

<dl> <dt>

[**LsaClose**](lsaclose.md)
</dt> <dt>

[**LsaOpenPolicy**](https://msdn.microsoft.com/library/windows/desktop/aa378299)
</dt> </dl>

�

�



