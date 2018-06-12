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
description: Элемент ошибки содержит возврату ошибки службы автообнаружения.
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762376"
---
# <a name="error-pox"></a><span data-ttu-id="0c3d4-103">Ошибка (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-103">Error (POX)</span></span>

<span data-ttu-id="0c3d4-104">Элемент **ошибки** содержит возврату ошибки службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="0c3d4-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0c3d4-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0c3d4-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0c3d4-108">Ошибка (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0c3d4-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c3d4-109">Attributes and elements</span></span>

<span data-ttu-id="0c3d4-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c3d4-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c3d4-111">Attributes</span></span>

|<span data-ttu-id="0c3d4-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-112">**Attribute**</span></span>|<span data-ttu-id="0c3d4-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c3d4-114">Время</span><span class="sxs-lookup"><span data-stu-id="0c3d4-114">Time</span></span>  <br/> |<span data-ttu-id="0c3d4-115">Представляет время, когда была возвращена ошибка ответа.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="0c3d4-116">Id</span><span class="sxs-lookup"><span data-stu-id="0c3d4-116">Id</span></span>  <br/> |<span data-ttu-id="0c3d4-117">Представляет хэш-имя компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0c3d4-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c3d4-118">Child elements</span></span>

|<span data-ttu-id="0c3d4-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-119">**Element**</span></span>|<span data-ttu-id="0c3d4-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c3d4-121">Код ошибки (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="0c3d4-122">Содержит код ошибки для ошибки ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="0c3d4-123">Сообщение (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="0c3d4-124">Содержит сообщение об ошибке Ошибка ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="0c3d4-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="0c3d4-126">Содержит данные отладки при возникновении ошибки ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c3d4-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c3d4-127">Parent elements</span></span>

|<span data-ttu-id="0c3d4-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-128">**Element**</span></span>|<span data-ttu-id="0c3d4-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c3d4-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c3d4-130">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="0c3d4-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="0c3d4-131">Содержит возврату ошибки службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0c3d4-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c3d4-132">См. также</span><span class="sxs-lookup"><span data-stu-id="0c3d4-132">See also</span></span>



[<span data-ttu-id="0c3d4-133">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="0c3d4-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

