---
title: CorElementType Enumeration1
ms.date: 03/30/2017
api_name:
- CorElementType
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- CorElementType
helpviewer_keywords:
- CorElementType enumeration [.NET Framework metadata]
ms.assetid: c3809c8f-1737-4f0f-9442-0c01ee689871
topic_type:
- apiref
author: mairaw
ms.author: mairaw
ms.openlocfilehash: ebe2cf95f5637e6924b85c2389f1c59679580298
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="corelementtype-enumeration1"></a>CorElementType Enumeration1
指定公共语言运行时<xref:System.Type>、 类型修饰符，或者有关元数据类型签名中类型的信息。  
  
## <a name="syntax"></a>语法  
  
```  
typedef enum CorElementType {  
    ELEMENT_TYPE_END            = 0x0,  
    ELEMENT_TYPE_VOID           = 0x1,  
    ELEMENT_TYPE_BOOLEAN        = 0x2,  
    ELEMENT_TYPE_CHAR           = 0x3,  
    ELEMENT_TYPE_I1             = 0x4,  
    ELEMENT_TYPE_U1             = 0x5,  
    ELEMENT_TYPE_I2             = 0x6,  
    ELEMENT_TYPE_U2             = 0x7,  
    ELEMENT_TYPE_I4             = 0x8,  
    ELEMENT_TYPE_U4             = 0x9,  
    ELEMENT_TYPE_I8             = 0xa,  
    ELEMENT_TYPE_U8             = 0xb,  
    ELEMENT_TYPE_R4             = 0xc,  
    ELEMENT_TYPE_R8             = 0xd,  
    ELEMENT_TYPE_STRING         = 0xe,  
  
    ELEMENT_TYPE_PTR            = 0xf,  
    ELEMENT_TYPE_BYREF          = 0x10,  
  
    ELEMENT_TYPE_VALUETYPE      = 0x11,  
    ELEMENT_TYPE_CLASS          = 0x12,  
    ELEMENT_TYPE_VAR            = 0x13,  
    ELEMENT_TYPE_ARRAY          = 0x14,  
    ELEMENT_TYPE_GENERICINST    = 0x15,  
    ELEMENT_TYPE_TYPEDBYREF     = 0x16,  
  
    ELEMENT_TYPE_I              = 0x18,  
    ELEMENT_TYPE_U              = 0x19,  
    ELEMENT_TYPE_FNPTR          = 0x1B,  
    ELEMENT_TYPE_OBJECT         = 0x1C,  
    ELEMENT_TYPE_SZARRAY        = 0x1D,  
    ELEMENT_TYPE_MVAR           = 0x1e,  
  
    ELEMENT_TYPE_CMOD_REQD      = 0x1F,  
    ELEMENT_TYPE_CMOD_OPT       = 0x20,  
  
    ELEMENT_TYPE_INTERNAL       = 0x21,  
    ELEMENT_TYPE_MAX            = 0x22,  
  
    ELEMENT_TYPE_MODIFIER       = 0x40,  
    ELEMENT_TYPE_SENTINEL       = 0x01 | ELEMENT_TYPE_MODIFIER,  
    ELEMENT_TYPE_PINNED         = 0x05 | ELEMENT_TYPE_MODIFIER  
  
} CorElementType;  
```  
  
## <a name="members"></a>成员  
  
