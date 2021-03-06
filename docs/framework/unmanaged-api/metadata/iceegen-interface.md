---
title: ICeeGen 接口
ms.date: 03/30/2017
api_name:
- ICeeGen
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- ICeeGen
helpviewer_keywords:
- ICeeGen interface [.NET Framework metadata]
ms.assetid: 383d20b0-efe9-4e71-8fb8-1186b2e7d0c0
topic_type:
- apiref
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 0e3e70749a768377ea470bc44a66b9fdabbb1f93
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="iceegen-interface"></a>ICeeGen 接口
提供用于动态代码编译的方法。  
  
 此接口已过时，不应使用。  
  
## <a name="methods"></a>方法  
  
|方法|描述|  
|------------|-----------------|  
|[AddSectionReloc 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-addsectionreloc-method.md)|已过时。 将.reloc 指令添加到基本代码。|  
|[AllocateMethodBuffer 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-allocatemethodbuffer-method.md)|已过时。 创建方法，指定大小的缓冲区并获取该方法的相对虚拟地址。|  
|[ComputePointer 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-computepointer-method.md)|已过时。 确定指定的代码部分的缓冲区。|  
|[EmitString 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-emitstring-method.md)|已过时。 将指定的字符串发出到基本代码。|  
|[GenerateCeeFile 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-generateceefile-method.md)|已过时。 生成包含当前加载到此代码的基本代码文件`ICeeGen`。|  
|[GenerateCeeMemoryImage 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-generateceememoryimage-method.md)|已过时。 在基本代码的内存中生成的映像。|  
|[GetIlSection 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getilsection-method.md)|已过时。 获取由指定的句柄引用的基的中间语言代码的节。|  
|[GetIMapTokenIface 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getimaptokeniface-method.md)|已过时。 获取指定标记所引用的接口。|  
|[GetMethodBuffer 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getmethodbuffer-method.md)|已过时。 获取位于指定的相对虚拟地址的方法的相应大小的缓冲区。|  
|[GetSectionBlock 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getsectionblock-method.md)|已过时。 获取部分块的基本代码。|  
|[GetSectionCreate 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getsectioncreate-method.md)|已过时。 生成并获取使用指定的名称和标志值的代码节。|  
|[GetSectionDataLen 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getsectiondatalen-method.md)|已过时。 获取指定部分的长度。|  
|[GetString 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getstring-method.md)|已过时。 获取存储在指定的相对虚拟地址的字符串。|  
|[GetStringSection 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-getstringsection-method.md)|已过时。 获取由指定的句柄引用的代码部分的字符串表示形式。|  
|[TruncateSection 方法](../../../../docs/framework/unmanaged-api/metadata/iceegen-truncatesection-method.md)|已过时。 通过指定长度截断指定的代码段。|  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** Cor.h  
  
 **库：**用作 MsCorEE.dll 中的资源  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [元数据接口](../../../../docs/framework/unmanaged-api/metadata/metadata-interfaces.md)
