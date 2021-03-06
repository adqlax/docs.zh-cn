---
title: 使用 XML 架构
ms.date: 03/30/2017
ms.technology: dotnet-standard
ms.assetid: bbbcc70c-bf9a-4f6a-af72-1bab5384a187
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 83fddd00f44b184fa066f6c47b90b01fac7ef7bc
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="working-with-xml-schemas"></a>使用 XML 架构
要定义 XML 文档的结构及其元素关系、数据类型和内容约束，请使用文档类型定义 (DTD) 或 XML 架构定义语言 (XSD) 架构。 尽管 XML 文档如果符合万维网联合会 (W3C) 可扩展标记语言 (XML) 1.0 建议定义的所有语法要求，就被认为格式正确，但是，除非其格式正确并且符合其 DTD 或架构定义的约束，否则，不会认为该文档有效。 因此，尽管所有有效 XML 文档的格式都是正确的，但是并非所有格式正确的 XML 文档都有效。  
  
 若要详细了解 XML，请参阅 [W3C XML 1.0 建议](https://www.w3.org/TR/REC-xml/)。 若要详细了解 XML 架构，请参阅 [W3C XML 架构第 1 部分：结构建议](https://www.w3.org/TR/xmlschema-1/)和 [W3C XML 架构第 2 部分：数据类型建议](https://www.w3.org/TR/xmlschema-2/)中提供的建议。  
  
## <a name="in-this-section"></a>本节内容  
 [XML 架构对象模型 (SOM)](../../../../docs/standard/data/xml/xml-schema-object-model-som.md)  
 讨论 <xref:System.Xml.Schema?displayProperty=nameWithType> 命名空间中的架构对象模型 (SOM)，SOM 提供一组类，用于从文件读取架构定义语言 (XSD) 架构或通过编程创建内存中架构。  
  
 [用于编译架构的 XmlSchemaSet](../../../../docs/standard/data/xml/xmlschemaset-for-schema-compilation.md)  
 讨论 <xref:System.Xml.Schema.XmlSchemaSet> 类，该类是可以存储和验证 XSD 架构的缓存。  
  
 [XmlSchemaValidator 基于推送的验证](../../../../docs/standard/data/xml/xmlschemavalidator-push-based-validation.md)  
 讨论 <xref:System.Xml.Schema.XmlSchemaValidator> 类，该类提供了一种高效、高性能的机制，通过基于推送的方式针对 XSD 架构验证 XML 数据。  
  
 [推断 XML 架构](../../../../docs/standard/data/xml/inferring-an-xml-schema.md)  
 讨论如何使用 <xref:System.Xml.Schema.XmlSchemaInference> 类从 XML 文档的结构推断 XSD 架构。  
  
## <a name="reference"></a>参考  
 <xref:System.Xml.Schema.XmlSchemaSet> &#124; <xref:System.Xml.Schema.XmlSchemaInference> &#124; <xref:System.Xml.XmlReader>  
  
## <a name="related-sections"></a>相关章节  
 [在 DOM 中验证 XML 文档](../../../../docs/standard/data/xml/validating-an-xml-document-in-the-dom.md)  
 讨论如何在文档对象模型 (DOM) 中验证 XML。 可以在 XML 加载到 DOM 中时进行验证，也可以在 DOM 中验证以前未经过验证的 XML 文档。  
  
 [使用 XPathNavigator 验证架构](../../../../docs/standard/data/xml/schema-validation-using-xpathnavigator.md)  
 讨论如何验证使用 <xref:System.Xml.XPath.XPathNavigator> 类浏览和编辑的 XML。
