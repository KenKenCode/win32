---
title: SetReadonly method of the MSFT\_SMStorageVolume class
description: Changes the device access of the storage volume to Readable.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 'b6ca3df1-b75f-455f-a737-326f6fa5751f'
ms.prod: 'windows-server-dev'
ms.technology: 'windows-management-instrumentation'
ms.tgt_platform: multiple
keywords: ["SetReadonly method", "SetReadonly method, MSFT_SMStorageVolume class", "MSFT_SMStorageVolume class, SetReadonly method"]
topic_type:
- apiref
api_name:
- MSFT_SMStorageVolume.SetReadonly
api_location:
- StorageService.dll
api_type:
- COM
---

# SetReadonly method of the MSFT\_SMStorageVolume class

Changes the device access of the storage volume to Readable.

## Syntax


```mof
Uint32 SetReadonly(
  [in, optional]��String ���������������username,
  [in, optional]��String ���������������password,
  [out, optional]�MSFT_SMExtendedStatus ExtendedStatus
);
```



## Parameters

<dl> <dt>

*username* \[in, optional\]
</dt> <dd>

Used to authenticate with the SMI-S provider. If not provided, the storage service attempts to obtain these credentials from the configuration provider.

</dd> <dt>

*password* \[in, optional\]
</dt> <dd>

Used to authenticate with the SMI-S provider. If not provided, the storage service attempts to obtain these credentials from the configuration provider.

</dd> <dt>

*ExtendedStatus* \[out, optional\]
</dt> <dd>

An [**MSFT\_SMExtendedStatus**](msft-smextendedstatus.md) object containing the results of calling this method.

</dd> </dl>

## Return value

<dl> <dt>

**Success** (0)
</dt> <dt>

**Not Supported** (1)
</dt> <dt>

**Unspecified Error** (2)
</dt> <dt>

**Timeout** (3)
</dt> <dt>

**Failed** (4)
</dt> <dt>

**Invalid Parameter** (5)
</dt> <dt>

**Invalid logical unit ID** (4097)
</dt> <dt>

**Invalid permission** (4100)
</dt> <dt>

**StorageService: Cannot modify volume instance** (40304)
</dt> <dt>

**StorageService CIM Error: Failed** (43001)
</dt> <dt>

**StorageService CIM Error: Access denied** (43002)
</dt> <dt>

**StorageService CIM Error: Invalid namespace** (43003)
</dt> <dt>

**StorageService CIM Error: Invalid parameter** (43004)
</dt> <dt>

**StorageService CIM Error: Invalid class** (43005)
</dt> <dt>

**StorageService CIM Error: Not found** (43006)
</dt> <dt>

**StorageService CIM Error: Not supported** (43007)
</dt> <dt>

**StorageService CIM Error: Class has children** (43008)
</dt> <dt>

**StorageService CIM Error: Class has instances** (43009)
</dt> <dt>

**StorageService CIM Error: Invalid superclass** (43010)
</dt> <dt>

**StorageService CIM Error: Already exists** (43011)
</dt> <dt>

**StorageService CIM Error: No such property** (43012)
</dt> <dt>

**StorageService CIM Error: Type mismatch** (43013)
</dt> <dt>

**StorageService CIM Error: Query language not supported** (43014)
</dt> <dt>

**StorageService CIM Error: Invalid query** (43015)
</dt> <dt>

**StorageService CIM Error: Method not available** (43016)
</dt> <dt>

**StorageService CIM Error: Method not found** (43017)
</dt> <dt>

**StorageService CIM Error: Unexpected response** (43018)
</dt> <dt>

**StorageService CIM Error: Invalid response destination** (43019)
</dt> <dt>

**StorageService CIM Error: Namespace not empty** (43020)
</dt> <dt>

**StorageService CIM Error: Invalid enumeration context** (43021)
</dt> <dt>

**StorageService CIM Error: Invalid operation timeout** (43022)
</dt> <dt>

**StorageService CIM Error: Pull has been abandoned** (43023)
</dt> <dt>

**StorageService CIM Error: Pull cannot be abandoned** (43024)
</dt> <dt>

**StorageService CIM Error: Filtered enumeration not supported** (43025)
</dt> <dt>

**StorageService CIM Error: Continuation on error not supported** (43026)
</dt> <dt>

**StorageService CIM Error: Server limits exceeded** (43027)
</dt> <dt>

**StorageService CIM Error: Server is shutting down** (43028)
</dt> <dt>

**StorageService CIM Error: Query feature not supported** (43029)
</dt> <dt>

**StorageService: Generic Failure** (51000)
</dt> <dt>

**StorageService: Invalid connection credentials** (51005)
</dt> <dt>

**StorageService: SSL connection failure** (51010)
</dt> </dl>

## Requirements



|                                     |                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                     |
| Minimum supported server<br/> | Windows Server�2012<br/>                                                                |
| Namespace<br/>                | Root\\Microsoft\\Windows\\Storage\\SM<br/>                                              |
| MOF<br/>                      | <dl> <dt>MsftStrgMan.mof</dt> </dl>    |
| DLL<br/>                      | <dl> <dt>StorageService.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_SMStorageVolume**](msft-smstoragevolume.md)
</dt> </dl>

�

�




