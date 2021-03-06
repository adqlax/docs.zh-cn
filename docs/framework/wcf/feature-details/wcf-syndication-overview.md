---
title: WCF 联合概述
ms.date: 03/30/2017
ms.assetid: af6d4c39-e5e8-4099-aee6-5261feff9107
ms.openlocfilehash: c059ca3ee33b254a60d6b8596b02e1f995fd2ca1
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="wcf-syndication-overview"></a>WCF 联合概述
Windows Communication Foundation (WCF) 提供对公开从 WCF 服务的联合源的支持。 联合是一种应用程序集成机制，在这种机制中，服务器以一种可互操作的格式（称为源）公开某些应用程序数据。 源是应用程序数据的集合，其中包括一些源级别的元数据（标题、作者、URL 和其他元数据）以及一系列源项。 在源内，源项通常是按时间的倒序顺序排序的。 源项由一组标准的项级别元数据（标题、URL、创建日期、类别和其他项级别的元数据）以及任意数量的应用程序特定数据组成。 联合源的两种最常见类型为真正简单的整合 (RSS) 2.0 和 Atom 1.0，WCF 支持这两种。  
  
## <a name="object-model"></a>对象模型  
 WCF 定义了一组特定于联合的类，您可以以独立于格式的方式使用源、 源的项和相关元数据： <xref:System.ServiceModel.Syndication.SyndicationFeed>， <xref:System.ServiceModel.Syndication.SyndicationItem>， <xref:System.ServiceModel.Syndication.SyndicationPerson>， <xref:System.ServiceModel.Syndication.SyndicationLink>，和其他特定于联合的类。 WCF 还定义基于 WCF REST 编程模型以提供联合支持，包括构建的基础结构类： <xref:System.ServiceModel.Syndication.Atom10FeedFormatter>，和<!--zz <xref:System.ServiceModel.Syndication.RSS20FeedFormatter>--> `RSS20FeedFormatter`。 源格式化程序类支持在 RSS 2.0 和 Atom 1.0 之间序列化对象模型。  
  
## <a name="scenarios"></a>方案  
 如今，联合通常用于博客，其中博客作者会定期发布某类信息。 可以是文本、图像、音频或其他类型的信息。 许多报纸和杂志也使用联合来发布新闻故事或文章。 通过订阅这样的源，用户可以获得所有来自此类网站的最新信息。 虽然联合通常与博客和发行者关联，但联合也可以与任何公开信息集合的应用程序一起使用，例如，想要使用联合源公开的 bug 数据库。 你可以创建一个 WCF 服务来公开运算调用`CodeDefects`。 此操作可能会需要一个参数，该参数指定要检索其 bug 的人员的电子邮件地址。 客户端可以使用以下 URL 来调用此操作： http://someserver/bugDatabase/CodeDefects?user=johndoe。  
  
## <a name="syndication-formats"></a>联合格式  
 WCF 联合平台支持 RSS 2.0 和 Atom 1.0。  
  
## <a name="see-also"></a>请参阅  
 [WCF Web HTTP 编程模型](../../../../docs/framework/wcf/feature-details/wcf-web-http-programming-model.md)
