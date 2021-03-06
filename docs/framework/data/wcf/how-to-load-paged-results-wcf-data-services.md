---
title: "如何：加载分页结果（WCF 数据服务）"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework-oob
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: article
dev_langs:
- csharp
- vb
helpviewer_keywords:
- WCF Data Services, deferred content
- WCF Data Services, loading data
ms.assetid: bb786ea4-f3ef-4ad3-9a41-3a0b7feb6a1f
caps.latest.revision: "2"
author: dotnet-bot
ms.author: dotnetcontent
manager: wpickett
ms.workload: dotnet
ms.openlocfilehash: 405bea18b03ba695dcb952d10a193decc124841d
ms.sourcegitcommit: 16186c34a957fdd52e5db7294f291f7530ac9d24
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="how-to-load-paged-results-wcf-data-services"></a>如何：加载分页结果（WCF 数据服务）
[!INCLUDE[ssAstoria](../../../../includes/ssastoria-md.md)] 允许数据服务限制单个响应源中返回的实体数。 在此情况下，源中的最后一项包含指向下一页数据的链接。 通过调用执行 <xref:System.Data.Services.Client.QueryOperationResponse%601.GetContinuation%2A> 时返回的 <xref:System.Data.Services.Client.QueryOperationResponse%601> 的 <xref:System.Data.Services.Client.DataServiceQuery%601> 方法可以获取下一页数据的 URI。 然后，可以使用此对象所表示的 URI 加载下一页结果。 有关详细信息，请参阅[加载延迟的内容](../../../../docs/framework/data/wcf/loading-deferred-content-wcf-data-services.md)。  
  
 本主题中的示例使用罗斯文示例数据服务和自动生成的客户端数据服务类。 在完成时创建此服务和客户端数据类[WCF 数据服务快速入门](../../../../docs/framework/data/wcf/quickstart-wcf-data-services.md)。  
  
## <a name="example"></a>示例  
 下面的示例使用 `do…while` 循环从数据服务的分页结果中加载 `Customers` 实体。  
  
 [!code-csharp[Astoria Northwind Client#GetCustomersPaged](../../../../samples/snippets/csharp/VS_Snippets_Misc/astoria northwind client/cs/source.cs#getcustomerspaged)]
 [!code-vb[Astoria Northwind Client#GetCustomersPaged](../../../../samples/snippets/visualbasic/VS_Snippets_Misc/astoria northwind client/vb/source.vb#getcustomerspaged)]  
  
## <a name="example"></a>示例  
 下面的示例返回每个 `Orders` 实体的相关 `Customers` 实体，并使用 `do…while` 循环从数据服务中加载 `Customers` 实体页以及使用嵌套的 `while` 循环从数据服务中加载相关的 `Orders` 实体的页。  
  
 [!code-csharp[Astoria Northwind Client#GetCustomersPagedNested](../../../../samples/snippets/csharp/VS_Snippets_Misc/astoria northwind client/cs/source.cs#getcustomerspagednested)]
 [!code-vb[Astoria Northwind Client#GetCustomersPagedNested](../../../../samples/snippets/visualbasic/VS_Snippets_Misc/astoria northwind client/vb/source.vb#getcustomerspagednested)]  
  
## <a name="see-also"></a>请参阅  
 [加载延迟的内容](../../../../docs/framework/data/wcf/loading-deferred-content-wcf-data-services.md)  
 [如何：加载相关实体](../../../../docs/framework/data/wcf/how-to-load-related-entities-wcf-data-services.md)
