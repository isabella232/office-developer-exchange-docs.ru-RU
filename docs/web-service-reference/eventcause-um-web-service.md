---
title: EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: Элемент EventCause содержит значение, указывающее, вызвавшего событие звонок в ответ на запрос GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762393"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="ede37-103">EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-103">EventCause (UM web service)</span></span>

<span data-ttu-id="ede37-104">Элемент **EventCause** содержит значение, указывающее, вызвавшего событие звонок в ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="ede37-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="ede37-105">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="ede37-106">EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="ede37-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="ede37-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ede37-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ede37-108">Attributes and elements</span></span>

<span data-ttu-id="ede37-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ede37-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ede37-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ede37-110">Attributes</span></span>

<span data-ttu-id="ede37-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ede37-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ede37-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ede37-112">Child elements</span></span>

<span data-ttu-id="ede37-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ede37-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ede37-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ede37-114">Parent elements</span></span>

|<span data-ttu-id="ede37-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ede37-115">**Element**</span></span>|<span data-ttu-id="ede37-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ede37-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ede37-117">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="ede37-118">Определяет ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="ede37-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ede37-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ede37-119">Text value</span></span>

<span data-ttu-id="ede37-120">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ede37-120">A text value is required.</span></span> <span data-ttu-id="ede37-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="ede37-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="ede37-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ede37-122">None</span></span>
    
- <span data-ttu-id="ede37-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="ede37-123">UserBusy</span></span>
    
- <span data-ttu-id="ede37-124">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="ede37-124">NoAnswer</span></span>
    
- <span data-ttu-id="ede37-125">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="ede37-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="ede37-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ede37-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ede37-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ede37-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ede37-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ede37-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ede37-129">Сообщения</span><span class="sxs-lookup"><span data-stu-id="ede37-129">Messages</span></span>  <br/> |
|<span data-ttu-id="ede37-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ede37-130">Validation File</span></span>  <br/> |<span data-ttu-id="ede37-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ede37-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ede37-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ede37-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ede37-133">False</span><span class="sxs-lookup"><span data-stu-id="ede37-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ede37-134">См. также</span><span class="sxs-lookup"><span data-stu-id="ede37-134">See also</span></span>



[<span data-ttu-id="ede37-135">Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="ede37-136">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="ede37-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

