---
title: "CeeSectionAttr 枚举"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: CeeSectionAttr
api_location: mscoree.dll
api_type: COM
f1_keywords: CeeSectionAttr
helpviewer_keywords: CeeSectionAttr enumeration [.NET Framework metadata]
ms.assetid: 0db51881-b869-4677-a715-1726a9216489
topic_type: apiref
caps.latest.revision: "9"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 0f0c87c0e5703f13cf843ca5a4213440af71bd12
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="ceesectionattr-enumeration"></a><span data-ttu-id="b75f1-102">CeeSectionAttr 枚举</span><span class="sxs-lookup"><span data-stu-id="b75f1-102">CeeSectionAttr Enumeration</span></span>
<span data-ttu-id="b75f1-103">提供用于指定以供节特性值[ICeeGen](../../../../docs/framework/unmanaged-api/metadata/iceegen-interface.md)接口。</span><span class="sxs-lookup"><span data-stu-id="b75f1-103">Provides values that specify attributes of a section for use by the [ICeeGen](../../../../docs/framework/unmanaged-api/metadata/iceegen-interface.md) interface.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="b75f1-104">语法</span><span class="sxs-lookup"><span data-stu-id="b75f1-104">Syntax</span></span>  
  
```  
typedef enum  {  
    sdNone      = 0,  
    sdReadOnly  = IMAGE_SCN_CNT_INITIALIZED_DATA |  
                  IMAGE_SCN_MEM_READ,  
    sdReadWrite = sdReadOnly | IMAGE_SCN_MEM_WRITE,  
    sdExecute   = IMAGE_SCN_MEM_READ | IMAGE_SCN_CNT_CODE |  
                  IMAGE_SCN_MEM_EXECUTE  
} CeeSectionAttr;  
```  
  
## <a name="members"></a><span data-ttu-id="b75f1-105">成员</span><span class="sxs-lookup"><span data-stu-id="b75f1-105">Members</span></span>  
  
|<span data-ttu-id="b75f1-106">成员</span><span class="sxs-lookup"><span data-stu-id="b75f1-106">Member</span></span>|<span data-ttu-id="b75f1-107">描述</span><span class="sxs-lookup"><span data-stu-id="b75f1-107">Description</span></span>|  
|------------|-----------------|  
|`sdNone`|<span data-ttu-id="b75f1-108">部分包含任何属性。</span><span class="sxs-lookup"><span data-stu-id="b75f1-108">Section has no attributes.</span></span>|  
|`sdReadOnly`|<span data-ttu-id="b75f1-109">部分包含初始化只能读取，未更新的数据。</span><span class="sxs-lookup"><span data-stu-id="b75f1-109">Section contains initialized data that can be only read, not updated.</span></span>|  
|`sdReadWrite`|<span data-ttu-id="b75f1-110">部分包含可读取或更新的初始化的数据。</span><span class="sxs-lookup"><span data-stu-id="b75f1-110">Section contains initialized data that can be read or updated.</span></span>|  
|`sdExecute`|<span data-ttu-id="b75f1-111">部分包含允许读取和执行的可执行代码。</span><span class="sxs-lookup"><span data-stu-id="b75f1-111">Section contains executable code that is allowed to be read and executed.</span></span>|  
  
## <a name="requirements"></a><span data-ttu-id="b75f1-112">要求</span><span class="sxs-lookup"><span data-stu-id="b75f1-112">Requirements</span></span>  
 <span data-ttu-id="b75f1-113">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="b75f1-113">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="b75f1-114">**标头：** Cor.h</span><span class="sxs-lookup"><span data-stu-id="b75f1-114">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="b75f1-115">**库：**作为 MsCorEE.dll 中的资源</span><span class="sxs-lookup"><span data-stu-id="b75f1-115">**Library:** Included as a resource in MsCorEE.dll</span></span>  
  
 <span data-ttu-id="b75f1-116">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="b75f1-116">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="b75f1-117">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b75f1-117">See Also</span></span>  
 [<span data-ttu-id="b75f1-118">元数据枚举</span><span class="sxs-lookup"><span data-stu-id="b75f1-118">Metadata Enumerations</span></span>](../../../../docs/framework/unmanaged-api/metadata/metadata-enumerations.md)