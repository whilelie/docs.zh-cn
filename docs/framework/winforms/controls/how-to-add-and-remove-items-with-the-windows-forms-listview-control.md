---
title: 如何：使用 Windows 窗体 ListView 控件添加和移除项
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- ListView control [Windows Forms], populating
- list views [Windows Forms], adding list items
- ListView control [Windows Forms], adding list items
ms.assetid: 1b35a80a-edd8-495f-a807-a28c4aae52c6
ms.openlocfilehash: 83ef2e108695988bbb0329d9f01e1317d9308f18
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-add-and-remove-items-with-the-windows-forms-listview-control"></a>如何：使用 Windows 窗体 ListView 控件添加和移除项
将项添加到 Windows 窗体的过程<xref:System.Windows.Forms.ListView>控件包含主要的指定项并将属性分配给它。 可以在任何时候完成添加或删除列表项。  
  
### <a name="to-add-items-programmatically"></a>以编程方式添加项  
  
1.  使用<xref:System.Windows.Forms.ListView.ListViewItemCollection.Add%2A>方法<xref:System.Windows.Forms.ListView.Items%2A>属性。  
  
     [!code-csharp[System.Windows.Forms.ListViewLegacyTopics#11](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/CS/Class1.cs#11)]
     [!code-vb[System.Windows.Forms.ListViewLegacyTopics#11](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/VB/Class1.vb#11)]  
  
### <a name="to-remove-items-programmatically"></a>以编程方式移除项  
  
1.  使用<xref:System.Windows.Forms.ListView.ListViewItemCollection.RemoveAt%2A>或<xref:System.Windows.Forms.ListView.ListViewItemCollection.Clear%2A>方法<xref:System.Windows.Forms.ListView.Items%2A>属性。 <xref:System.Windows.Forms.ListView.ListViewItemCollection.RemoveAt%2A>方法中删除单个项;<xref:System.Windows.Forms.ListView.ListViewItemCollection.Clear%2A>方法从列表中移除所有项。  
  
     [!code-csharp[System.Windows.Forms.ListViewLegacyTopics#12](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/CS/Class1.cs#12)]
     [!code-vb[System.Windows.Forms.ListViewLegacyTopics#12](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/VB/Class1.vb#12)]  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.Forms.ListView>  
 [ListView 控件](../../../../docs/framework/winforms/controls/listview-control-windows-forms.md)  
 [ListView 控件概述](../../../../docs/framework/winforms/controls/listview-control-overview-windows-forms.md)