|成员|描述|  
|------------|-----------------|  
|`ELEMENT_TYPE_END`|内部使用。|  
|`ELEMENT_TYPE_VOID`|Void 类型。|  
|`ELEMENT_TYPE_BOOLEAN`|布尔值类型|  
|`ELEMENT_TYPE_CHAR`|一个字符类型。|  
|`ELEMENT_TYPE_I1`|一个带符号的 1 字节整数。|  
|`ELEMENT_TYPE_U1`|1 字节无符号整数。|  
|`ELEMENT_TYPE_I2`|一个带符号的 2 字节整数。|  
|`ELEMENT_TYPE_U2`|无符号的 2 字节整数。|  
|`ELEMENT_TYPE_I4`|一个带符号的 4 字节整数。|  
|`ELEMENT_TYPE_U4`|无符号的 4 字节整数。|  
|`ELEMENT_TYPE_I8`|一个带符号的 8 字节整数。|  
|`ELEMENT_TYPE_U8`|无符号的 8 字节整数。|  
|`ELEMENT_TYPE_R4`|4 字节的浮点数。|  
|`ELEMENT_TYPE_R8`|8 字节浮点。|  
|`ELEMENT_TYPE_STRING`|System.String 类型。|  
|`ELEMENT_TYPE_PTR`|指针类型修饰符。|  
|`ELEMENT_TYPE_BYREF`|引用类型修饰符。|  
|`ELEMENT_TYPE_VALUETYPE`|值类型修饰符。|  
|`ELEMENT_TYPE_CLASS`|类类型修饰符。|  
|`ELEMENT_TYPE_VAR`|类变量的类型修饰符。|  
|`ELEMENT_TYPE_ARRAY`|多维数组类型修饰符。|  
|`ELEMENT_TYPE_GENERICINST`|泛型类型的类型修饰符。|  
|`ELEMENT_TYPE_TYPEDBYREF`|类型化的引用。|  
|`ELEMENT_TYPE_I`|本机整数的大小。|  
|`ELEMENT_TYPE_U`|本机的无符号整数的大小。|  
|`ELEMENT_TYPE_FNPTR`|指向函数的指针。|  
|`ELEMENT_TYPE_OBJECT`|一种 System.Object 类型。|  
|`ELEMENT_TYPE_SZARRAY`|一维、 零的下限数组的类型修饰符。|  
|`ELEMENT_TYPE_MVAR`|方法变量的类型修饰符。|  
|`ELEMENT_TYPE_CMOD_REQD`|C 语言必需的修饰符。|  
|`ELEMENT_TYPE_CMOD_OPT`|C 语言可选修饰符。|  
|`ELEMENT_TYPE_INTERNAL`|内部使用。|  
|`ELEMENT_TYPE_MAX`|无效类型。|  
|`ELEMENT_TYPE_MODIFIER`|内部使用。|  
|`ELEMENT_TYPE_SENTINEL`|类型修饰符，有关的可变数目的参数列表 sentinel。|  
|`ELEMENT_TYPE_PINNED`|内部使用。|  
  
## <a name="remarks"></a>备注  
 类型修饰符构成表示更复杂的类型的基础。 A`CorElementType`类型修饰符值应用于类型签名中紧随该项的值。 之后的值`CorElementType`类型修饰符值可以是`CorElementType`简单类型值、 元数据标记或其他值，指定下表中。  
  
> [!NOTE]
>  所有数字 (*数*，*自变量计数*，*元数据标记*，*级别*，*计数*，和*绑定*) 都存储为压缩的整数。 请参阅[标准 ecma-335-公共语言基础结构 (CLI)](http://go.microsoft.com/fwlink/?LinkID=116487) ECMA 网站有关的详细信息上。  
  
|类型修饰符|格式|  
|-------------------|------------|  
|`ELEMENT_TYPE_PTR`|ELEMENT_TYPE_PTR <`CorElementType`值 >|  
|`ELEMENT_TYPE_BYREF`|ELEMENT_TYPE_BYREF <`CorElementType`值 >|  
|`ELEMENT_TYPE_VALUETYPE`|ELEMENT_TYPE_VALUETYPE <`mdTypeDef`元数据令牌 >|  
|`ELEMENT_TYPE_CLASS`|ELEMENT_TYPE_CLASS <`mdTypeDef`元数据令牌 >|  
|`ELEMENT_TYPE_VAR`|ELEMENT_TYPE_VAR\<数量 >|  
|`ELEMENT_TYPE_ARRAY`|ELEMENT_TYPE_ARRAY <`CorElementType`值 >\<级别 > \<count1 > \<bound1 >...\<countN > \<boundN >|  
|`ELEMENT_TYPE_GENERICINST`|ELEMENT_TYPE_GENERICINST <`mdTypeDef`元数据标记 >\<自变量计数 > \<arg1 >...\<argN >|  
|`ELEMENT_TYPE_FNPTR`|ELEMENT_TYPE_FNPTR\<对于函数，包括调用约定的完整签名 >|  
|`ELEMENT_TYPE_SZARRAY`|ELEMENT_TYPE_SZARRAY <`CorElementType`值 >|  
|`ELEMENT_TYPE_MVAR`|ELEMENT_TYPE_MVAR\<数量 >|  
|`ELEMENT_TYPE_CMOD_REQD`|ELEMENT_TYPE_ <`mdTypeRef`或`mdTypeDef`元数据令牌 >|  
|`ELEMENT_TYPE_CMOD_OPT`|E_T_CMOD_OPT <`mdTypeRef`或`mdTypeDef`元数据令牌 >|  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CorHdr.h  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [Metadata 枚举](../../../../docs/framework/unmanaged-api/metadata/metadata-enumerations.md)
