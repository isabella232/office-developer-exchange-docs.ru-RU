---
title: Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)
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
description: Элемент Жеткаллинфореспонсе определяет ответ на запрос для операции GetCallInfo (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461207"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="183cc-103">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="183cc-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="183cc-104">Элемент **жеткаллинфореспонсе** определяет ответ на запрос для [операции GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="183cc-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="183cc-105">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="183cc-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="183cc-106">**умкаллинфо**</span><span class="sxs-lookup"><span data-stu-id="183cc-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="183cc-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="183cc-107">Attributes and elements</span></span>

<span data-ttu-id="183cc-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="183cc-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="183cc-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="183cc-109">Attributes</span></span>

<span data-ttu-id="183cc-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="183cc-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="183cc-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="183cc-111">Child elements</span></span>

|<span data-ttu-id="183cc-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="183cc-112">**Element**</span></span>|<span data-ttu-id="183cc-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="183cc-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="183cc-114">каллстате</span><span class="sxs-lookup"><span data-stu-id="183cc-114">CallState</span></span>  <br/> |<span data-ttu-id="183cc-115">Содержит значение, указывающее состояние вызова, для которого требуется [Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="183cc-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="183cc-116">евенткаусе</span><span class="sxs-lookup"><span data-stu-id="183cc-116">EventCause</span></span>  <br/> |<span data-ttu-id="183cc-117">Содержит значение, указывающее причину события для вызова, для которого в [операции GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) запрошены сведения.</span><span class="sxs-lookup"><span data-stu-id="183cc-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="183cc-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="183cc-118">Parent elements</span></span>

<span data-ttu-id="183cc-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="183cc-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="183cc-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="183cc-120">Text value</span></span>

<span data-ttu-id="183cc-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="183cc-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="183cc-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="183cc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="183cc-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="183cc-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="183cc-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="183cc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="183cc-125">Сообщения</span><span class="sxs-lookup"><span data-stu-id="183cc-125">Messages</span></span>  <br/> |
|<span data-ttu-id="183cc-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="183cc-126">Validation File</span></span>  <br/> |<span data-ttu-id="183cc-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="183cc-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="183cc-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="183cc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="183cc-129">False</span><span class="sxs-lookup"><span data-stu-id="183cc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="183cc-130">См. также</span><span class="sxs-lookup"><span data-stu-id="183cc-130">See also</span></span>



[<span data-ttu-id="183cc-131">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="183cc-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="183cc-132">Каллстате (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="183cc-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="183cc-133">Евенткаусе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="183cc-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

