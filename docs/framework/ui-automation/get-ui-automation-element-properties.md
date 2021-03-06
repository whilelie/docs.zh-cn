---
title: 获取 UI 自动化元素的属性
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- properties, retrieving
- UI Automation, retrieving properties of elements
ms.assetid: 09576b1a-291f-435c-980e-dee32d899ae1
author: Xansky
ms.author: mhopkins
manager: markl
ms.openlocfilehash: 73678433692f5532f712f0d2c7a3c5bf138a87b5
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="get-ui-automation-element-properties"></a>获取 UI 自动化元素的属性
> [!NOTE]
>  本文档适用于想要使用 [!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)] 命名空间中定义的托管 <xref:System.Windows.Automation> 类的 .NET Framework 开发人员。 有关 [!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)]的最新信息，请参阅 [Windows 自动化 API：UI 自动化](http://go.microsoft.com/fwlink/?LinkID=156746)。  
  
 本主题演示如何检索的属性[!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)]元素。  
  
### <a name="get-a-current-property-value"></a>获取当前的属性值  
  
1.  获取<xref:System.Windows.Automation.AutomationElement>你想要获取其属性。  
  
2.  调用<xref:System.Windows.Automation.AutomationElement.GetCurrentPropertyValue%2A>，或检索<xref:System.Windows.Automation.AutomationElement.Current%2A>属性结构并获取其成员之一的值。  
  
### <a name="get-a-cached-property-value"></a>获取缓存的属性值  
  
1.  获取<xref:System.Windows.Automation.AutomationElement>你想要获取其属性。 属性必须在指定<xref:System.Windows.Automation.CacheRequest>。  
  
2.  调用<xref:System.Windows.Automation.AutomationElement.GetCachedPropertyValue%2A>，或检索<xref:System.Windows.Automation.AutomationElement.Cached%2A>属性结构并获取其成员之一的值。  
  
## <a name="example"></a>示例  
 下面的示例演示各种方法来检索当前属性<xref:System.Windows.Automation.AutomationElement>。  
  
 [!code-csharp[UIAClient_snip#170](../../../samples/snippets/csharp/VS_Snippets_Wpf/UIAClient_snip/CSharp/ClientForm.cs#170)]
 [!code-vb[UIAClient_snip#170](../../../samples/snippets/visualbasic/VS_Snippets_Wpf/UIAClient_snip/VisualBasic/ClientForm.vb#170)]  
  
## <a name="see-also"></a>请参阅  
 [客户端的 UI 自动化属性](../../../docs/framework/ui-automation/ui-automation-properties-for-clients.md)  
 [在 UI 自动化中使用缓存](../../../docs/framework/ui-automation/use-caching-in-ui-automation.md)  
 [在 UI 自动化客户端中缓存](../../../docs/framework/ui-automation/caching-in-ui-automation-clients.md)
