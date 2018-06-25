---
title: CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: Элемент CallState содержит значение, указывающее состояние звонка.
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761663"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="16712-103">CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-103">CallState (UM web service)</span></span>

<span data-ttu-id="16712-104">Элемент **CallState** содержит значение, указывающее состояние звонка.</span><span class="sxs-lookup"><span data-stu-id="16712-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="16712-105">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="16712-106">CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="16712-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="16712-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16712-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16712-108">Attributes and elements</span></span>

<span data-ttu-id="16712-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="16712-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16712-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16712-110">Attributes</span></span>

<span data-ttu-id="16712-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="16712-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16712-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16712-112">Child elements</span></span>

<span data-ttu-id="16712-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="16712-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16712-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16712-114">Parent elements</span></span>

|<span data-ttu-id="16712-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16712-115">**Element**</span></span>|<span data-ttu-id="16712-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16712-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16712-117">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="16712-118">Определяет ответ на [операцию GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="16712-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16712-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="16712-119">Text value</span></span>

<span data-ttu-id="16712-120">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="16712-120">A text value is required.</span></span> <span data-ttu-id="16712-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="16712-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="16712-122">Простоя</span><span class="sxs-lookup"><span data-stu-id="16712-122">Idle</span></span>
    
- <span data-ttu-id="16712-123">Подключение</span><span class="sxs-lookup"><span data-stu-id="16712-123">Connecting</span></span>
    
- <span data-ttu-id="16712-124">Оповещения</span><span class="sxs-lookup"><span data-stu-id="16712-124">Alerted</span></span>
    
- <span data-ttu-id="16712-125">Подключено</span><span class="sxs-lookup"><span data-stu-id="16712-125">Connected</span></span>
    
- <span data-ttu-id="16712-126">Отключено</span><span class="sxs-lookup"><span data-stu-id="16712-126">Disconnected</span></span>
    
- <span data-ttu-id="16712-127">Входящая</span><span class="sxs-lookup"><span data-stu-id="16712-127">Incoming</span></span>
    
- <span data-ttu-id="16712-128">Передача</span><span class="sxs-lookup"><span data-stu-id="16712-128">Transferring</span></span>
    
- <span data-ttu-id="16712-129">Переадресация</span><span class="sxs-lookup"><span data-stu-id="16712-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="16712-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16712-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16712-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16712-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="16712-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16712-132">Schema Name</span></span>  <br/> |<span data-ttu-id="16712-133">Сообщения</span><span class="sxs-lookup"><span data-stu-id="16712-133">Messages</span></span>  <br/> |
|<span data-ttu-id="16712-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16712-134">Validation File</span></span>  <br/> |<span data-ttu-id="16712-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16712-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16712-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16712-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="16712-137">False</span><span class="sxs-lookup"><span data-stu-id="16712-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16712-138">См. также</span><span class="sxs-lookup"><span data-stu-id="16712-138">See also</span></span>



[<span data-ttu-id="16712-139">Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="16712-140">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="16712-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

