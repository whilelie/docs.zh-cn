---
title: 实体框架提供程序（WCF 数据服务）
ms.date: 03/30/2017
helpviewer_keywords:
- WCF Data Services, providers
ms.assetid: 650b5eb6-c71d-4dc1-8b64-b6beaf752114
ms.openlocfilehash: 0b6e76e6c05a091c57f27fc759044d3567cd976a
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="entity-framework-provider-wcf-data-services"></a>实体框架提供程序（WCF 数据服务）
与 [!INCLUDE[ssAstoria](../../../../includes/ssastoria-md.md)] 类似，ADO.NET 实体框架也基于实体数据模型（一种实体关系模型）。 实体框架将针对实体数据模型中，调用其实现*概念模型*，转换为针对数据源的等效操作。 这使实体框架成为基于关系数据的数据服务的理想提供程序，任何具有支持实体框架的数据提供程序的数据库都可用于 [!INCLUDE[ssAstoria](../../../../includes/ssastoria-md.md)]。 有关当前支持实体框架的数据源的列表，请参阅[用于实体框架的第三方提供商](http://go.microsoft.com/fwlink/?LinkId=143699)。  
  
 在概念模型中，实体容器是服务的根。 必须先在实体框架中定义一个概念模型，数据服务才能公开数据。 有关详细信息，请参阅[如何： 创建数据服务使用 ADO.NET 实体框架数据源](../../../../docs/framework/data/wcf/create-a-data-service-using-an-adonet-ef-data-wcf.md)。  
  
 [!INCLUDE[ssAstoria](../../../../includes/ssastoria-md.md)] 支持开放式并发模型，使您能够定义并发标记的实体。 这样一个包含一个或多个实体属性的并发标记由数据服务用来确定，正在请求、更新或删除的数据中是否发生了更改。 如果从请求的 eTag 中获取的标记值与实体的当前值不相同，则数据服务将引发异常。 若要指示某个属性为并发标记的一部分，必须在`ConcurrencyMode="Fixed"`提供程序所定义的数据模型中应用 [!INCLUDE[adonet_ef](../../../../includes/adonet-ef-md.md)] 特性。 并发标记不能包含键属性或导航属性。 有关详细信息，请参阅[更新数据服务](../../../../docs/framework/data/wcf/updating-the-data-service-wcf-data-services.md)。  
  
 若要了解有关实体框架的详细信息，请参阅[实体框架概述](../../../../docs/framework/data/adonet/ef/overview.md)。  
  
## <a name="see-also"></a>请参阅  
 [数据服务提供程序](../../../../docs/framework/data/wcf/data-services-providers-wcf-data-services.md)  
 [反射提供程序](../../../../docs/framework/data/wcf/reflection-provider-wcf-data-services.md)  
 [实体数据模型](../../../../docs/framework/data/adonet/entity-data-model.md)
