---
title: "调试全局静态函数"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
helpviewer_keywords:
- global static functions [.NET Framework debugging]
- debugging global static functions [.NET Framework]
- unmanaged global static functions [.NET Framework], debugging
ms.assetid: efc64414-77c3-48d0-881a-8594ed416aad
caps.latest.revision: "11"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: ad5d3ef689a251ea4b154afc5d1bfb387388ddb3
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="debugging-global-static-functions"></a><span data-ttu-id="12a9e-102">调试全局静态函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-102">Debugging Global Static Functions</span></span>
<span data-ttu-id="12a9e-103">本节介绍了调试 API 使用的非托管全局静态函数。</span><span class="sxs-lookup"><span data-stu-id="12a9e-103">This section describes the unmanaged global static functions that the debugging API uses.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="12a9e-104">本节内容</span><span class="sxs-lookup"><span data-stu-id="12a9e-104">In This Section</span></span>  
 [<span data-ttu-id="12a9e-105">_EFN_GetManagedExcepStack 函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-105">_EFN_GetManagedExcepStack Function</span></span>](../../../../docs/framework/unmanaged-api/debugging/efn-getmanagedexcepstack-function.md)  
 <span data-ttu-id="12a9e-106">给定托管的异常对象地址后，将返回其中包含的堆栈跟踪的字符串版本。</span><span class="sxs-lookup"><span data-stu-id="12a9e-106">Given a managed exception object address, returns a string version of the stack trace contained inside.</span></span>  
  
 [<span data-ttu-id="12a9e-107">_EFN_GetManagedObjectFieldInfo 函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-107">_EFN_GetManagedObjectFieldInfo Function</span></span>](../../../../docs/framework/unmanaged-api/debugging/efn-getmanagedobjectfieldinfo-function.md)  
 <span data-ttu-id="12a9e-108">使用提供的对象指针和字段名，获取从对象的开头到字段和字段值的偏移量。</span><span class="sxs-lookup"><span data-stu-id="12a9e-108">Gets the offset from the start of an object to a field and the field's value, using the provided object pointer and field name.</span></span>  
  
 [<span data-ttu-id="12a9e-109">_EFN_GetManagedObjectName 函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-109">_EFN_GetManagedObjectName Function</span></span>](../../../../docs/framework/unmanaged-api/debugging/efn-getmanagedobjectname-function.md)  
 <span data-ttu-id="12a9e-110">通过使用提供的托管对象指针获取类型名称。</span><span class="sxs-lookup"><span data-stu-id="12a9e-110">Gets the name of a type by using the provided managed object pointer.</span></span>  
  
 [<span data-ttu-id="12a9e-111">_EFN_StackTrace 函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-111">_EFN_StackTrace Function</span></span>](../../../../docs/framework/unmanaged-api/debugging/efn-stacktrace-function.md)  
 <span data-ttu-id="12a9e-112">提供托管堆栈跟踪的文本表示形式以及 `CONTEXT` 记录的数组，其中每项对应非托管代码和托管代码之间的每个转换。</span><span class="sxs-lookup"><span data-stu-id="12a9e-112">Provides a text representation of a managed stack trace and an array of `CONTEXT` records, one for each transition between unmanaged and managed code.</span></span>  
  
 [<span data-ttu-id="12a9e-113">CLRDataCreateInstance 函数</span><span class="sxs-lookup"><span data-stu-id="12a9e-113">CLRDataCreateInstance Function</span></span>](../../../../docs/framework/unmanaged-api/debugging/clrdatacreateinstance-function.md)  
 <span data-ttu-id="12a9e-114">由公共语言运行时 (CLR) 数据访问服务调用，用于创建指定目标进程的指定接口对象。</span><span class="sxs-lookup"><span data-stu-id="12a9e-114">Called by the common language runtime (CLR) data access services to create the specified interface object for the specified target process.</span></span>  
  
 [<span data-ttu-id="12a9e-115">PFN_CLRDataCreateInstance 函数指针</span><span class="sxs-lookup"><span data-stu-id="12a9e-115">PFN_CLRDataCreateInstance Function Pointer</span></span>](../../../../docs/framework/unmanaged-api/debugging/pfn-clrdatacreateinstance-function-pointer.md)  
 <span data-ttu-id="12a9e-116">指向 CLR 数据访问服务调用来创建指定目标进程的指定接口对象的函数。</span><span class="sxs-lookup"><span data-stu-id="12a9e-116">Points to a function that is called by the CLR data access services to create the specified interface object for the specified target process.</span></span>  
  
## <a name="related-sections"></a><span data-ttu-id="12a9e-117">相关章节</span><span class="sxs-lookup"><span data-stu-id="12a9e-117">Related Sections</span></span>  
 [<span data-ttu-id="12a9e-118">调试组件类</span><span class="sxs-lookup"><span data-stu-id="12a9e-118">Debugging Coclasses</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-coclasses.md)  
  
 [<span data-ttu-id="12a9e-119">调试接口</span><span class="sxs-lookup"><span data-stu-id="12a9e-119">Debugging Interfaces</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-interfaces.md)  
  
 [<span data-ttu-id="12a9e-120">调试枚举</span><span class="sxs-lookup"><span data-stu-id="12a9e-120">Debugging Enumerations</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-enumerations.md)  
  
 [<span data-ttu-id="12a9e-121">调试结构</span><span class="sxs-lookup"><span data-stu-id="12a9e-121">Debugging Structures</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-structures.md)