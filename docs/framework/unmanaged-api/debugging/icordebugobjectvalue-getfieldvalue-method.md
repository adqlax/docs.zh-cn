---
title: ICorDebugObjectValue::GetFieldValue 方法
ms.date: 03/30/2017
api_name:
- ICorDebugObjectValue.GetFieldValue
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugObjectValue::GetFieldValue
helpviewer_keywords:
- ICorDebugObjectValue::GetFieldValue method [.NET Framework debugging]
- GetFieldValue method [.NET Framework debugging]
ms.assetid: c96770b0-3e09-47bb-bd29-20353b043459
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 230666cefdadd56465fac35222500ad4b6da67e3
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="icordebugobjectvaluegetfieldvalue-method"></a>ICorDebugObjectValue::GetFieldValue 方法
获取此对象值的指定类的指定字段的值。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT GetFieldValue (  
    [in]  ICorDebugClass     *pClass,  
    [in]  mdFieldDef         fieldDef,  
    [out] ICorDebugValue     **ppValue  
);  
```  
  
#### <a name="parameters"></a>参数  
 `pClass`  
 [in]指向一个表示要为其获取字段值的类的"ICorDebugClass"对象的指针。  
  
 `fieldDef`  
 [in]`mdFieldDef`引用描述字段的元数据的令牌。  
  
 `ppValue`  
 [out]指向一个表示指定的字段的值的"ICorDebugValue"对象的指针。  
  
## <a name="remarks"></a>备注  
 在指定的类`pClass`对象值的类的层次结构中必须是参数，并且该字段必须为该类的字段。  
  
 `GetFieldValue`方法为泛型对象和泛型类仍会成功。 例如，如果 MyDictionary\<V > 继承自字典\<字符串，V >，并且对象值的类型 MyDictionary\<int32 >，并传递`ICorDebugClass`字典的对象\<K，V > 将已成功获取字典中的字段\<字符串、 int32 >。  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CorDebug.idl、 CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
    
 
