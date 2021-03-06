---
title: 使用唯一侦听 Uri 模式示例发现服务
ms.date: 03/30/2017
ms.assetid: 9a6d35b2-0469-43c8-a0c9-63623e3d2733
ms.openlocfilehash: e6129594df6170f94a06caa08a9f16e4770bbfd4
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="discover-a-service-with-unique-listen-uri-mode-sample"></a>使用唯一侦听 Uri 模式示例发现服务
此示例演示如何发现 <xref:System.ServiceModel.Channels.BindingContext.ListenUriMode%2A> 属性设置为 <xref:System.ServiceModel.Description.ListenUriMode.Unique> 的服务。 当 <xref:System.ServiceModel.Channels.BindingContext.ListenUriMode%2A> 属性设置为 <xref:System.ServiceModel.Description.ListenUriMode.Unique> 时，通过将端口设置为唯一或追加 GUID 使其对路径唯一来确保 ListenUri 唯一。  
  
### <a name="features-on-the-service"></a>服务上的功能  
 对于 TCP 终结点，<xref:System.ServiceModel.Channels.BindingContext.ListenUriMode%2A> 属性设置为 <xref:System.ServiceModel.Description.ListenUriMode.Unique>。 随后可在 <xref:System.ServiceModel.Discovery.UdpDiscoveryEndpoint> 上发现服务。  
  
### <a name="features-on-the-client"></a>客户端上的功能  
 此客户端使用 `Via.Uri` 方法通过正确的 <xref:System.ServiceModel.Discovery.DiscoveryClient.Find%2A> 连接到服务。 随后查询从该方法返回的 <xref:System.ServiceModel.Discovery.FindResponse>，以了解其是否包含有效的 <xref:System.ServiceModel.Endpoint.ListenUri%2A> 以及是否与 `Address.Uri` 不同。 随后会将合适的信息传递给 `InvokeCalculatorService` 方法。 在 `InvokeCalculatorService` 方法中，调用方传入 <xref:System.ServiceModel.Endpoint.ListenUri%2A>，随后具有正确 `ClientViaBehavior` 的 `Via.Uri` 会添加到客户端的终结点。  
  
##### <a name="to-use-this-sample"></a>使用此示例  
  
1.  使用 [!INCLUDE[vs_current_long](../../../../includes/vs-current-long-md.md)] 打开 UniqueListenUriMode.sln。  
  
2.  要生成解决方案，按 Ctrl+Shift+B。  
  
3.  运行在 [解决方案基目录]\service\bin\debug 文件夹中生成的服务应用程序。  
  
4.  运行在 [解决方案基目录]\Client\bin\debug 文件夹中生成的客户端应用程序。  
  
     客户端定位正在运行的服务并向控制台写入服务终结点发布的元数据。  
  
> [!IMPORTANT]
>  您的计算机上可能已安装这些示例。 在继续操作之前，请先检查以下（默认）目录：  
>   
>  `<InstallDrive>:\WF_WCF_Samples`  
>   
>  如果此目录不存在，请转到[Windows Communication Foundation (WCF) 和针对.NET Framework 4 的 Windows Workflow Foundation (WF) 示例](http://go.microsoft.com/fwlink/?LinkId=150780)下载所有 Windows Communication Foundation (WCF) 和[!INCLUDE[wf1](../../../../includes/wf1-md.md)]示例。 此示例位于以下目录：  
>   
>  `<InstallDrive>:\WF_WCF_Samples\WCF\Basic\Discovery\UniqueListenUriMode`  
  
## <a name="see-also"></a>请参阅
