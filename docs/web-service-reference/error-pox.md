---
title: Ошибка (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Элемент Error содержит ответ об ошибке автообнаружения.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530651"
---
# <a name="error-pox"></a><span data-ttu-id="a5b7c-103">Ошибка (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-103">Error (POX)</span></span>

<span data-ttu-id="a5b7c-104">Элемент **Error** содержит ответ об ошибке автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="a5b7c-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a5b7c-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a5b7c-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a5b7c-108">Ошибка (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a5b7c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5b7c-109">Attributes and elements</span></span>

<span data-ttu-id="a5b7c-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5b7c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5b7c-111">Attributes</span></span>

|<span data-ttu-id="a5b7c-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-112">**Attribute**</span></span>|<span data-ttu-id="a5b7c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5b7c-114">Time</span><span class="sxs-lookup"><span data-stu-id="a5b7c-114">Time</span></span>  <br/> |<span data-ttu-id="a5b7c-115">Представляет время, когда был возвращен ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="a5b7c-116">Id</span><span class="sxs-lookup"><span data-stu-id="a5b7c-116">Id</span></span>  <br/> |<span data-ttu-id="a5b7c-117">Представляет хэш имени компьютера, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a5b7c-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5b7c-118">Child elements</span></span>

|<span data-ttu-id="a5b7c-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-119">**Element**</span></span>|<span data-ttu-id="a5b7c-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5b7c-121">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="a5b7c-122">Содержит код ошибки для ответа на автообнаружение ошибок.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="a5b7c-123">Сообщение (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="a5b7c-124">Содержит сообщение об ошибке для ответа на автообнаружение ошибок.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="a5b7c-125">Дебугдата (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="a5b7c-126">Содержит данные отладки для отклика автообнаружения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5b7c-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5b7c-127">Parent elements</span></span>

|<span data-ttu-id="a5b7c-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-128">**Element**</span></span>|<span data-ttu-id="a5b7c-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5b7c-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5b7c-130">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a5b7c-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="a5b7c-131">Содержит ответ об ошибке автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a5b7c-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5b7c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a5b7c-132">See also</span></span>



[<span data-ttu-id="a5b7c-133">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a5b7c-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

