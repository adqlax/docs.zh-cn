---
title: 更改 XML 文档中的命名空间声明
ms.date: 03/30/2017
ms.technology: dotnet-standard
dev_langs:
- csharp
- vb
ms.assetid: a2758f40-e497-4964-8d8d-1bb68af14dcd
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 2fa41e8a4e8f5a15d789ddc81c2b94072c6f16b9
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="changing-namespace-declarations-in-an-xml-document"></a>更改 XML 文档中的命名空间声明
XmlDocument 将命名空间声明和 xmlns 属性公开为文档对象模型的一部分。 这些声明和属性存储在 XmlDocument 中，因此在可以保存文档时暂留这些属性的位置。 更改这些属性对树中现有其他节点的 Name、NamespaceURI 和 Prefix 属性没有影响。 例如，如果加载以下文档，`test` 元素包含 NamespaceURI `123.`  
  
```xml  
<test xmlns="123"/>  
```  
  
 如果删除 `xmlns` 属性（如下所示），`test` 元素仍包含 NamespaceURI `123`。  
  
```vb  
doc.documentElement.RemoveAttribute("xmlns")  
```  
  
```csharp  
doc.documentElement.RemoveAttribute("xmlns");  
```  
  
 同样，如果将不同的 `xmlns` 属性添加到 `doc` 元素（如下所示），`test` 元素仍包含 NamespaceURI `123`。  
  
```vb  
doc.documentElement.SetAttribute("xmlns","456");  
```  
  
```csharp  
doc.documentElement.SetAttribute("xmlns","456");  
```  
  
 因此，保存并重新加载 XmlDocument 对象前，更改 `xmlns` 属性不会有任何影响。  
  
## <a name="see-also"></a>请参阅  
 [XML 文档对象模型 (DOM)](../../../../docs/standard/data/xml/xml-document-object-model-dom.md)
