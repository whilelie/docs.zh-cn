---
title: 如何： 打开一个消息框
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- message boxes [WPF], opening
- opening message boxes [WPF]
ms.assetid: acaad17f-af43-4eca-a004-f1c9e7c6f292
ms.openlocfilehash: dd79d69c9b1b54c5158b58ee2f1675e7d11a386a
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-open-a-message-box"></a>如何： 打开一个消息框
此示例演示如何以打开一个消息框。  
  
## <a name="example"></a>示例  
 消息框是一种预制模式对话框用于向用户显示信息。 通过调用静态打开一个消息框<xref:System.Windows.MessageBox.Show%2A>方法<xref:System.Windows.MessageBox>类。 当<xref:System.Windows.MessageBox.Show%2A>是调用，则消息将传递使用字符串参数。 几个重载<xref:System.Windows.MessageBox.Show%2A>允许你配置如何将出现一个消息框 (请参阅<xref:System.Windows.MessageBox>)。  
  
 [!code-csharp[MessageBoxSnippets#MessageBoxShow1CODE](../../../../samples/snippets/csharp/VS_Snippets_Wpf/MessageBoxSnippets/CSharp/Show1Window.xaml.cs#messageboxshow1code)]
 [!code-vb[MessageBoxSnippets#MessageBoxShow1CODE](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/MessageBoxSnippets/visualbasic/show1window.xaml.vb#messageboxshow1code)]  
  
## <a name="see-also"></a>请参阅  
 [消息框示例](http://go.microsoft.com/fwlink/?LinkID=160023)
