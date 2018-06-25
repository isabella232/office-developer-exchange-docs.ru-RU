---
title: RemoveDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: Элемент RemoveDelegateResponse содержит состояние и результат операции запроса RemoveDelegate.
ms.openlocfilehash: 45d0bcfaeb4d453f50cce8449f5cb7fdb70512a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835092"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="38da2-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="38da2-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="38da2-104">Элемент **RemoveDelegateResponse** содержит состояние и результат [операции RemoveDelegate](removedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="38da2-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="38da2-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="38da2-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38da2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38da2-106">Attributes and elements</span></span>

<span data-ttu-id="38da2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="38da2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38da2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38da2-108">Attributes</span></span>

<span data-ttu-id="38da2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="38da2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38da2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38da2-110">Child elements</span></span>

|<span data-ttu-id="38da2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38da2-111">**Element**</span></span>|<span data-ttu-id="38da2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38da2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38da2-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="38da2-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="38da2-114">Содержит сообщения ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="38da2-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="38da2-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="38da2-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="38da2-116">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="38da2-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="38da2-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38da2-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="38da2-118">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="38da2-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="38da2-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="38da2-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="38da2-120">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="38da2-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="38da2-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="38da2-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="38da2-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="38da2-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="38da2-123">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="38da2-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38da2-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38da2-124">Parent elements</span></span>

<span data-ttu-id="38da2-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="38da2-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38da2-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="38da2-126">Remarks</span></span>

<span data-ttu-id="38da2-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="38da2-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38da2-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38da2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38da2-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38da2-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38da2-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38da2-130">Schema Name</span></span>  <br/> |<span data-ttu-id="38da2-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="38da2-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38da2-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38da2-132">Validation File</span></span>  <br/> |<span data-ttu-id="38da2-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38da2-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38da2-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38da2-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="38da2-135">False</span><span class="sxs-lookup"><span data-stu-id="38da2-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38da2-136">См. также</span><span class="sxs-lookup"><span data-stu-id="38da2-136">See also</span></span>



[<span data-ttu-id="38da2-137">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="38da2-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="38da2-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38da2-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

