---
title: DelegateUserResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUserResponseMessageType
api_type:
- schema
ms.assetid: 3dc9552c-1e2d-40ac-a137-827883c2bb88
description: Элемент DelegateUserResponseMessageType содержит ответное сообщение для одного делегата пользователя.
ms.openlocfilehash: ac99e0ca219fc1f1e117f9288d895e27a1df4700
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762016"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="54ef9-103">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="54ef9-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="54ef9-104">Элемент **DelegateUserResponseMessageType** содержит ответное сообщение для одного делегата пользователя.</span><span class="sxs-lookup"><span data-stu-id="54ef9-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="54ef9-105">**DelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="54ef9-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="54ef9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54ef9-106">Attributes and elements</span></span>

<span data-ttu-id="54ef9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54ef9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54ef9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54ef9-108">Attributes</span></span>

<span data-ttu-id="54ef9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="54ef9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54ef9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54ef9-110">Child elements</span></span>

|<span data-ttu-id="54ef9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54ef9-111">**Element**</span></span>|<span data-ttu-id="54ef9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54ef9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54ef9-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="54ef9-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="54ef9-114">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="54ef9-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="54ef9-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54ef9-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="54ef9-116">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="54ef9-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="54ef9-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="54ef9-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="54ef9-118">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="54ef9-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="54ef9-119">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="54ef9-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="54ef9-120">MessageXml</span><span class="sxs-lookup"><span data-stu-id="54ef9-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="54ef9-121">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="54ef9-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="54ef9-122">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="54ef9-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="54ef9-123">Идентифицирует одного делегата, возвращаемого в ответе управления delegate.</span><span class="sxs-lookup"><span data-stu-id="54ef9-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54ef9-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54ef9-124">Parent elements</span></span>

|<span data-ttu-id="54ef9-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54ef9-125">**Element**</span></span>|<span data-ttu-id="54ef9-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54ef9-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54ef9-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="54ef9-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="54ef9-128">Содержит сообщения ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="54ef9-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54ef9-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="54ef9-129">Remarks</span></span>

<span data-ttu-id="54ef9-130">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="54ef9-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54ef9-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54ef9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54ef9-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54ef9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54ef9-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54ef9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="54ef9-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="54ef9-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54ef9-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54ef9-135">Validation File</span></span>  <br/> |<span data-ttu-id="54ef9-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54ef9-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54ef9-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54ef9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="54ef9-138">False</span><span class="sxs-lookup"><span data-stu-id="54ef9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54ef9-139">См. также</span><span class="sxs-lookup"><span data-stu-id="54ef9-139">See also</span></span>

- [<span data-ttu-id="54ef9-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="54ef9-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="54ef9-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="54ef9-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="54ef9-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="54ef9-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="54ef9-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="54ef9-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="54ef9-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="54ef9-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

