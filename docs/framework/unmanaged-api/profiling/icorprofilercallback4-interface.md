---
title: "ICorProfilerCallback4 接口"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorProfilerCallback4
api_location: mscorwks.dll
api_type: COM
f1_keywords: ICorProfilerCallback4
helpviewer_keywords: ICorProfilerCallback4 interface [.NET Framework profiling]
ms.assetid: 665f3cfc-cd6f-4880-906c-ea65ad384783
topic_type: apiref
caps.latest.revision: "8"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 64a26f5dfb0ad9f06bb1b9eb31dcae36f4623c4d
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="icorprofilercallback4-interface"></a><span data-ttu-id="c255b-102">ICorProfilerCallback4 接口</span><span class="sxs-lookup"><span data-stu-id="c255b-102">ICorProfilerCallback4 Interface</span></span>
<span data-ttu-id="c255b-103">提供用于将信息传递给探查器公共语言运行时 (CLR) 的回叫方法。</span><span class="sxs-lookup"><span data-stu-id="c255b-103">Provides callback methods that the common language runtime (CLR) uses to communicate information to the profiler.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="c255b-104">方法</span><span class="sxs-lookup"><span data-stu-id="c255b-104">Methods</span></span>  
  
|<span data-ttu-id="c255b-105">方法</span><span class="sxs-lookup"><span data-stu-id="c255b-105">Method</span></span>|<span data-ttu-id="c255b-106">描述</span><span class="sxs-lookup"><span data-stu-id="c255b-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="c255b-107">GetReJITParameters 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-107">GetReJITParameters Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-getrejitparameters-method.md)|<span data-ttu-id="c255b-108">允许代码探查器设置新的重新编译的方法体的替代代码生成标志。</span><span class="sxs-lookup"><span data-stu-id="c255b-108">Allows the code profiler to set alternate code generation flags for a new recompiled method body.</span></span>|  
|[<span data-ttu-id="c255b-109">MovedReferences2 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-109">MovedReferences2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-movedreferences2-method.md)|<span data-ttu-id="c255b-110">压缩垃圾回收的结果将堆中对象的新布局报告。</span><span class="sxs-lookup"><span data-stu-id="c255b-110">Reports the new layout of objects in the heap as a result of a compacting garbage collection.</span></span>|  
|[<span data-ttu-id="c255b-111">ReJITCompilationFinished 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-111">ReJITCompilationFinished Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-rejitcompilationfinished-method.md)|<span data-ttu-id="c255b-112">通知探查器在实时 (JIT) 编译器已完成函数的重新编译。</span><span class="sxs-lookup"><span data-stu-id="c255b-112">Notifies the profiler that the just-in-time (JIT) compiler has finished the recompilation of a function.</span></span>|  
|[<span data-ttu-id="c255b-113">ReJITCompilationStarted 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-113">ReJITCompilationStarted Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-rejitcompilationstarted-method.md)|<span data-ttu-id="c255b-114">通知探查器在实时 (JIT) 编译器已开始重新编译函数。</span><span class="sxs-lookup"><span data-stu-id="c255b-114">Notifies the profiler that the just-in-time (JIT) compiler has started to recompile a function.</span></span>|  
|[<span data-ttu-id="c255b-115">ReJITError 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-115">ReJITError Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-rejiterror-method.md)|<span data-ttu-id="c255b-116">报告处理重新编译请求时遇到错误。</span><span class="sxs-lookup"><span data-stu-id="c255b-116">Reports an error encountered while processing a recompile request.</span></span>|  
|[<span data-ttu-id="c255b-117">SurvivingReferences2 方法</span><span class="sxs-lookup"><span data-stu-id="c255b-117">SurvivingReferences2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-survivingreferences2-method.md)|<span data-ttu-id="c255b-118">将堆中对象的布局报告为非压缩垃圾回收的结果。</span><span class="sxs-lookup"><span data-stu-id="c255b-118">Reports the layout of objects in the heap as a result of a non-compacting garbage collection.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="c255b-119">备注</span><span class="sxs-lookup"><span data-stu-id="c255b-119">Remarks</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="c255b-120">要求</span><span class="sxs-lookup"><span data-stu-id="c255b-120">Requirements</span></span>  
 <span data-ttu-id="c255b-121">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="c255b-121">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="c255b-122">**头文件：** CorProf.idl、CorProf.h</span><span class="sxs-lookup"><span data-stu-id="c255b-122">**Header:** CorProf.idl, CorProf.h</span></span>  
  
 <span data-ttu-id="c255b-123">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="c255b-123">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="c255b-124">**.NET framework 版本：**[!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="c255b-124">**.NET Framework Versions:** [!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="c255b-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c255b-125">See Also</span></span>  
 [<span data-ttu-id="c255b-126">ICorProfilerCallback2 接口</span><span class="sxs-lookup"><span data-stu-id="c255b-126">ICorProfilerCallback2 Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback2-interface.md)  
 [<span data-ttu-id="c255b-127">分析接口</span><span class="sxs-lookup"><span data-stu-id="c255b-127">Profiling Interfaces</span></span>](../../../../docs/framework/unmanaged-api/profiling/profiling-interfaces.md)  
 [<span data-ttu-id="c255b-128">ICorProfilerInfo 接口</span><span class="sxs-lookup"><span data-stu-id="c255b-128">ICorProfilerInfo Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo-interface.md)