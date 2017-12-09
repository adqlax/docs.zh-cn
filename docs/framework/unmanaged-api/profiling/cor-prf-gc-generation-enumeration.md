---
title: "COR_PRF_GC_GENERATION 枚举"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: COR_PRF_GC_GENERATION
api_location: mscorwks.dll
api_type: COM
f1_keywords: COR_PRF_GC_GENERATION
helpviewer_keywords: COR_GC_GENERATION_FLAGS enumeration [.NET Framework profiling]
ms.assetid: d6ece160-26ad-4d39-abd7-05acd6f78c48
topic_type: apiref
caps.latest.revision: "10"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: a296dd333579f9d0e734b7c00a8adb648605295d
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="corprfgcgeneration-enumeration"></a><span data-ttu-id="6a32f-102">COR_PRF_GC_GENERATION 枚举</span><span class="sxs-lookup"><span data-stu-id="6a32f-102">COR_PRF_GC_GENERATION Enumeration</span></span>
<span data-ttu-id="6a32f-103">标识垃圾回收生成。</span><span class="sxs-lookup"><span data-stu-id="6a32f-103">Identifies a garbage-collection generation.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="6a32f-104">语法</span><span class="sxs-lookup"><span data-stu-id="6a32f-104">Syntax</span></span>  
  
```  
typedef enum {  
    COR_PRF_GC_GEN_0 = 0,  
    COR_PRF_GC_GEN_1 = 1,  
    COR_PRF_GC_GEN_2 = 2,  
    COR_PRF_GC_LARGE_OBJECT_HEAP = 3  
} COR_PRF_GC_GENERATION;  
```  
  
## <a name="members"></a><span data-ttu-id="6a32f-105">成员</span><span class="sxs-lookup"><span data-stu-id="6a32f-105">Members</span></span>  
  
|<span data-ttu-id="6a32f-106">成员</span><span class="sxs-lookup"><span data-stu-id="6a32f-106">Member</span></span>|<span data-ttu-id="6a32f-107">描述</span><span class="sxs-lookup"><span data-stu-id="6a32f-107">Description</span></span>|  
|------------|-----------------|  
|`COR_PRF_GC_GEN_0`|<span data-ttu-id="6a32f-108">为第 0 代存储对象。</span><span class="sxs-lookup"><span data-stu-id="6a32f-108">The object is stored as generation 0.</span></span>|  
|`COR_PRF_GC_GEN_1`|<span data-ttu-id="6a32f-109">为第 1 代存储对象。</span><span class="sxs-lookup"><span data-stu-id="6a32f-109">The object is stored as generation 1.</span></span>|  
|`COR_PRF_GC_GEN_2`|<span data-ttu-id="6a32f-110">作为第 2 代存储对象。</span><span class="sxs-lookup"><span data-stu-id="6a32f-110">The object is stored as generation 2.</span></span>|  
|`COR_PRF_GC_LARGE_OBJECT_HEAP`|<span data-ttu-id="6a32f-111">大型对象堆中存储对象。</span><span class="sxs-lookup"><span data-stu-id="6a32f-111">The object is stored in the large-object heap.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="6a32f-112">备注</span><span class="sxs-lookup"><span data-stu-id="6a32f-112">Remarks</span></span>  
 <span data-ttu-id="6a32f-113">垃圾回收器内存管理性能提高将对象划分为不同的代根据存在时间。</span><span class="sxs-lookup"><span data-stu-id="6a32f-113">The garbage collector improves memory management performance by dividing objects into generations based on age.</span></span> <span data-ttu-id="6a32f-114">垃圾回收器当前正在使用三代，编号为 0、 1 和 2，以及用于大型对象的特殊堆段。</span><span class="sxs-lookup"><span data-stu-id="6a32f-114">The garbage collector currently uses three generations, numbered 0, 1, and 2, plus a special heap segment that is used for large objects.</span></span> <span data-ttu-id="6a32f-115">其大小大于特定值的对象存储在大型对象堆。</span><span class="sxs-lookup"><span data-stu-id="6a32f-115">Objects whose size is larger than a particular value are stored in the large-object heap.</span></span> <span data-ttu-id="6a32f-116">其他分配的对象都属于第 0 代。</span><span class="sxs-lookup"><span data-stu-id="6a32f-116">Other allocated objects start out belonging to generation 0.</span></span> <span data-ttu-id="6a32f-117">第 0 代中发生了垃圾回收后存在的所有对象将被都提升到第 1 代中。</span><span class="sxs-lookup"><span data-stu-id="6a32f-117">All objects that exist after garbage collection occurs in generation 0 are promoted to generation 1.</span></span> <span data-ttu-id="6a32f-118">第 1 代中发生了垃圾回收后存在的对象将移到第 2 代。</span><span class="sxs-lookup"><span data-stu-id="6a32f-118">Objects that exist after garbage collection occurs in generation 1 move into generation 2.</span></span>  
  
 <span data-ttu-id="6a32f-119">代意味着垃圾回收器必须使用分配的对象的一个子集在任何时候使用。</span><span class="sxs-lookup"><span data-stu-id="6a32f-119">The use of generations means that the garbage collector has to work with only a subset of the allocated objects at any one time.</span></span>  
  
 <span data-ttu-id="6a32f-120">`COR_PRF_GC_GENERATION`枚举由[COR_PRF_GC_GENERATION_RANGE](../../../../docs/framework/unmanaged-api/profiling/cor-prf-gc-generation-range-structure.md)结构。</span><span class="sxs-lookup"><span data-stu-id="6a32f-120">The `COR_PRF_GC_GENERATION` enumeration is used by the [COR_PRF_GC_GENERATION_RANGE](../../../../docs/framework/unmanaged-api/profiling/cor-prf-gc-generation-range-structure.md) structure.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="6a32f-121">要求</span><span class="sxs-lookup"><span data-stu-id="6a32f-121">Requirements</span></span>  
 <span data-ttu-id="6a32f-122">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="6a32f-122">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="6a32f-123">**头文件：** CorProf.idl、CorProf.h</span><span class="sxs-lookup"><span data-stu-id="6a32f-123">**Header:** CorProf.idl, CorProf.h</span></span>  
  
 <span data-ttu-id="6a32f-124">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="6a32f-124">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="6a32f-125">**.NET framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="6a32f-125">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="6a32f-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6a32f-126">See Also</span></span>  
 [<span data-ttu-id="6a32f-127">分析枚举</span><span class="sxs-lookup"><span data-stu-id="6a32f-127">Profiling Enumerations</span></span>](../../../../docs/framework/unmanaged-api/profiling/profiling-enumerations.md)