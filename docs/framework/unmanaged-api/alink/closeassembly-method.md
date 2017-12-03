---
title: "CloseAssembly 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name:
- IALink.CloseAssembly
- CloseAssembly
api_location: alink.dll
api_type: COM
f1_keywords: CloseAssembly
helpviewer_keywords: CloseAssembly method
ms.assetid: f66a43bc-a5c5-4190-acbe-63fd27640634
topic_type: apiref
caps.latest.revision: "6"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: be68348b619f342eca4841a6052088bf7152f453
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="closeassembly-method"></a><span data-ttu-id="276a7-102">CloseAssembly 方法</span><span class="sxs-lookup"><span data-stu-id="276a7-102">CloseAssembly Method</span></span>
<span data-ttu-id="276a7-103">确定程序集操作。</span><span class="sxs-lookup"><span data-stu-id="276a7-103">Finalizes assembly operations.</span></span> <span data-ttu-id="276a7-104">在开始一个新的程序集或未绑定的模块之前调用此方法。</span><span class="sxs-lookup"><span data-stu-id="276a7-104">Call this method before beginning a new assembly or unbound module.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="276a7-105">语法</span><span class="sxs-lookup"><span data-stu-id="276a7-105">Syntax</span></span>  
  
```  
HRESULT CloseAssembly(  
    mdAssembly AssemblyID  
) PURE;  
```  
  
#### <a name="parameters"></a><span data-ttu-id="276a7-106">参数</span><span class="sxs-lookup"><span data-stu-id="276a7-106">Parameters</span></span>  
 `AssemblyID`  
 <span data-ttu-id="276a7-107">程序集的 ID。</span><span class="sxs-lookup"><span data-stu-id="276a7-107">ID of the assembly.</span></span>  
  
## <a name="return-value"></a><span data-ttu-id="276a7-108">返回值</span><span class="sxs-lookup"><span data-stu-id="276a7-108">Return Value</span></span>  
 <span data-ttu-id="276a7-109">如果该方法成功，则返回，则为 S_OK。</span><span class="sxs-lookup"><span data-stu-id="276a7-109">Returns S_OK if the method succeeds.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="276a7-110">要求</span><span class="sxs-lookup"><span data-stu-id="276a7-110">Requirements</span></span>  
 <span data-ttu-id="276a7-111">需要 alink.h。</span><span class="sxs-lookup"><span data-stu-id="276a7-111">Requires alink.h.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="276a7-112">另请参阅</span><span class="sxs-lookup"><span data-stu-id="276a7-112">See Also</span></span>  
 [<span data-ttu-id="276a7-113">IALink 接口</span><span class="sxs-lookup"><span data-stu-id="276a7-113">IALink Interface</span></span>](../../../../docs/framework/unmanaged-api/alink/ialink-interface.md)  
 [<span data-ttu-id="276a7-114">IALink2 接口</span><span class="sxs-lookup"><span data-stu-id="276a7-114">IALink2 Interface</span></span>](../../../../docs/framework/unmanaged-api/alink/ialink2-interface.md)  
 [<span data-ttu-id="276a7-115">ALink API</span><span class="sxs-lookup"><span data-stu-id="276a7-115">ALink API</span></span>](../../../../docs/framework/unmanaged-api/alink/index.md)