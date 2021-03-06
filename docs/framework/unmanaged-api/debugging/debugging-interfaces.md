---
title: 调试接口
ms.date: 03/30/2017
helpviewer_keywords:
- unmanaged interfaces [.NET Framework], debugging
- debugging interfaces [.NET Framework]
- interfaces [.NET Framework debugging]
ms.assetid: b6297c26-7624-4431-8af4-14112d07bcd5
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 991e333c53101a2be2a8a19d3960c3d0879619be
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="debugging-interfaces"></a>调试接口
本节描述进行程序调试处理的非托管接口，所调试的程序在公共语言运行时 (CLR) 中执行。  
  
## <a name="in-this-section"></a>本节内容  
 [ICLRDataEnumMemoryRegions 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdataenummemoryregions-interface.md)  
 提供对由调用方指定的内存区域进行枚举的方法。  
  
 [ICLRDataEnumMemoryRegionsCallback 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdataenummemoryregionscallback-interface.md)  
 为 `EnumMemoryRegions` 提供一种回调方法，用于向调试器报告尝试枚举指定内存区域的结果。  
  
 [ICLRDataTarget 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget-interface.md)  
 提供与目标 CLR 进程进行交互的方法。  
  
 [ICLRDataTarget2 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget2-interface.md)  
 数据访问服务层在目标进程中操作虚拟内存区域时所用的 `ICLRDataTarget` 的子类。  
  
 [ICLRDataTarget3 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget3-interface.md)  
 一个子类[ICLRDataTarget2](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget2-interface.md) ，可提供对异常信息的访问。  
  
 [ICLRDebugging 接口](../../../../docs/framework/unmanaged-api/debugging/iclrdebugging-interface.md)  
 提供一些方法，用于处理模块的加载和卸载以进行调试。  
  
 [ICLRDebuggingLibraryProvider 方法](../../../../docs/framework/unmanaged-api/debugging/iclrdebugginglibraryprovider-interface.md)  
 包括[ProvideLibrary 方法](../../../../docs/framework/unmanaged-api/debugging/iclrdebugginglibraryprovider-providelibrary-method.md)方法，后者将获取一个库提供程序允许公共语言运行时特定于版本的调试库需要定位和加载上的回调接口。  
  
 [ICLRMetadataLocator 接口](../../../../docs/framework/unmanaged-api/debugging/iclrmetadatalocator-interface.md)  
 数据访问服务层用于在目标进程中定位程序集的元数据的接口。  
  
 [ICorDebug 接口](../../../../docs/framework/unmanaged-api/debugging/icordebug-interface.md)  
 提供允许开发人员在 CLR 环境中调试应用程序的方法。  
  
 [ICorDebugAppDomain Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain-interface.md)  
 提供用于调试应用程序域的方法。  
  
 [ICorDebugAppDomain2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain2-interface.md)  
 提供处理数组、指针、函数指针和 ByRef 类型的方法。 此接口是 `ICorDebugAppDomain` 接口的扩展。  
  
 [ICorDebugAppDomain3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain3-interface.md)  
 提供用于处理应用程序域中的 [!INCLUDE[wrt](../../../../includes/wrt-md.md)]类型的方法。 此接口是 `ICorDebugAppDomain` 和 `ICorDebugAppDomain2` 接口的扩展。  
  
 [ICorDebugAppDomain4 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain4-interface.md)  
 合理扩展[ICorDebugAppDomain](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain-interface.md)接口以从 COM 可调用包装器获取托管的对象。  
  
 [ICorDebugAppDomainEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomainenum-interface.md)  
 提供一种方法，此方法从枚举中的下一个位置开始，返回指定数目的 `ICorDebugAppDomain` 值。  
  
 [ICorDebugArrayValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugarrayvalue-interface.md)  
 表示一维或多维数组的 `ICorDebugHeapValue` 的子类。  
  
 [ICorDebugAssembly Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugassembly-interface.md)  
 表示一个程序集。  
  
 [ICorDebugAssembly2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugassembly2-interface.md)  
 表示一个程序集。 此接口是 `ICorDebugAssembly` 接口的扩展。  
  
 [ICorDebugAssembly3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugassembly3-interface.md)  
 合理扩展[ICorDebugAssembly](../../../../docs/framework/unmanaged-api/debugging/icordebugassembly-interface.md)接口，从而为容器程序集及其包含的程序集提供支持。 **在仅.NET Native 上可用。**  
  
 [ICorDebugAssemblyEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugassemblyenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugAssembly` 数组。  
  
 [ICorDebugBlockingObjectEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugblockingobjectenum-interface.md)  
 有关的列表中提供的枚举器[CorDebugBlockingObject](../../../../docs/framework/unmanaged-api/debugging/cordebugblockingobject-structure.md)结构。  
  
 [ICorDebugBoxValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugboxvalue-interface.md)  
 表示装箱的值类对象的 `ICorDebugHeapValue` 的子类。  
  
 [ICorDebugBreakpoint Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugbreakpoint-interface.md)  
 表示函数中的断点，或值的观察点。  
  
 [ICorDebugBreakpointEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugbreakpointenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugBreakpoint` 数组。  
  
 [ICorDebugChain Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugchain-interface.md)  
 表示一个物理或逻辑调用堆栈段。  
  
 [ICorDebugChainEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugchainenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugChain` 数组。  
  
 [ICorDebugClass Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugclass-interface.md)  
 表示基类型或复杂类型（即用户定义的类型）。 如果该类型为泛型类型，则 `ICorDebugClass` 表示实例化的泛型类型。  
  
 [ICorDebugClass2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugclass2-interface.md)  
 表示泛型类或具有 <xref:System.Type> 类型的方法参数的类。 此接口扩展了 `ICorDebugClass`。  
  
 [ICorDebugCode Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugcode-interface1.md)  
 表示 Microsoft 中间语言 (MSIL) 代码段或本机代码段。  
  
 [ICorDebugCode2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugcode2-interface.md)  
 提供扩展 `ICorDebugCode` 的功能的方法。  
  
 [ICorDebugCode3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugcode3-interface.md)  
 提供的扩展的方法[ICorDebugCode](../../../../docs/framework/unmanaged-api/debugging/icordebugcode-interface1.md)和[ICorDebugCode2](../../../../docs/framework/unmanaged-api/debugging/icordebugcode2-interface.md)以提供有关托管返回值的信息。  
  
 [ICorDebugCode4 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugcode4-interface.md)  
 提供使调试器能够枚举的本地变量和函数中的自变量的方法。  
  
 [ICorDebugCodeEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugcodeenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugCode` 数组。  
  
 [ICorDebugComObjectValue 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugcomobjectvalue-interface.md)  
 提供用来检索缓存的接口对象的方法。  
  
 [ICorDebugContext Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugcontext-interface.md)  
 表示一个上下文对象。 此接口尚未实现。  
  
 [ICorDebugController Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugcontroller-interface.md)  
 表示可以控制代码执行上下文的 <xref:System.Diagnostics.Process> 或 <xref:System.AppDomain> 范围。  
  
 [ICorDebugDataTarget 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget-interface.md)  
 提供一个回调接口，该接口可提供对特定目标进程的访问。  
  
 [ICorDebugDataTarget2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget2-interface.md)  
 合理扩展[ICorDebugDataTarget](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget-interface.md)接口。 **在仅.NET Native 上可用。**  
  
 [ICorDebugDataTarget3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget3-interface.md)  
 合理扩展[ICorDebugDataTarget](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget-interface.md)接口以提供有关已加载模块的信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugDebugEvent 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugdebugevent-interface.md)  
 定义所有 `ICorDebug` 调试事件派生的基接口。 **在仅.NET Native 上可用。**  
  
 [ICorDebugEditAndContinueErrorInfo 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugeditandcontinueerrorinfo-interface.md)  
 已过时。 不要使用此接口。  
  
 [ICorDebugEditAndContinueSnapshot Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugeditandcontinuesnapshot-interface.md)  
 已过时。 不要使用此接口。  
  
 [ICorDebugEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugenum-interface1.md)  
 作为调试枚举器的抽象基接口。  
  
 [ICorDebugErrorInfoEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugerrorinfoenum-interface.md)  
 已过时。 不要使用此接口。  
  
 [ICorDebugEval Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugeval-interface.md)  
 提供使调试器能够在正在调试的代码的上下文中执行代码的方法。  
  
 [ICorDebugEval2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugeval2-interface.md)  
 扩展 `ICorDebugEval` 以对泛型类型提供支持。  
  
 [ICorDebugExceptionDebugEvent 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugexceptiondebugevent-interface.md)  
 扩展[icor 调试调试事件](../../../../docs/framework/unmanaged-api/debugging/icordebugdebugevent-interface.md)接口以支持异常事件。 **在仅.NET Native 上可用。**  
  
 [ICorDebugExceptionObjectCallStackEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugexceptionobjectcallstackenum-interface.md)  
 为嵌入在异常对象中的调用堆栈信息提供枚举器。  
  
 [ICorDebugExceptionObjectValue 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugexceptionobjectvalue-interface.md)  
 扩展[ICorDebugObjectValue](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-interface.md)接口以提供来自托管的异常对象的堆栈跟踪信息。  
  
 [ICorDebugFrame Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugframe-interface.md)  
 表示当前堆栈上的帧。  
  
 [ICorDebugFrameEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugframeenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugFrame` 数组。  
  
 [ICorDebugFunction Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugfunction-interface1.md)  
 表示一个托管函数或方法。  
  
 [ICorDebugFunction2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugfunction2-interface.md)  
 对 `ICorDebugFunction` 进行逻辑扩展，以支持“仅我的代码”的单步执行调试。  
  
 [ICorDebugFunction3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugfunction3-interface.md)  
 合理扩展[ICorDebugFunction](../../../../docs/framework/unmanaged-api/debugging/icordebugfunction-interface1.md)接口以提供对代码的访问，ReJIT 请求中。  
  
 [ICorDebugFunctionBreakpoint Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugfunctionbreakpoint-interface.md)  
 扩展 `ICorDebugBreakpoint` 以支持函数中的断点。  
  
 [ICorDebugGCReferenceEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebuggcreferenceenum-interface.md)  
 提供针对将进行垃圾回收的对象的枚举器。  
  
 [ICorDebugGenericValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebuggenericvalue-interface.md)  
 应用于所有值的 `ICorDebugValue` 的子类。 此接口可为值提供 Get 和 Set 方法。  
  
 [ICorDebugGuidToTypeEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugguidtotypeenum-interface.md)  
 提供针对映射 GUID 的对象及其相应的 `ICorDebugType` 对象的枚举器。  
  
 [ICorDebugHandleValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebughandlevalue-interface.md)  
 `ICorDebugReferenceValue` 的一个子类，前者表示调试器已为其创建了垃圾回收句柄的引用值。  
  
 [ICorDebugHeapEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugheapenum-interface.md)  
 提供针对托管堆上的对象的枚举器。  
  
 [ICorDebugHeapSegmentEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugheapsegmentenum-interface.md)  
 提供针对托管堆的内存区域的枚举器。  
  
 [ICorDebugHeapValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugheapvalue-interface.md)  
 表示 CLR 垃圾回收器已收集的对象的 `ICorDebugValue` 的子类。  
  
 [ICorDebugHeapValue2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugheapvalue2-interface1.md)  
 对运行时句柄提供支持的 `ICorDebugHeapValue` 的扩展。  
  
 [ICorDebugHeapValue3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugheapvalue3-interface.md)  
 公开对象的监视器锁属性。  
  
 [ICorDebugILCode 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugilcode-interface.md)  
 表示中间语言 (IL) 代码段。  
  
 [ICorDebugILCode2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugilcode2-interface.md)  
 合理扩展[ICorDebugILCode](../../../../docs/framework/unmanaged-api/debugging/icordebugilcode-interface.md)接口，以提供的方法，返回的标记的函数的局部变量签名，并将探查器检测到的中间语言 (IL) 偏移量到原始方法的 IL偏移量。  
  
 [ICorDebugILFrame Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugilframe-interface.md)  
 表示 MSIL 代码的堆栈帧。  
  
 [ICorDebugILFrame2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugilframe2-interface.md)  
 `ICorDebugILFrame` 的逻辑扩展。  
  
 [ICorDebugILFrame3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugilframe3-interface.md)  
 提供用于封装函数的返回值的方法。  
  
 [ICorDebugILFrame4 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugilframe4-interface.md)  
 提供使你能够访问中间语言 (IL) 代码的堆栈帧中的局部变量和代码的方法。 一个用于指定调试器是否可以访问在探查器 ReJIT 检测中添加的变量和代码的参数。  
  
 [ICorDebugInstanceFieldSymbol 接口](../../../../docs/framework/unmanaged-api/debugging/icordebuginstancefieldsymbol-interface.md)  
 表示某一实例字段的调试符号信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugInternalFrame Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe-interface.md)  
 标识调试器的帧类型。  
  
 [ICorDebugInternalFrame2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe2-interface.md)  
 提供有关内部帧，包括堆栈地址和相对于位置的信息[ICorDebugFrame](../../../../docs/framework/unmanaged-api/debugging/icordebugframe-interface.md)对象。  
  
 [ICorDebugLoadedModule 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugloadedmodule-interface.md)  
 提供有关已加载模块的信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugManagedCallback 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback-interface.md)  
 提供用于处理调试器回调的方法。  
  
 [ICorDebugManagedCallback2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback2-interface.md)  
 提供支持调试器异常处理和托管调试助手 (MDA) 的方法。 `ICorDebugManagedCallback2` 是 `ICorDebugManagedCallback` 的逻辑扩展。  
  
 [ICorDebugManagedCallback3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback3-interface.md)  
 提供一个回调方法，该方法指示已发出启用的自定义调试器通知。  
  
 [ICorDebugMDA 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmda-interface.md)  
 表示托管调试助手 (MDA) 消息。  
  
 [ICorDebugMemoryBuffer 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmemorybuffer-interface.md)  
 表示内存中缓冲区。 **在仅.NET Native 上可用。**  
  
 [ICorDebugMergedAssemblyRecord 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmergedassemblyrecord-interface.md)  
 提供有关合并的程序集的信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugMetaDataLocator 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmetadatalocator-interface.md)  
 向调试器提供元数据信息。  
  
 [ICorDebugModule Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugmodule-interface.md)  
 表示 CLR 模块，它是可执行文件或动态链接库 (DLL)。  
  
 [ICorDebugModule2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugmodule2-interface.md)  
 用作 `ICorDebugModule` 的逻辑扩展。  
  
 [ICorDebugModule3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmodule3-interface.md)  
 为动态模块创建符号读取器。  
  
 [ICorDebugModuleBreakpoint Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugmodulebreakpoint-interface.md)  
 扩展 `ICorDebugBreakpoint` 以提供对特定模块的访问。  
  
 [ICorDebugModuleDebugEvent 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmoduledebugevent-interface.md)  
 扩展[icor 调试调试事件](../../../../docs/framework/unmanaged-api/debugging/icordebugdebugevent-interface.md)接口以支持模块级事件。 **在仅.NET Native 上可用。**  
  
 [ICorDebugModuleEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugmoduleenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugModule` 数组。  
  
 [ICorDebugMutableDataTarget 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugmutabledatatarget-interface.md)  
 扩展[ICorDebugDataTarget](../../../../docs/framework/unmanaged-api/debugging/icordebugdatatarget-interface.md)接口以支持可变数据目标。  
  
 [ICorDebugNativeFrame Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugnativeframe-interface.md)  
 用于本机帧的 `ICorDebugFrame` 的专用实现。  
  
 [ICorDebugNativeFrame2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugnativeframe2-interface.md)  
 提供用于测试子帧与父帧关系的方法。  
  
 [ICorDebugObjectEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并通过对象数组的相对虚拟地址 (RVA) 对其进行枚举。  
  
 [ICorDebugObjectValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-interface.md)  
 表示包含对象的值的 `ICorDebugValue` 的子类。  
  
 [ICorDebugObjectValue2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue2-interface.md)  
 扩展 `ICorDebugObjectValue` 以支持继承和重写。  
  
 [ICorDebugProcess Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess-interface.md)  
 表示正在执行托管代码的进程。  
  
 [ICorDebugProcess2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess2-interface1.md)  
 `ICorDebugProcess` 的逻辑扩展。  
  
 [ICorDebugProcess3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess3-interface.md)  
 控制自定义调试器通知。  
  
 [ICorDebugProcess5 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess5-interface.md)  
 扩展[ICorDebugProcess](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess-interface.md)接口以支持对托管堆，提供有关垃圾回收的托管对象的信息并确定调试器是否从应用程序加载映像的访问的本地本机映像缓存中。  
  
 [ICorDebugProcess6 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess6-interface.md)  
 合理扩展[ICorDebugProcess](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess-interface.md)接口以启用解码托管的调试事件的编码在本机异常调试事件和虚拟模块拆分等功能。 **在仅.NET Native 上可用。**  
  
 [ICorDebugProcess7 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess7-interface.md)  
 提供了一种方法，用于配置调试器以处理目标进程中的内存中元数据更新。  
  
 [ICorDebugProcess8 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess8-interface.md)  
 合理扩展[ICorDebugProcess](../../../../docs/framework/unmanaged-api/debugging/icordebugprocess-interface.md)接口以启用或禁用某些类型的[ICorDebugManagedCallback2](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback2-interface.md)异常回调。  
  
 [ICorDebugProcessEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugprocessenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugProcess` 数组。  
  
 [ICorDebugReferenceValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugreferencevalue-interface.md)  
 `ICorDebugValue` 的子类，它支持引用类型。  
  
 [ICorDebugRegisterSet 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset-interface.md)  
 表示在当前正在执行代码的计算机上可用的寄存器组。  
  
 [ICorDebugRegisterSet2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset2-interface.md)  
 为具有 64 个以上寄存器的硬件平台扩展 `ICorDebugRegisterSet` 的功能。  
  
 [ICorDebugRemote 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugremote-interface.md)  
 提供启动托管调试器或将其附加到远程目标进程的能力。  
  
 [ICorDebugRemoteTarget 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugremotetarget-interface.md)  
 提供使你能够在 CLR 环境中调试基于 Silverlight 的应用程序的方法。  
  
 [ICorDebugRuntimeUnwindableFrame 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugruntimeunwindableframe-interface.md)  
 提供对非托管方法的支持，这些方法需要公共语言运行时 (CLR) 来展开帧。  
  
 [ICorDebugStackWalk 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugstackwalk-interface.md)  
 提供用于获取线程堆栈上的托管方法或帧的方法。  
  
 [ICorDebugStaticFieldSymbol 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugstaticfieldsymbol-interface.md)  
 表示某个静态字段的调试符号信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugStepper Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugstepper-interface.md)  
 表示在代码执行过程中由调试器执行的一个步骤。此步骤作为命令颁发和完成之间的标识符使用，可以实现取消对某个步骤的执行。  
  
 [ICorDebugStepper2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugstepper2-interface1.md)  
 提供对“仅我的代码”(JMC) 调试的支持。  
  
 [ICorDebugStepperEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugstepperenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugStepper` 数组。  
  
 [ICorDebugStringValue Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugstringvalue-interface.md)  
 应用于字符串值的 `ICorDebugHeapValue` 的子类。  
  
 [ICorDebugSymbolProvider 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugsymbolprovider-interface.md)  
 提供可用于检索调试符号信息的方法。 **在仅.NET Native 上可用。**  
  
 [ICorDebugSymbolProvider2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugsymbolprovider2-interface.md)  
 合理扩展[ICorDebugSymbolProvider](../../../../docs/framework/unmanaged-api/debugging/icordebugsymbolprovider-interface.md)接口以检索其他调试符号信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugThread Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugthread-interface.md)  
 表示进程中的线程。 `ICorDebugThread` 实例的生存期与它表示的线程的生存期相同。  
  
 [ICorDebugThread2 Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugthread2-interface.md)  
 用作 `ICorDebugThread` 的逻辑扩展。  
  
 [ICorDebugThread3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugthread3-interface.md)  
 提供的入口点[ICorDebugStackWalk](../../../../docs/framework/unmanaged-api/debugging/icordebugstackwalk-interface.md)和相应接口。  
  
 [ICorDebugThread4 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugthread4-interface.md)  
 提供线程阻塞信息。  
  
 [ICorDebugThreadEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugthreadenum-interface1.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugThread` 数组。  
  
 [ICorDebugType Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugtype-interface.md)  
 表示基类型或复杂类型（即用户定义的类型）。 如果该类型是泛型类型，则 `ICorDebugType` 表示未实例化的泛型类型。  
  
 [ICorDebugType2 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugtype2-interface.md)  
 扩展[ICorDebugType](../../../../docs/framework/unmanaged-api/debugging/icordebugtype-interface.md)接口以检索的基类型或复杂 （用户定义的） 类型的类型标识符。  
  
 [ICorDebugTypeEnum Interface1](../../../../docs/framework/unmanaged-api/debugging/icordebugtypeenum-interface.md)  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugType` 数组。  
  
 [ICorDebugUnmanagedCallback 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugunmanagedcallback-interface.md)  
 提供与 CLR 没有直接关系的本机事件的通知。  
  
 "ICorDebugValue"  
 表示正在调试的进程中的读取或写入值。  
  
 "ICorDebugValue2"  
 扩展 `ICorDebugValue` 以提供对 `ICorDebugType` 的支持。  
  
 [ICorDebugValue3 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugvalue3-interface.md)  
 扩展"ICorDebugValue"和"ICorDebugValue2"接口，以支持大于 2 GB 的数组。  
  
 "ICorDebugValueBreakpoint"  
 扩展 `ICorDebugBreakpoint` 以提供对特定值的访问。  
  
 "ICorDebugValueEnum"  
 实现 `ICorDebugEnum` 方法，并枚举 `ICorDebugValue` 数组。  
  
 [ICorDebugVariableHome 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugvariablehome-interface.md)  
 表示本地变量或函数参数。  
  
 [ICorDebugVariableHomeEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugvariablehomeenum-interface.md)  
 提供对本地变量和函数中的参数的枚举器。  
  
 [ICorDebugVariableSymbol 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugvariablesymbol-interface.md)  
 检索变量的调试符号信息。 **在仅.NET Native 上可用。**  
  
 [ICorDebugVirtualUnwinder 接口](../../../../docs/framework/unmanaged-api/debugging/icordebugvirtualunwinder-interface.md)  
 提供帮助堆栈展开的方法。 **在仅.NET Native 上可用。**  
  
 [ICorPublish 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublish-interface.md)  
 用作发布进程的常规接口。  
  
 [ICorPublishAppDomain 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublishappdomain-interface.md)  
 表示并提供关于应用程序域的信息。  
  
 [ICorPublishAppDomainEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublishappdomainenum-interface.md)  
 提供遍历进程中当前存在的 `ICorPublishAppDomain` 对象的集合的方法。  
  
 [ICorPublishEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublishenum-interface.md)  
 用作发布枚举器的抽象基。  
  
 [ICorPublishProcess 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublishprocess-interface.md)  
 提供用于访问有关进程的信息的方法。  
  
 [ICorPublishProcessEnum 接口](../../../../docs/framework/unmanaged-api/debugging/icorpublishprocessenum-interface.md)  
 提供遍历 `ICorPublishProcess` 对象的集合的方法。  
  
## <a name="related-sections"></a>相关章节  
 [调试组件类](../../../../docs/framework/unmanaged-api/debugging/debugging-coclasses.md)  
  
 [调试全局静态函数](../../../../docs/framework/unmanaged-api/debugging/debugging-global-static-functions.md)  
  
 [调试枚举](../../../../docs/framework/unmanaged-api/debugging/debugging-enumerations.md)  
  
 [调试结构](../../../../docs/framework/unmanaged-api/debugging/debugging-structures.md)
