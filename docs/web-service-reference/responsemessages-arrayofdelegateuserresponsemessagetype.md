---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: Элемент ResponseMessages содержит сообщений ответа на запрос управления delegate веб-служб Exchange.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="101c2-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="101c2-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="101c2-104">Элемент **ResponseMessages** содержит сообщений ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="101c2-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="101c2-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="101c2-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="101c2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="101c2-106">Attributes and elements</span></span>

<span data-ttu-id="101c2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="101c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="101c2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="101c2-108">Attributes</span></span>

<span data-ttu-id="101c2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="101c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="101c2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="101c2-110">Child elements</span></span>

|<span data-ttu-id="101c2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="101c2-111">**Element**</span></span>|<span data-ttu-id="101c2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="101c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="101c2-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="101c2-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="101c2-114">Содержит сообщения ответа для операции управления delegate.</span><span class="sxs-lookup"><span data-stu-id="101c2-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="101c2-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="101c2-115">Parent elements</span></span>

|<span data-ttu-id="101c2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="101c2-116">**Element**</span></span>|<span data-ttu-id="101c2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="101c2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="101c2-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="101c2-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="101c2-119">Содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="101c2-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="101c2-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="101c2-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="101c2-121">Содержит состояние и результат [операции GetDelegate](getdelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="101c2-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="101c2-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="101c2-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="101c2-123">Содержит состояние и результат [операции UpdateDelegate](updatedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="101c2-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="101c2-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="101c2-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="101c2-125">Содержит состояние и результат [операции RemoveDelegate](removedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="101c2-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="101c2-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="101c2-126">Remarks</span></span>

<span data-ttu-id="101c2-127">Данный элемент используется в [операции AddDelegate](adddelegate-operation.md), [GetDelegate операции](getdelegate-operation.md), [операция UpdateDelegate](updatedelegate-operation.md)и [RemoveDelegate операции](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="101c2-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="101c2-128">Ответы операции управления delegate структурированы иначе, чем другие ответы.</span><span class="sxs-lookup"><span data-stu-id="101c2-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="101c2-129">Сообщения ответа управления delegate строго типизированный.</span><span class="sxs-lookup"><span data-stu-id="101c2-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="101c2-130">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="101c2-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="101c2-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="101c2-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="101c2-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="101c2-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="101c2-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="101c2-133">Schema Name</span></span>  <br/> |<span data-ttu-id="101c2-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="101c2-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="101c2-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="101c2-135">Validation File</span></span>  <br/> |<span data-ttu-id="101c2-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="101c2-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="101c2-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="101c2-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="101c2-138">False</span><span class="sxs-lookup"><span data-stu-id="101c2-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="101c2-139">См. также</span><span class="sxs-lookup"><span data-stu-id="101c2-139">See also</span></span>



[<span data-ttu-id="101c2-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="101c2-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="101c2-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="101c2-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="101c2-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="101c2-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="101c2-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="101c2-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="101c2-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="101c2-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

