---
title: 如何：调用自定义数据库函数
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
ms.assetid: 4354e5eb-dd45-469d-97fb-1c495705ee59
ms.openlocfilehash: 790bb8d4ea1e146d94ea7cf153b8909c6cc1af7a
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2018
---
# <a name="how-to-call-custom-database-functions"></a>如何：调用自定义数据库函数
本主题介绍如何从 LINQ to Entities 查询中调用在数据库中定义的自定义函数。  
  
 从 LINQ to Entities 查询中调用的数据库函数在数据库中执行。 在数据库中执行函数可以改进应用程序性能。  
  
 下面的过程高度概括了有关调用自定义数据库函数的信息。 后面的示例提供了有关该过程中各个步骤的更多详细信息。  
  
### <a name="to-call-custom-functions-that-are-defined-in-the-database"></a>调用在数据库中定义的自定义函数  
  
1.  在数据库中创建自定义函数。  
  
     有关在 SQL Server 中创建自定义函数的详细信息，请参阅[CREATE FUNCTION (Transact SQL)](http://go.microsoft.com/fwlink/?LinkID=139871)。  
  
2.  在您的 .edmx 文件的存储架构定义语言 (SSDL) 中声明一个函数。 该函数的名称必须与在数据库中声明的函数的名称相同。  
  
     有关详细信息，请参阅[函数元素 (SSDL)](http://msdn.microsoft.com/library/b60cfc3d-8b93-423e-8c99-b867256640a4)。  
  
3.  将相应的方法添加到应用程序代码中的类，并将 <xref:System.Data.Objects.DataClasses.EdmFunctionAttribute> 应用于该方法。注意，该特性的 <xref:System.Data.Objects.DataClasses.EdmFunctionAttribute.NamespaceName%2A> 和 <xref:System.Data.Objects.DataClasses.EdmFunctionAttribute.FunctionName%2A> 参数分别是概念模型的命名空间名称和概念模型中的函数名称。 LINQ 的函数名称解析区分大小写。  
  
4.  在 LINQ to Entities 查询中调用此方法。  
  
## <a name="example"></a>示例  
 下面的示例演示如何从 LINQ to Entities 查询中调用自定义数据库函数。 本示例使用 School 模型。 School 模型有关的信息，请参阅[创建 School 示例数据库](http://msdn.microsoft.com/library/c1bec483-a0ea-4660-aa0b-7b0a8b68fed0)和[生成学校.edmx 文件](http://msdn.microsoft.com/library/c48b3907-a8be-4fe6-884c-e95af1852758)。  
  
 下面的代码将 `AvgStudentGrade` 函数添加到 School 示例数据库。  
  
> [!NOTE]
>  用于调用自定义数据库函数的步骤是相同的，与数据库服务器无关。 但是，下面的代码特定于在 SQL Server 数据库中创建函数。 在其他数据库服务器中创建自定义函数的代码可能有所不同。  
  
 [!code-sql[DP L2E MapToDBFunction#1](../../../../../../samples/snippets/tsql/VS_Snippets_Data/dp l2e maptodbfunction/tsql/create_avgstudentgrade.sql#1)]  
  
## <a name="example"></a>示例  
 接下来，在您的 .edmx 文件的存储架构定义语言 (SSDL) 中声明一个函数。 下面的代码在 SSDL 中声明 `AvgStudentGrade` 函数：  
  
 [!code-xml[DP L2E MapToDBFunction#2](../../../../../../samples/snippets/csharp/VS_Snippets_Data/dp l2e maptodbfunction/cs/school.edmx#2)]  
  
## <a name="example"></a>示例  
 现在创建一个方法，并将其映射到在 SSDL 中声明的函数。 通过使用 <xref:System.Data.Objects.DataClasses.EdmFunctionAttribute> 将以下类中的方法映射到在 SSDL 中定义的函数（上述）。 调用此方法时，将执行数据库中相应的函数。  
  
 [!code-csharp[DP L2E MapToDBFunction#3](../../../../../../samples/snippets/csharp/VS_Snippets_Data/dp l2e maptodbfunction/cs/program.cs#3)]
 [!code-vb[DP L2E MapToDBFunction#3](../../../../../../samples/snippets/visualbasic/VS_Snippets_Data/dp l2e maptodbfunction/vb/module1.vb#3)]  
  
## <a name="example"></a>示例  
 最后，在 LINQ to Entities 查询中调用此方法。 下面的代码将向控制台显示学生的姓氏和平均年级：  
  
 [!code-csharp[DP L2E MapToDBFunction#4](../../../../../../samples/snippets/csharp/VS_Snippets_Data/dp l2e maptodbfunction/cs/program.cs#4)]
 [!code-vb[DP L2E MapToDBFunction#4](../../../../../../samples/snippets/visualbasic/VS_Snippets_Data/dp l2e maptodbfunction/vb/module1.vb#4)]  
  
## <a name="see-also"></a>请参阅  
 [.edmx 文件概述](http://msdn.microsoft.com/library/f4c8e7ce-1db6-417e-9759-15f8b55155d4)  
 [LINQ to Entities 中的查询](../../../../../../docs/framework/data/adonet/ef/language-reference/queries-in-linq-to-entities.md)
