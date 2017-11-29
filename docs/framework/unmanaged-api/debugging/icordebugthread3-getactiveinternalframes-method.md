---
title: "ICorDebugThread3::GetActiveInternalFrames 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugThread3.GetActiveInternalFrames Method
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugThread3::GetActiveInternalFrames
helpviewer_keywords:
- ICorDebugThread3::GetActiveInternalFrames method [.NET Framework debugging]
- GetActiveInternalFrames method [.NET Framework debugging]
ms.assetid: d69796b4-5b6d-457c-85f6-2cf42e8a8773
topic_type: apiref
caps.latest.revision: "7"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: b9b94827ac49c69c5e72c2e300a80914774cc498
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="icordebugthread3getactiveinternalframes-method"></a><span data-ttu-id="901ae-102">ICorDebugThread3::GetActiveInternalFrames 方法</span><span class="sxs-lookup"><span data-stu-id="901ae-102">ICorDebugThread3::GetActiveInternalFrames Method</span></span>
<span data-ttu-id="901ae-103">返回内部帧的数组 ([ICorDebugInternalFrame2](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe2-interface.md)对象) 堆栈上。</span><span class="sxs-lookup"><span data-stu-id="901ae-103">Returns an array of internal frames ([ICorDebugInternalFrame2](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe2-interface.md) objects) on the stack.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="901ae-104">语法</span><span class="sxs-lookup"><span data-stu-id="901ae-104">Syntax</span></span>  
  
```  
HRESULT GetActiveInternalFrames  
      (  
      [in] ULONG32 cInternalFrames,  
      [out] ULONG32 *pcInternalFrames,  
      [in, out,size_is(cInternalFrames), length_is(*pcInternalFrames)]  
            ICorDebugInternalFrame2 * ppInternalFrames[]  
      );  
```  
  
#### <a name="parameters"></a><span data-ttu-id="901ae-105">参数</span><span class="sxs-lookup"><span data-stu-id="901ae-105">Parameters</span></span>  
 `cInternalFrames`  
 <span data-ttu-id="901ae-106">[in]预期中的内部帧的数目`ppInternalFrames`。</span><span class="sxs-lookup"><span data-stu-id="901ae-106">[in] The number of internal frames expected in `ppInternalFrames`.</span></span>  
  
 `pcInternalFrames`  
 <span data-ttu-id="901ae-107">[out]指向的指针`ULONG32`，其中包含的堆栈上的内部帧的数目。</span><span class="sxs-lookup"><span data-stu-id="901ae-107">[out] A pointer to a `ULONG32` that contains the number of internal frames on the stack.</span></span>  
  
 `ppInternalFrames`  
 <span data-ttu-id="901ae-108">[在中，out]指向数组内部堆栈上框架的地址的指针。</span><span class="sxs-lookup"><span data-stu-id="901ae-108">[in, out] A pointer to the address of an array of internal frames on the stack.</span></span>  
  
## <a name="return-value"></a><span data-ttu-id="901ae-109">返回值</span><span class="sxs-lookup"><span data-stu-id="901ae-109">Return Value</span></span>  
 <span data-ttu-id="901ae-110">此方法返回以下特定 HRESULT 以及表示方法失败的 HRESULT 错误。</span><span class="sxs-lookup"><span data-stu-id="901ae-110">This method returns the following specific HRESULTs as well as HRESULT errors that indicate method failure.</span></span>  
  
|<span data-ttu-id="901ae-111">HRESULT</span><span class="sxs-lookup"><span data-stu-id="901ae-111">HRESULT</span></span>|<span data-ttu-id="901ae-112">描述</span><span class="sxs-lookup"><span data-stu-id="901ae-112">Description</span></span>|  
|-------------|-----------------|  
|<span data-ttu-id="901ae-113">S_OK</span><span class="sxs-lookup"><span data-stu-id="901ae-113">S_OK</span></span>|<span data-ttu-id="901ae-114">[ICorDebugInternalFrame2](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe2-interface.md)已成功创建对象。</span><span class="sxs-lookup"><span data-stu-id="901ae-114">The [ICorDebugInternalFrame2](../../../../docs/framework/unmanaged-api/debugging/icordebuginternalframe2-interface.md) object was successfully created.</span></span>|  
|<span data-ttu-id="901ae-115">E_INVALIDARG</span><span class="sxs-lookup"><span data-stu-id="901ae-115">E_INVALIDARG</span></span>|<span data-ttu-id="901ae-116">`cInternalFrames`不为零和`ppInternalFrames`是`null`，或`pcInternalFrames`是`null`。</span><span class="sxs-lookup"><span data-stu-id="901ae-116">`cInternalFrames` is not zero and `ppInternalFrames` is `null`, or `pcInternalFrames` is `null`.</span></span>|  
|<span data-ttu-id="901ae-117">HRESULT_FROM_WIN32(ERROR_INSUFFICIENT_BUFFER)</span><span class="sxs-lookup"><span data-stu-id="901ae-117">HRESULT_FROM_WIN32(ERROR_INSUFFICIENT_BUFFER)</span></span>|<span data-ttu-id="901ae-118">`ppInternalFrames`小于内部帧的计数。</span><span class="sxs-lookup"><span data-stu-id="901ae-118">`ppInternalFrames` is smaller than the count of internal frames.</span></span>|  
  
