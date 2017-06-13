---
title: ".NET Framework 中的网络编程 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "VB"
  - "CSharp"
  - "C++"
  - "jsharp"
helpviewer_keywords: 
  - "网络"
  - "Internet"
  - "Internet, .NET Framework Internet 服务"
  - "网络资源"
ms.assetid: 8d455610-67a0-4fa8-a62f-7747064a9256
caps.latest.revision: 24
author: "mcleblanc"
ms.author: "markl"
manager: "markl"
caps.handback.revision: 24
---
# .NET Framework 中的网络编程
Microsoft .NET Framework 为 Internet 服务提供了一种分层、可扩展且托管的实现，可以快速、轻松地将其集成到你的应用程序中。 你的网络应用程序可以基于可插入协议而构建，以便自动利用新的 Internet 协议，或者，它们可以使用 Windows 套接字接口的托管实现在套接字级别上使用网络。  
  
## 本节内容  
 [可插入协议简介](../../../docs/framework/network-programming/introducing-pluggable-protocols.md)  
 描述如何访问 Internet 资源而不考虑它所需的访问协议。  
  
 [正在请求数据...](../../../docs/framework/network-programming/requesting-data.md)  
 说明如何使用可插入协议上载数据和从 Internet 资源下载数据。  
  
 [对可插入协议进行编程](../../../docs/framework/network-programming/programming-pluggable-protocols.md)  
 说明如何派生协议特定的类以实现可插入协议。  
  
 [使用应用程序协议](../../../docs/framework/network-programming/using-application-protocols.md)  
 描述利用 TCP、UDP 和 HTTP 等网络协议的编程应用程序。  
  
 [Internet 协议版本 6](../../../docs/framework/network-programming/internet-protocol-version-6.md)  
 描述 Internet 协议版本 6 \(IPv6\) 相对于当前的 Internet 协议套件版本 \(IPv4\) 的优势，描述 IPv6 寻址、路由和自动配置，以及如何启用和禁用 IPv6。  
  
 [配置 Internet 应用程序](../../../docs/framework/network-programming/configuring-internet-applications.md)  
 说明如何使用 .NET Framework 配置文件来配置 Internet 应用程序。  
  
 [.NET Framework 中的网络跟踪](../../../docs/framework/network-programming/network-tracing.md)  
 说明如何使用网络跟踪来获取有关方法调用的信息，以及有关托管应用程序所生成网络流量的信息。  
  
 [网络应用程序的缓存管理](../../../docs/framework/network-programming/cache-management-for-network-applications.md)  
 描述如何使用应用程序（采用 <xref:System.Net.WebClient?displayProperty=fullName>、<xref:System.Net.WebRequest?displayProperty=fullName> 和 <xref:System.Net.HttpWebRequest?displayProperty=fullName> 类）的缓存。  
  
 [网络编程中的安全性](../../../docs/framework/network-programming/security-in-network-programming.md)  
 描述如何使用 Internet 标准安全性和身份验证方法。  
  
 [System.Net 类的最佳实践](../../../docs/framework/network-programming/best-practices-for-system-net-classes.md)  
 提供关于如何充分利用 Internet 应用程序的提示和技巧。  
  
 [通过代理访问 Internet](../../../docs/framework/network-programming/accessing-the-internet-through-a-proxy.md)  
 描述如何配置代理。  
  
 [NetworkInformation](../../../docs/framework/network-programming/networkinformation.md)  
 描述如何收集有关网络事件、更改、统计信息和属性的信息，并说明如何使用 <xref:System.Net.NetworkInformation.Ping?displayProperty=fullName> 类确定远程主机是否可到达。  
  
 [对 2.0 版中的 System.Uri 命名空间的更改](../../../docs/framework/network-programming/changes-to-the-system-uri-namespace-in-version-2-0.md)  
 描述在版本 2.0 中对 <xref:System.Uri?displayProperty=fullName> 类做出的一些更改，这些更改用于修复错误行为、增强可用性和安全性。  
  
 [System.Uri 中的国际资源标识符支持](../../../docs/framework/network-programming/international-resource-identifier-support-in-system-uri.md)  
 描述在版本 3.5、3.0 SP1 和 2.0 SP1 中对 <xref:System.Uri?displayProperty=fullName> 类进行的增强，这些增强用于提供国际资源标识符 \(IRI\) 和国际化域名 \(IDN\) 支持。  
  
 [版本 3.5 中的套接字性能增强](../../../docs/framework/network-programming/socket-performance-enhancements-in-version-3-5.md)  
 描述在版本 3.5、3.0 SP1 和 2.0 SP1 中对 <xref:System.Net.Sockets.Socket?displayProperty=fullName> 类做出的一系列增强，这些增强提供了一种可供专用高性能套接字应用程序使用的替代异步模式。  
  
 [对等名称解析协议](../../../docs/framework/network-programming/peer-name-resolution-protocol.md)  
 描述在版本 3.5 中添加的支持，它们用于支持对等名称解析协议 \(PNRP\)、一种无服务器和动态名称注册及名称解析协议。 这些新功能由 <xref:System.Net.PeerToPeer?displayProperty=fullName> 命名空间提供支持。  
  
 [对等协作](../../../docs/framework/network-programming/peer-to-peer-collaboration.md)  
 描述在版本 3.5 中添加的支持，它们用于支持基于 PNRP 而构建的对等协作。 这些新功能由 <xref:System.Net.PeerToPeer.Collaboration?displayProperty=fullName> 命名空间提供支持。  
  
 [3.5 SP1 版本中对 HttpWebRequest 的 NTLM 身份验证的更改](../../../docs/framework/network-programming/changes-to-ntlm-authentication-for-httpwebrequest-in-version-3-5-sp1.md)  
 描述在版本 3.5 SP1 中做出的安全性更改，这些更改可影响以下类处理集成式 Windows 身份验证的方式：<xref:System.Net.HttpWebRequest?displayProperty=fullName>、<xref:System.Net.HttpListener?displayProperty=fullName>、<xref:System.Net.Security.NegotiateStream?displayProperty=fullName>，以及 System.Net 命名空间中的相关类。  
  
 [带有扩展保护的集成 Windows 身份验证](../../../docs/framework/network-programming/integrated-windows-authentication-with-extended-protection.md)  
 描述扩展保护方面的增强，这些增强可影响以下类处理集成式 Windows 身份验证的方式：<xref:System.Net.HttpWebRequest?displayProperty=fullName>、<xref:System.Net.HttpListener?displayProperty=fullName>、<xref:System.Net.Mail.SmtpClient?displayProperty=fullName>、<xref:System.Net.Security.SslStream?displayProperty=fullName>、<xref:System.Net.Security.NegotiateStream?displayProperty=fullName> 以及 <xref:System.Net?displayProperty=fullName> 和相关命名空间中的相关类。  
  
 [使用 IPv6 和 Teredo 的 NAT 遍历](../../../docs/framework/network-programming/nat-traversal-using-ipv6-and-teredo.md)  
 描述添加到 <xref:System.Net?displayProperty=fullName>、<xref:System.Net.NetworkInformation?displayProperty=fullName> 和 <xref:System.Net.Sockets?displayProperty=fullName> 命名空间的增强，这些增强用于支持使用 IPv6 和 Teredo 进行 NAT 遍历。  
  
 [Windows 应用商店应用的网络隔离](../../../docs/framework/network-programming/network-isolation-for-windows-store-apps.md)  
 描述当在 <xref:System.Net>应用中使用 <xref:System.Net.Http>、<xref:System.Net.Http.Headers> 和 [!INCLUDE[win8_appname_long](../../../includes/win8-appname-long-md.md)] 命名空间中的类时，网络隔离所产生的影响。  
  
 [网络编程示例](../../../docs/framework/network-programming/network-programming-samples.md)  
 可下载网络编程示例的链接，这些示例使用 <xref:System.Net>、<xref:System.Net.Cache>、<xref:System.Net.Configuration>、<xref:System.Net.Mail>、<xref:System.Net.Mime>、<xref:System.Net.NetworkInformation>、<xref:System.Net.PeerToPeer>、<xref:System.Net.Security>、<xref:System.Net.Sockets> 命名空间中的类。  
  
