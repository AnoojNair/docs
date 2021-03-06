---
title: "CLRDataCreateInstance Function"
ms.date: "03/30/2017"
api_name: 
  - "CLRDataCreateInstance"
api_location: 
  - "mscordbi.dll"
  - "mscordacwks.dll"
api_type: 
  - "COM"
f1_keywords: 
  - "CLRDataCreateInstance"
helpviewer_keywords: 
  - "CLRDataCreateInstance function [.NET Framework debugging]"
ms.assetid: 440bad90-5a88-45e7-9157-4596801d8d19
topic_type: 
  - "apiref"
author: "rpetrusha"
ms.author: "ronpet"
---
# CLRDataCreateInstance Function
Creates an interface object for the specified target item.  
  
## Syntax  
  
```  
HRESULT CLRDataCreateInstance (  
    [in]  REFIID           iid,   
    [in]  ICLRDataTarget  *target,   
    [out] void           **iface  
);  
```  
  
#### Parameters  
 `iid`  
 [in] The identifier of the interface to be instantiated.  
  
 `target`  
 [in] A pointer to a user-implemented [ICLRDataTarget](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget-interface.md) object that represents the target item for which to create the interface object.  
  
 `iface`  
 [out] A pointer to the address of the returned interface object.  
  
## Remarks  
 The `ICLRDataTarget` object is implemented by the writer of the debugging application. The implementation depends on the type of target item being represented. The target item may be a process, memory dump, remote machine, and so on.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** ClrData.idl  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## See Also  
 [Debugging Global Static Functions](../../../../docs/framework/unmanaged-api/debugging/debugging-global-static-functions.md)
