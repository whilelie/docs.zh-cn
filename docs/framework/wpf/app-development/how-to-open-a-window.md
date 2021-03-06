---
title: 如何： 打开一个窗口
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- windows [WPF], opening
- opening windows [WPF]
ms.assetid: 6b91b2bb-fda7-491d-a72e-139dd630a5b0
ms.openlocfilehash: 23dc74666d8f47a0fb735d96ad22ed56c96bdbc5
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-open-a-window"></a>如何： 打开一个窗口
此示例演示如何打开窗口。  
  
## <a name="example"></a>示例  
 通过实例化打开一个窗口<xref:System.Windows.Window>并调用<xref:System.Windows.Window.Show%2A>方法。 <xref:System.Windows.Window.Show%2A> 将打开一个窗口，并立即返回而不等待新窗口将会关闭。 这种类型的窗口是也称为*无模式*窗口中，它不会限制用户输入。  
  
 [!code-csharp[HOWTOWindowManagementSnippets#OpenNewWindowCODE](../../../../samples/snippets/csharp/VS_Snippets_Wpf/HOWTOWindowManagementSnippets/CSharp/MainWindow.xaml.cs#opennewwindowcode)]
 [!code-vb[HOWTOWindowManagementSnippets#OpenNewWindowCODE](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/HOWTOWindowManagementSnippets/visualbasic/mainwindow.xaml.vb#opennewwindowcode)]  
  
## <a name="net-framework-security"></a>.NET Framework 安全性  
 实例化<xref:System.Windows.Window>需要有权调用不安全的本机方法 (请参阅<xref:System.Windows.Window.%23ctor%2A>)。
