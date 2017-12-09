---
title: "IMetaDataEmit::DefineNestedType 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IMetaDataEmit.DefineNestedType
api_location: mscoree.dll
api_type: COM
f1_keywords: IMetaDataEmit::DefineNestedType
helpviewer_keywords:
- IMetaDataEmit::DefineNestedType method [.NET Framework metadata]
- DefineNestedType method [.NET Framework metadata]
ms.assetid: 1e994de6-4628-459c-b967-b34be1e9fe4f
topic_type: apiref
caps.latest.revision: "11"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: bf0357275b0ad2dd7d57a3b3f07e17dc3e38e1a1
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="imetadataemitdefinenestedtype-method"></a><span data-ttu-id="60745-102">IMetaDataEmit::DefineNestedType 方法</span><span class="sxs-lookup"><span data-stu-id="60745-102">IMetaDataEmit::DefineNestedType Method</span></span>
<span data-ttu-id="60745-103">创建类型定义的元数据签名，则返回`mdTypeDef`令牌对于该类型，并指定已定义的类型是所引用的类型的成员`tdEncloser`参数。</span><span class="sxs-lookup"><span data-stu-id="60745-103">Creates the metadata signature of a type definition, returns an `mdTypeDef` token for that type, and specifies that the defined type is a member of the type referenced by the `tdEncloser` parameter.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="60745-104">语法</span><span class="sxs-lookup"><span data-stu-id="60745-104">Syntax</span></span>  
  
```  
HRESULT DefineNestedType (   
    [in]  LPCWSTR     szTypeDef,  
    [in]  DWORD       dwTypeDefFlags,   
    [in]  mdToken     tkExtends,   
    [in]  mdToken     rtkImplements[],   
    [in]  mdTypeDef   tdEncloser,   
    [out] mdTypeDef   *ptd  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="60745-105">参数</span><span class="sxs-lookup"><span data-stu-id="60745-105">Parameters</span></span>  
 `szTypeDef`  
 <span data-ttu-id="60745-106">[in]以 Unicode 类型的名称。</span><span class="sxs-lookup"><span data-stu-id="60745-106">[in] The name of the type in Unicode.</span></span>  
  
 `dwTypeDefFlags`  
 <span data-ttu-id="60745-107">[in]`TypeDef`属性。</span><span class="sxs-lookup"><span data-stu-id="60745-107">[in] `TypeDef` attributes.</span></span> <span data-ttu-id="60745-108">这是一个位掩码的`CorTypeAttr`值。</span><span class="sxs-lookup"><span data-stu-id="60745-108">This is a bitmask of `CorTypeAttr` values.</span></span>  
  
 `tkExtends`  
 <span data-ttu-id="60745-109">[in]基本类的标记。</span><span class="sxs-lookup"><span data-stu-id="60745-109">[in] The token of the base class.</span></span> <span data-ttu-id="60745-110">这可以是`mdTypeDef`或`mdTypeRef`令牌。</span><span class="sxs-lookup"><span data-stu-id="60745-110">This is either a `mdTypeDef` or a `mdTypeRef` token.</span></span>  
  
 <span data-ttu-id="60745-111">`rtkImplements`[]</span><span class="sxs-lookup"><span data-stu-id="60745-111">`rtkImplements`[]</span></span>  
 <span data-ttu-id="60745-112">[in]指定此类或接口实现的接口的令牌的数组。</span><span class="sxs-lookup"><span data-stu-id="60745-112">[in] An array of tokens that specify the interfaces that this class or interface implements.</span></span>  
  
 `tdEncloser`  
 <span data-ttu-id="60745-113">[in]封闭类型的标记。</span><span class="sxs-lookup"><span data-stu-id="60745-113">[in] The token of the enclosing type.</span></span> <span data-ttu-id="60745-114">数组的最后一个元素必须是`mdTokenNil`。</span><span class="sxs-lookup"><span data-stu-id="60745-114">The last element of the array must be `mdTokenNil`.</span></span>  
  
 `ptd`  
 <span data-ttu-id="60745-115">[out]`mdTypeDef`分配的令牌。</span><span class="sxs-lookup"><span data-stu-id="60745-115">[out] The `mdTypeDef` token assigned.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="60745-116">要求</span><span class="sxs-lookup"><span data-stu-id="60745-116">Requirements</span></span>  
 <span data-ttu-id="60745-117">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="60745-117">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="60745-118">**标头：** Cor.h</span><span class="sxs-lookup"><span data-stu-id="60745-118">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="60745-119">**库：**用作 MSCorEE.dll 中的资源</span><span class="sxs-lookup"><span data-stu-id="60745-119">**Library:** Used as a resource in MSCorEE.dll</span></span>  
  
 <span data-ttu-id="60745-120">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="60745-120">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="60745-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="60745-121">See Also</span></span>  
 [<span data-ttu-id="60745-122">IMetaDataEmit 接口</span><span class="sxs-lookup"><span data-stu-id="60745-122">IMetaDataEmit Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataemit-interface.md)  
 [<span data-ttu-id="60745-123">IMetaDataEmit2 接口</span><span class="sxs-lookup"><span data-stu-id="60745-123">IMetaDataEmit2 Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataemit2-interface.md)