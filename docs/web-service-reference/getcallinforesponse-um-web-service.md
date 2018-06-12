---
title: GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: Элемент GetCallInfoResponse определяет ответа на запрос GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762711"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="8940b-103">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8940b-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="8940b-104">Элемент **GetCallInfoResponse** определяет ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="8940b-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="8940b-105">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8940b-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="8940b-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="8940b-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8940b-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8940b-107">Attributes and elements</span></span>

<span data-ttu-id="8940b-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8940b-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8940b-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8940b-109">Attributes</span></span>

<span data-ttu-id="8940b-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="8940b-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8940b-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8940b-111">Child elements</span></span>

|<span data-ttu-id="8940b-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8940b-112">**Element**</span></span>|<span data-ttu-id="8940b-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8940b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8940b-114">CallState</span><span class="sxs-lookup"><span data-stu-id="8940b-114">CallState</span></span>  <br/> |<span data-ttu-id="8940b-115">Содержит значение, указывающее состояние звонка для которого сведения Запрошенная [операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="8940b-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="8940b-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="8940b-116">EventCause</span></span>  <br/> |<span data-ttu-id="8940b-117">Содержит значение, которое указывает причину события для звонка для которого сведения Запрошенная [операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="8940b-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8940b-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8940b-118">Parent elements</span></span>

<span data-ttu-id="8940b-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="8940b-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8940b-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8940b-120">Text value</span></span>

<span data-ttu-id="8940b-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="8940b-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8940b-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8940b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8940b-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8940b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8940b-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8940b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8940b-125">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8940b-125">Messages</span></span>  <br/> |
|<span data-ttu-id="8940b-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8940b-126">Validation File</span></span>  <br/> |<span data-ttu-id="8940b-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8940b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8940b-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8940b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8940b-129">False</span><span class="sxs-lookup"><span data-stu-id="8940b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8940b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8940b-130">See also</span></span>



[<span data-ttu-id="8940b-131">Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8940b-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="8940b-132">CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8940b-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="8940b-133">EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8940b-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

