---
title: ICLRTask2::EndPreventAsyncAbort 方法
ms.date: 03/30/2017
api_name:
- ICLRTask2.EndPreventAsyncAbort
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- ICLRTask2::EndPreventAsyncAbort
helpviewer_keywords:
- EndPreventAsyncAbort method [.NET Framework hosting]
- ICLRTask2::EndPreventAsyncAbort method [.NET Framework hosting]
ms.assetid: d8013659-e3df-44b3-814f-a6b534ce62f8
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 8cacc96d66d5d4eb46c08c93d9c2793282627539
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="iclrtask2endpreventasyncabort-method"></a>ICLRTask2::EndPreventAsyncAbort 方法
允许新的或挂起的线程中止请求导致线程中止当前线程上。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT EndPreventAsyncAbort();  
```  
  
## <a name="return-value"></a>返回值  
 此方法返回以下特定 HRESULT 以及表示方法失败的 HRESULT 错误。  
  
|HRESULT|描述|  
|-------------|-----------------|  
|S_OK|该方法已成功完成。|  
|HOST_E_INVALIDOPERATION|这不是当前线程的线程上调用了方法。|  
  
## <a name="remarks"></a>备注  
 一个与当前线程调用此方法递减延迟线程中止计数器。  
  
 调用[iclrtask2:: Beginpreventasyncabort](../../../../docs/framework/unmanaged-api/hosting/iclrtask2-beginpreventasyncabort-method.md)和`EndPreventAsyncAbort`可以嵌套。 只要计数器值大于零，当前线程的线程中止延迟。  
  
 虚拟机 (VM) 内部使用此功能公开的功能。 不正确使用了这些方法可能导致虚拟机中未指定的行为。 例如，调用`EndPreventAsyncAbort`而无需首先调用`BeginPreventAsyncAbort`VM 先前已增大时无法设置为零的计数器。 同样，内部计数器未检查存在溢出。 如果该阈值超过其整型的限制，因为它就会递增主机和 VM，获得的行为是未指定。  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** MSCorEE.h  
  
 **库：**作为 MSCorEE.dll 中的资源  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [BeginPreventAsyncAbort 方法](../../../../docs/framework/unmanaged-api/hosting/iclrtask2-beginpreventasyncabort-method.md)  
 [ICLRTask2 接口](../../../../docs/framework/unmanaged-api/hosting/iclrtask2-interface.md)  
 [ICLRTaskManager 接口](../../../../docs/framework/unmanaged-api/hosting/iclrtaskmanager-interface.md)  
 [IHostTask 接口](../../../../docs/framework/unmanaged-api/hosting/ihosttask-interface.md)  
 [IHostTaskManager 接口](../../../../docs/framework/unmanaged-api/hosting/ihosttaskmanager-interface.md)  
 [承载接口](../../../../docs/framework/unmanaged-api/hosting/hosting-interfaces.md)
