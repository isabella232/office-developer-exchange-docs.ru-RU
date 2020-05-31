---
title: Евенткаусе (веб-служба единой системы обмена сообщениями)
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
description: Элемент Евенткаусе содержит значение, указывающее причину события Call в ответе на запрос веб-службы единой системы обмена сообщениями GetCallInfo.
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762393"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="7605f-103">Евенткаусе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-103">EventCause (UM web service)</span></span>

<span data-ttu-id="7605f-104">Элемент **евенткаусе** содержит значение, указывающее причину события Call в ответе на запрос [веб-службы единой системы обмена сообщениями GetCallInfo](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="7605f-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="7605f-105">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="7605f-106">Евенткаусе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="7605f-107">**умевенткаусе**</span><span class="sxs-lookup"><span data-stu-id="7605f-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7605f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7605f-108">Attributes and elements</span></span>

<span data-ttu-id="7605f-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7605f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7605f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7605f-110">Attributes</span></span>

<span data-ttu-id="7605f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7605f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7605f-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7605f-112">Child elements</span></span>

<span data-ttu-id="7605f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="7605f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7605f-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7605f-114">Parent elements</span></span>

|<span data-ttu-id="7605f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7605f-115">**Element**</span></span>|<span data-ttu-id="7605f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7605f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7605f-117">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="7605f-118">Определяет ответ на запрос [GetCallInfoной операции (веб-службы единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="7605f-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7605f-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7605f-119">Text value</span></span>

<span data-ttu-id="7605f-120">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7605f-120">A text value is required.</span></span> <span data-ttu-id="7605f-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="7605f-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="7605f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="7605f-122">None</span></span>
    
- <span data-ttu-id="7605f-123">усербуси</span><span class="sxs-lookup"><span data-stu-id="7605f-123">UserBusy</span></span>
    
- <span data-ttu-id="7605f-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="7605f-124">NoAnswer</span></span>
    
- <span data-ttu-id="7605f-125">Другое</span><span class="sxs-lookup"><span data-stu-id="7605f-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="7605f-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7605f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7605f-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7605f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7605f-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7605f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7605f-129">Сообщения</span><span class="sxs-lookup"><span data-stu-id="7605f-129">Messages</span></span>  <br/> |
|<span data-ttu-id="7605f-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7605f-130">Validation File</span></span>  <br/> |<span data-ttu-id="7605f-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7605f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7605f-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7605f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7605f-133">False</span><span class="sxs-lookup"><span data-stu-id="7605f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7605f-134">См. также</span><span class="sxs-lookup"><span data-stu-id="7605f-134">See also</span></span>



[<span data-ttu-id="7605f-135">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="7605f-136">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7605f-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

