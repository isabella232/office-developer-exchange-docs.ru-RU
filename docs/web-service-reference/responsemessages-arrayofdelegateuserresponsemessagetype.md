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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="81c14-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="81c14-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="81c14-104">Элемент **ResponseMessages** содержит сообщений ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="81c14-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="81c14-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="81c14-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81c14-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81c14-106">Attributes and elements</span></span>

<span data-ttu-id="81c14-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="81c14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81c14-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81c14-108">Attributes</span></span>

<span data-ttu-id="81c14-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="81c14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81c14-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81c14-110">Child elements</span></span>

|<span data-ttu-id="81c14-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c14-111">**Element**</span></span>|<span data-ttu-id="81c14-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c14-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="81c14-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="81c14-114">Содержит сообщения ответа для операции управления delegate.</span><span class="sxs-lookup"><span data-stu-id="81c14-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81c14-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81c14-115">Parent elements</span></span>

|<span data-ttu-id="81c14-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c14-116">**Element**</span></span>|<span data-ttu-id="81c14-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c14-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c14-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="81c14-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="81c14-119">Содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="81c14-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="81c14-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="81c14-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="81c14-121">Содержит состояние и результат [операции GetDelegate](getdelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="81c14-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="81c14-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="81c14-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="81c14-123">Содержит состояние и результат [операции UpdateDelegate](updatedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="81c14-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="81c14-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="81c14-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="81c14-125">Содержит состояние и результат [операции RemoveDelegate](removedelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="81c14-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81c14-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="81c14-126">Remarks</span></span>

<span data-ttu-id="81c14-127">Данный элемент используется в [операции AddDelegate](adddelegate-operation.md), [GetDelegate операции](getdelegate-operation.md), [операция UpdateDelegate](updatedelegate-operation.md)и [RemoveDelegate операции](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="81c14-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="81c14-128">Ответы операции управления delegate структурированы иначе, чем другие ответы.</span><span class="sxs-lookup"><span data-stu-id="81c14-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="81c14-129">Сообщения ответа управления delegate строго типизированный.</span><span class="sxs-lookup"><span data-stu-id="81c14-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="81c14-130">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="81c14-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81c14-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81c14-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81c14-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81c14-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81c14-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81c14-133">Schema Name</span></span>  <br/> |<span data-ttu-id="81c14-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="81c14-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="81c14-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81c14-135">Validation File</span></span>  <br/> |<span data-ttu-id="81c14-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81c14-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81c14-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81c14-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="81c14-138">False</span><span class="sxs-lookup"><span data-stu-id="81c14-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81c14-139">См. также</span><span class="sxs-lookup"><span data-stu-id="81c14-139">See also</span></span>



[<span data-ttu-id="81c14-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="81c14-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="81c14-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="81c14-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="81c14-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="81c14-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="81c14-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="81c14-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="81c14-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="81c14-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