## 参考  
 <xref:System.Net?displayProperty=fullName>  
 为当前网络采用的多种协议提供简单的编程接口。 此命名空间中的 <xref:System.Net.WebRequest?displayProperty=fullName> 和 <xref:System.Net.WebResponse?displayProperty=fullName> 类是可插入协议的基础。  
  
 <xref:System.Net.Cache?displayProperty=fullName>  
 定义一些类型和枚举，这些类型和枚举用于为通过 <xref:System.Net.WebRequest?displayProperty=fullName> 和 <xref:System.Net.HttpWebRequest?displayProperty=fullName> 类获取的资源制定缓存策略。  
  
 <xref:System.Net.Configuration?displayProperty=fullName>  
 应用程序以编程方式访问和更新 System.Net 命名空间的配置设置时所使用的类。  
  
 <xref:System.Net.Http?displayProperty=fullName>  
 用于为现代 HTTP 应用程序提供编程接口的类。  
  
 <xref:System.Net.Http.Headers?displayProperty=fullName>  
 为 <xref:System.Net.Http?displayProperty=fullName> 命名空间使用的 HTTP 标头集合提供支持。  
  
 <xref:System.Net.Mail?displayProperty=fullName>  
 使用 SMTP 协议撰写和发送邮件时所使用的类。  
  
 <xref:System.Net.Mime?displayProperty=fullName>  
 定义一些类型，这些类型用于表示供 <xref:System.Net.Mail?displayProperty=fullName> 命名空间中的类所使用的多用途 Internet 邮件交换 \(MIME\) 标头。  
  
 <xref:System.Net.NetworkInformation?displayProperty=fullName>  
 用于以编程方式收集有关网络事件、更改、统计信息和属性的信息的类。  
  
 <xref:System.Net.PeerToPeer?displayProperty=fullName>  
 为开发人员提供对等名称解析协议 \(PNRP\) 的一种托管实现。  
  
 <xref:System.Net.PeerToPeer.Collaboration?displayProperty=fullName>  
 为开发人员提供对接协作接口的一种托管实现。  
  
 <xref:System.Net.Security?displayProperty=fullName>  
 用于为主机间的安全通信提供网络流的类。  
  
 <xref:System.Net.Sockets?displayProperty=fullName>  
 为需要帮助控制网络访问的开发人员提供 Windows 套接字 \(Winsock\) 接口的一种托管实现。  
  
 <xref:System.Net.WebSockets?displayProperty=fullName>  
 为开发人员提供 WebSocket 接口的一种托管实现。  
  
 <xref:System.Uri?displayProperty=fullName>  
 提供统一资源标识符 \(URI\) 的对象表示形式和对 URI 各部分的轻松访问。  
  
 <xref:System.Security.Authentication.ExtendedProtection?displayProperty=fullName>  
 为采用应用程序扩展保护的身份验证提供支持。  
  
 <xref:System.Security.Authentication.ExtendedProtection.Configuration?displayProperty=fullName>  
 为配置采用应用程序扩展保护的身份验证提供支持。  
  
## 请参阅  
 [网络编程操作说明主题](../../../docs/framework/network-programming/network-programming-how-to-topics.md)   
 [网络编程示例](../../../docs/framework/network-programming/network-programming-samples.md)   
 [MSDN 代码库中的 .NET 联网示例](http://code.msdn.microsoft.com/Wiki/View.aspx?ProjectName=nclsamples)   
 [HttpClient 示例](http://go.microsoft.com/fwlink/?LinkId=242550)