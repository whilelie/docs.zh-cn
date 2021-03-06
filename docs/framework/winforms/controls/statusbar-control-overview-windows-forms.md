---
title: StatusBar 控件概述（Windows 窗体）
ms.date: 03/30/2017
f1_keywords:
- StatusBar
helpviewer_keywords:
- StatusBar control [Windows Forms], about StatusBar control
- status bars
ms.assetid: b7b9852c-633d-4416-bb2e-94852b989c6c
ms.openlocfilehash: 6dd5b45b38ec4fb04d9a53a1648cfe6e5a5b9f20
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="statusbar-control-overview-windows-forms"></a>StatusBar 控件概述（Windows 窗体）
> [!IMPORTANT]
>  <xref:System.Windows.Forms.StatusStrip>和<xref:System.Windows.Forms.ToolStripStatusLabel>控件替换，并将功能添加到<xref:System.Windows.Forms.StatusBar>和<xref:System.Windows.Forms.StatusBarPanel>控制; 但是，<xref:System.Windows.Forms.StatusBar>和<xref:System.Windows.Forms.StatusBarPanel>控件将保留用于向后兼容性和将来使用，如果你选择。  
  
 Windows 窗体[StatusBar 控件](../../../../docs/framework/winforms/controls/statusbar-control-windows-forms.md)在窗体上用作一个区域后，通常显示在窗口的底部，应用程序可在其中显示各种状态信息。 <xref:System.Windows.Forms.StatusBar> 控件可以具有状态栏面板上显示的文本或图标，以指示状态或一系列表示正在进程; 在动画中的图标例如，[!INCLUDE[ofprword](../../../../includes/ofprword-md.md)]指示正在保存文档。  
  
## <a name="using-the-statusbar-control"></a>使用 StatusBar 控件  
 Internet Explorer 使用状态栏以指示某个页面的 URL，何时鼠标滚动超链接;[!INCLUDE[ofprword](../../../../includes/ofprword-md.md)]提供你在页的位置、 部分位置和编辑模式，例如改写和修订跟踪; 和 Visual Studio 使用状态栏以提供上下文相关的信息，如告诉你如何操作可停靠窗口上的信息为停靠或浮动。  
  
 你可以在状态栏上显示一条消息，通过设置<xref:System.Windows.Forms.StatusBar.ShowPanels%2A>属性`false`（默认值） 和设置<xref:System.Windows.Forms.StatusBar.Text%2A>到你想要在状态栏中显示的文本的状态栏的属性。 可以将状态栏划分为面板，以通过设置显示的信息的多个类型<xref:System.Windows.Forms.StatusBar.ShowPanels%2A>属性`true`和使用<xref:System.Windows.Forms.StatusBar.StatusBarPanelCollection.Add%2A>方法<xref:System.Windows.Forms.StatusBar.StatusBarPanelCollection>。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.Forms.StatusBar>  
 <xref:System.Windows.Forms.ToolStripStatusLabel>  
 [如何：确定 Windows 窗体 StatusBar 控件中的哪个面板获得了单击](../../../../docs/framework/winforms/controls/determine-which-panel-wf-statusbar-control-was-clicked.md)