## <a name="exceptions"></a><span data-ttu-id="901ae-119">异常</span><span class="sxs-lookup"><span data-stu-id="901ae-119">Exceptions</span></span>  
  
## <a name="remarks"></a><span data-ttu-id="901ae-120">备注</span><span class="sxs-lookup"><span data-stu-id="901ae-120">Remarks</span></span>  
 <span data-ttu-id="901ae-121">内部帧是推送到堆栈由运行时存储临时数据的数据结构。</span><span class="sxs-lookup"><span data-stu-id="901ae-121">Internal frames are data structures pushed onto the stack by the runtime to store temporary data.</span></span>  
  
 <span data-ttu-id="901ae-122">当你第一次调用`GetActiveInternalFrames`，应设置`cInternalFrames`参数设为 0 （零），和`ppInternalFrames`参数为 null。</span><span class="sxs-lookup"><span data-stu-id="901ae-122">When you first call `GetActiveInternalFrames`, you should set the `cInternalFrames` parameter to 0 (zero), and the `ppInternalFrames` parameter to null.</span></span> <span data-ttu-id="901ae-123">当`GetActiveInternalFrames`首先返回，`pcInternalFrames`包含在堆栈上的内部帧的计数。</span><span class="sxs-lookup"><span data-stu-id="901ae-123">When `GetActiveInternalFrames` first returns, `pcInternalFrames` contains the count of the internal frames on the stack.</span></span>  
  
 <span data-ttu-id="901ae-124">`GetActiveInternalFrames`然后应可以调用第二次。</span><span class="sxs-lookup"><span data-stu-id="901ae-124">`GetActiveInternalFrames` should then be called a second time.</span></span> <span data-ttu-id="901ae-125">应传递适当的计数 (`pcInternalFrames`) 中`cInternalFrames`参数，并指定指向数组中的相应大小的`ppInternalFrames`。</span><span class="sxs-lookup"><span data-stu-id="901ae-125">You should pass the proper count (`pcInternalFrames`) in the `cInternalFrames` parameter, and specify a pointer to an appropriately sized array in `ppInternalFrames`.</span></span>  
  
 <span data-ttu-id="901ae-126">使用[icordebugstackwalk:: Getframe](../../../../docs/framework/unmanaged-api/debugging/icordebugthread3-getactiveinternalframes-method.md)方法以返回实际堆栈帧。</span><span class="sxs-lookup"><span data-stu-id="901ae-126">Use the [ICorDebugStackWalk::GetFrame](../../../../docs/framework/unmanaged-api/debugging/icordebugthread3-getactiveinternalframes-method.md) method to return actual stack frames.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="901ae-127">要求</span><span class="sxs-lookup"><span data-stu-id="901ae-127">Requirements</span></span>  
 <span data-ttu-id="901ae-128">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="901ae-128">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="901ae-129">**标头：** CorDebug.idl、 CorDebug.h</span><span class="sxs-lookup"><span data-stu-id="901ae-129">**Header:** CorDebug.idl, CorDebug.h</span></span>  
  
 <span data-ttu-id="901ae-130">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="901ae-130">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="901ae-131">**.NET framework 版本：**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="901ae-131">**.NET Framework Versions:** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="901ae-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="901ae-132">See Also</span></span>  
 [<span data-ttu-id="901ae-133">调试接口</span><span class="sxs-lookup"><span data-stu-id="901ae-133">Debugging Interfaces</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-interfaces.md)  
 [<span data-ttu-id="901ae-134">调试</span><span class="sxs-lookup"><span data-stu-id="901ae-134">Debugging</span></span>](../../../../docs/framework/unmanaged-api/debugging/index.md)