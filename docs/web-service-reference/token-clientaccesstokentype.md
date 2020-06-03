---
title: Маркер (Клиентакцесстокентипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: Элемент Token указывает маркер клиентского доступа.
ms.openlocfilehash: d195e81d8d20eb2288e921c640c7b2898a5341ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467867"
---
# <a name="token-clientaccesstokentype"></a><span data-ttu-id="cce21-103">Маркер (Клиентакцесстокентипе)</span><span class="sxs-lookup"><span data-stu-id="cce21-103">Token (ClientAccessTokenType)</span></span>

<span data-ttu-id="cce21-104">Элемент **Token** указывает маркер клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cce21-104">The **Token** element specifies a client access token.</span></span> 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 <span data-ttu-id="cce21-105">**клиентакцесстокентипе**</span><span class="sxs-lookup"><span data-stu-id="cce21-105">**ClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cce21-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cce21-106">Attributes and elements</span></span>

<span data-ttu-id="cce21-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cce21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cce21-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cce21-108">Attributes</span></span>

<span data-ttu-id="cce21-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cce21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cce21-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cce21-110">Child elements</span></span>

<span data-ttu-id="cce21-111">[ID (строка)](id-string.md)  |  [Токентипе](tokentype.md)  |  [Токенвалуе](tokenvalue.md)  |  [Срок жизни](ttl.md)</span><span class="sxs-lookup"><span data-stu-id="cce21-111">[ID (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cce21-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cce21-112">Parent elements</span></span>

[<span data-ttu-id="cce21-113">жетклиентакцесстокенреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="cce21-113">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="cce21-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="cce21-114">Remarks</span></span>

<span data-ttu-id="cce21-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cce21-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cce21-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cce21-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cce21-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cce21-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cce21-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cce21-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cce21-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cce21-119">Schema name</span></span>  <br/> |<span data-ttu-id="cce21-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cce21-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="cce21-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cce21-121">Validation file</span></span>  <br/> |<span data-ttu-id="cce21-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cce21-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cce21-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cce21-123">Can be empty</span></span>  <br/> ||
   

