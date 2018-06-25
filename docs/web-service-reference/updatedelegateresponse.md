---
title: UpdateDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: Элемент UpdateDelegateResponse содержит состояние и результат операции запроса UpdateDelegate.
ms.openlocfilehash: b90dd7d8011cf75831481b8f2b92df80d9a67d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840310"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="3934a-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="3934a-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="3934a-104">Элемент **UpdateDelegateResponse** содержит состояние и результат [операции UpdateDelegate](updatedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="3934a-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="3934a-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3934a-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3934a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3934a-106">Attributes and elements</span></span>

<span data-ttu-id="3934a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3934a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3934a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3934a-108">Attributes</span></span>

<span data-ttu-id="3934a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3934a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3934a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3934a-110">Child elements</span></span>

|<span data-ttu-id="3934a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3934a-111">**Element**</span></span>|<span data-ttu-id="3934a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3934a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3934a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="3934a-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="3934a-114">Содержит сообщения ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3934a-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="3934a-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="3934a-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3934a-116">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="3934a-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3934a-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3934a-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3934a-118">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="3934a-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3934a-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3934a-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3934a-120">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="3934a-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3934a-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3934a-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3934a-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3934a-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3934a-123">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="3934a-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3934a-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3934a-124">Parent elements</span></span>

<span data-ttu-id="3934a-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="3934a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3934a-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="3934a-126">Remarks</span></span>

<span data-ttu-id="3934a-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3934a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3934a-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3934a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3934a-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3934a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3934a-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3934a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3934a-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3934a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3934a-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3934a-132">Validation File</span></span>  <br/> |<span data-ttu-id="3934a-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3934a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3934a-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3934a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3934a-135">False</span><span class="sxs-lookup"><span data-stu-id="3934a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3934a-136">См. также</span><span class="sxs-lookup"><span data-stu-id="3934a-136">See also</span></span>



[<span data-ttu-id="3934a-137">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="3934a-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="3934a-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3934a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

