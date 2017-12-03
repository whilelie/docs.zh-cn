---
title: "IAppDomainBinding 接口"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IAppDomainBinding
api_location: mscoree.dll
api_type: COM
f1_keywords: IAppDomainBinding
helpviewer_keywords: IAppDomainBinding interface [.NET Framework hosting]
ms.assetid: 368881ab-c4ea-4731-bf22-c596aac7c66c
topic_type: apiref
caps.latest.revision: "11"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 2e02c1b9499bc2972f88c9045d3f59423edb6cb2
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="iappdomainbinding-interface"></a><span data-ttu-id="fecaf-102">IAppDomainBinding 接口</span><span class="sxs-lookup"><span data-stu-id="fecaf-102">IAppDomainBinding Interface</span></span>
<span data-ttu-id="fecaf-103">提供由公共语言运行时 (CLR)，用于通知主机应用程序已创建应用程序域调用的方法。</span><span class="sxs-lookup"><span data-stu-id="fecaf-103">Provides a method that is called by the common language runtime (CLR) to notify the host application that an application domain has been created.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="fecaf-104">方法</span><span class="sxs-lookup"><span data-stu-id="fecaf-104">Methods</span></span>  
  
|<span data-ttu-id="fecaf-105">方法</span><span class="sxs-lookup"><span data-stu-id="fecaf-105">Method</span></span>|<span data-ttu-id="fecaf-106">描述</span><span class="sxs-lookup"><span data-stu-id="fecaf-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="fecaf-107">OnAppDomain 方法</span><span class="sxs-lookup"><span data-stu-id="fecaf-107">OnAppDomain Method</span></span>](../../../../docs/framework/unmanaged-api/hosting/iappdomainbinding-onappdomain-method.md)|<span data-ttu-id="fecaf-108">由公共语言运行时 (CLR)，用于通知宿主已创建应用程序域调用。</span><span class="sxs-lookup"><span data-stu-id="fecaf-108">Called by the common language runtime (CLR) to notify the host that an application domain has been created.</span></span>|  
  
## <a name="requirements"></a><span data-ttu-id="fecaf-109">要求</span><span class="sxs-lookup"><span data-stu-id="fecaf-109">Requirements</span></span>  
 <span data-ttu-id="fecaf-110">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="fecaf-110">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="fecaf-111">**标头：** MSCorEE.h</span><span class="sxs-lookup"><span data-stu-id="fecaf-111">**Header:** MSCorEE.h</span></span>  
  
 <span data-ttu-id="fecaf-112">**库：**作为 MSCorEE.dll 中的资源</span><span class="sxs-lookup"><span data-stu-id="fecaf-112">**Library:** Included as a resource in MSCorEE.dll</span></span>  
  
 <span data-ttu-id="fecaf-113">**.NET framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="fecaf-113">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="fecaf-114">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fecaf-114">See Also</span></span>  
 [<span data-ttu-id="fecaf-115">承载接口</span><span class="sxs-lookup"><span data-stu-id="fecaf-115">Hosting Interfaces</span></span>](../../../../docs/framework/unmanaged-api/hosting/hosting-interfaces.md)