---
title: 无法根据这些自变量推断类型参数的数据类型
ms.date: 07/20/2015
f1_keywords:
- bc36644
- bc36647
- vbc36647
- vbc36644
helpviewer_keywords:
- BC36644
- BC36647
ms.assetid: 0e0050f2-2039-4311-b260-f0ebfde84189
ms.openlocfilehash: 6f84df5c9388220e5ca817d95362753df0920534
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="data-types-of-the-type-parameters-cannot-be-inferred-from-these-arguments"></a>无法根据这些自变量推断类型参数的数据类型
无法从这些实参推断类型参数的数据类型。 显式指定数据类型可更正此错误。  
  
 当重载决策失败时发生此错误。 它以从属消息的形式发生，该消息指出已消除特定的重载候选。 错误消息，告诉编译器无法使用类型推断功能来确定类型参数的数据类型。  
  
> [!NOTE]
>  当无法指定实参时（例如，对于查询表达式中的查询运算符），显示的错误消息不包括第二个句子。  
  
 下面的代码演示了此错误。  
  
```vb  
Module Module1  
  
    Sub Main()  
  
        '' Not Valid.  
        'OverloadedGenericMethod("Hello", "World")  
  
    End Sub  
  
    Sub OverloadedGenericMethod(Of T)(ByVal x As String,   
                                      ByVal y As InterfaceExample(Of T))  
    End Sub  
  
    Sub OverloadedGenericMethod(Of T, R)(ByVal x As T,   
                                         ByVal y As InterfaceExample(Of R))  
    End Sub  
  
End Module  
  
Interface InterfaceExample(Of T)  
End Interface  
```  
  
 **错误 ID:** BC36647 和 BC36644  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
-   你或许能够指定类型形参的数据类型，而无需依赖类型推断。  
  
## <a name="see-also"></a>请参阅  
 [宽松委托转换](../../../visual-basic/programming-guide/language-features/delegates/relaxed-delegate-conversion.md)  
 [在 Visual Basic 中的泛型过程](../../../visual-basic/programming-guide/language-features/data-types/generic-procedures.md)  
 [在 Visual Basic 中的类型转换](../../../visual-basic/programming-guide/language-features/data-types/type-conversions.md)
