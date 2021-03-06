---
title: XML 文本概述 (Visual Basic)
ms.date: 07/20/2015
helpviewer_keywords:
- XML literals [Visual Basic], about XML literals
- declaring XML literals [Visual Basic]
- LINQ to XML [Visual Basic], XML literals
- literals [Visual Basic], XML
ms.assetid: 37987c15-4ab8-471b-bd45-399816bfb57f
ms.openlocfilehash: 03fc8c11b5553c9c3a63bdcb69bf6135050e2c89
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="xml-literals-overview-visual-basic"></a>XML 文本概述 (Visual Basic)
*XML 文本*，可将 XML 直接合并到 Visual Basic 代码。 XML 文本语法表示[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]对象，也是如此相似的 XML 1.0 语法。 这样会更容易，以编程方式创建 XML 元素和文档，因为你的代码具有相同的结构与最终的 XML。  
  
 Visual Basic 编译到的 XML 文本[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]对象。 [!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)] 提供用于创建和操作 XML，简单对象模型和此模型完美集成[!INCLUDE[vbteclinqext](~/includes/vbteclinqext-md.md)]。 有关详细信息，请参阅<xref:System.Xml.Linq.XElement>。  
  
 你可以在 XML 文本中嵌入的 Visual Basic 表达式。 在运行时，应用程序创建[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]合并嵌入表达式的值的每个文本的对象。 这允许您指定 XML 文本中的动态内容。 有关详细信息，请参阅[XML 中的嵌入式表达式](../../../../visual-basic/programming-guide/language-features/xml/embedded-expressions-in-xml.md)。  
  
 有关 XML 文本语法和 XML 1.0 语法之间的差异的详细信息，请参阅[XML 文本和 XML 1.0 规范](../../../../visual-basic/programming-guide/language-features/xml/xml-literals-and-the-xml-1-0-specification.md)。  
  
## <a name="simple-literals"></a>简单的文本  
 你可以创建[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]通过键入或粘贴中有效的 XML 在 Visual Basic 代码中的对象。 XML 元素文本返回<xref:System.Xml.Linq.XElement>对象。 有关详细信息，请参阅[XML 元素文本](../../../../visual-basic/language-reference/xml-literals/xml-element-literal.md)和[XML 文本和 XML 1.0 规范](../../../../visual-basic/programming-guide/language-features/xml/xml-literals-and-the-xml-1-0-specification.md)。 下面的示例创建具有多个子元素的 XML 元素。  
  
 [!code-vb[VbXMLSamples#5](../../../../visual-basic/language-reference/operators/codesnippet/VisualBasic/xml-literals-overview_1.vb)]  
  
 你可以通过启动 XML 文本与在创建 XML 文档`<?xml version="1.0"?>`，下面的示例中所示。 XML 文档文本返回<xref:System.Xml.Linq.XDocument>对象。 有关详细信息，请参阅[XML 文档文本](../../../../visual-basic/language-reference/xml-literals/xml-document-literal.md)。  
  
 [!code-vb[VbXMLSamples#6](../../../../visual-basic/language-reference/operators/codesnippet/VisualBasic/xml-literals-overview_2.vb)]  
  
> [!NOTE]
>  在 Visual Basic 中的 XML 文本语法并不完全相同的 XML 1.0 规范中的语法。 有关详细信息，请参阅[XML 文本和 XML 1.0 规范](../../../../visual-basic/programming-guide/language-features/xml/xml-literals-and-the-xml-1-0-specification.md)。  
  
## <a name="line-continuation"></a>续行符  
 XML 文本可以跨多行，而无需使用行继续符 （空间下划线输入序列）。 这使得更轻松地比较 XML 文档的代码中的 XML 文本。  
  
 编译器将作为 XML 文本的一部分行继续符。 因此，你应仅在其所属中时，才使用空间下划线输入序列[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]对象。  
  
 但是，如果，则需要行继续符嵌入式表达式中具有多行表达式。 有关详细信息，请参阅[XML 中的嵌入式表达式](../../../../visual-basic/programming-guide/language-features/xml/embedded-expressions-in-xml.md)。  
  
## <a name="embedding-queries-in-xml-literals"></a>在 XML 文本中嵌入查询  
 你可以在嵌入式表达式中使用查询。 执行此操作时，由查询返回的元素添加到 XML 元素。 这样，你添加到 XML 文本的动态内容，如用户的查询的结果。  
  
 例如，下面的代码使用嵌入式的查询从的成员创建 XML 元素`phoneNumbers2`数组，然后将这些元素添加的子级为`contact2`。  
  
 [!code-vb[VbXMLSamples#7](../../../../visual-basic/language-reference/operators/codesnippet/VisualBasic/xml-literals-overview_3.vb)]  
  
## <a name="how-the-compiler-creates-objects-from-xml-literals"></a>编译器如何从 XML 文本创建对象  
 Visual Basic 编译器将 XML 文本转换为等效的调用[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]构造函数以生成[!INCLUDE[sqltecxlinq](~/includes/sqltecxlinq-md.md)]对象。 例如，Visual Basic 编译器会将下面的代码示例调用转换<xref:System.Xml.Linq.XProcessingInstruction>XML 版本指令，构造函数调用到<xref:System.Xml.Linq.XElement>构造函数`<contact>`， `<name>`，和`<phone>`元素和调用<xref:System.Xml.Linq.XAttribute>构造函数`type`属性。 具体而言，考虑下面的示例中的属性，Visual Basic 编译器将调用<xref:System.Xml.Linq.XAttribute.%23ctor%28System.Xml.Linq.XName%2CSystem.Object%29>两次构造函数。 第一个的值将传递`type`为`name`参数和值`home`为`value`参数。 第二个还将传递值`type`为`name`参数，但值`work`为`value`参数。  
  
 [!code-vb[VbXMLSamples#6](../../../../visual-basic/language-reference/operators/codesnippet/VisualBasic/xml-literals-overview_2.vb)]  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Xml.Linq.XElement>  
 [在 Visual Basic 中创建 XML](../../../../visual-basic/programming-guide/language-features/xml/creating-xml.md)  
 [XML 中的嵌入式表达式](../../../../visual-basic/programming-guide/language-features/xml/embedded-expressions-in-xml.md)  
 [XML 文档文本](../../../../visual-basic/language-reference/xml-literals/xml-document-literal.md)  
 [XML 元素文本](../../../../visual-basic/language-reference/xml-literals/xml-element-literal.md)  
 [XML 文本](../../../../visual-basic/language-reference/xml-literals/index.md)
