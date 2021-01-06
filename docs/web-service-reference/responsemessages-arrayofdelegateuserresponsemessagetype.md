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
description: Элемент ResponseMessages содержит сообщения ответа для запроса на управление делегированием веб-служб Exchange.
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465459"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="69fcc-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="69fcc-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="69fcc-104">Элемент **ResponseMessages** содержит сообщения ответа для запроса на управление делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="69fcc-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="69fcc-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="69fcc-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69fcc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69fcc-106">Attributes and elements</span></span>

<span data-ttu-id="69fcc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="69fcc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69fcc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69fcc-108">Attributes</span></span>

<span data-ttu-id="69fcc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="69fcc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69fcc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69fcc-110">Child elements</span></span>

|<span data-ttu-id="69fcc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69fcc-111">**Element**</span></span>|<span data-ttu-id="69fcc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69fcc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69fcc-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="69fcc-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="69fcc-114">Содержит ответные сообщения для операций управления делегированием.</span><span class="sxs-lookup"><span data-stu-id="69fcc-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69fcc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69fcc-115">Parent elements</span></span>

|<span data-ttu-id="69fcc-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69fcc-116">**Element**</span></span>|<span data-ttu-id="69fcc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69fcc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69fcc-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="69fcc-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="69fcc-119">Содержит состояние и результат запроса на операцию [AddDelegate.](adddelegate-operation.md)</span><span class="sxs-lookup"><span data-stu-id="69fcc-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="69fcc-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="69fcc-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="69fcc-121">Содержит состояние и результат запроса на операцию [GetDelegate.](getdelegate-operation.md)</span><span class="sxs-lookup"><span data-stu-id="69fcc-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="69fcc-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="69fcc-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="69fcc-123">Содержит состояние и результат запроса [операции UpdateDelegate.](updatedelegate-operation.md)</span><span class="sxs-lookup"><span data-stu-id="69fcc-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="69fcc-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="69fcc-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="69fcc-125">Содержит состояние и результат запроса на операцию [RemoveDelegate.](removedelegate-operation.md)</span><span class="sxs-lookup"><span data-stu-id="69fcc-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69fcc-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="69fcc-126">Remarks</span></span>

<span data-ttu-id="69fcc-127">Этот элемент используется в [операциях AddDelegate,](adddelegate-operation.md) [GetDelegate,](getdelegate-operation.md) [UpdateDelegate](updatedelegate-operation.md)и [RemoveDelegate.](removedelegate-operation.md)</span><span class="sxs-lookup"><span data-stu-id="69fcc-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="69fcc-128">Реакции на операции управления делегированием структурированы иначе, чем другие ответы.</span><span class="sxs-lookup"><span data-stu-id="69fcc-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="69fcc-129">Сообщения ответа на запросы управления делегированием строго типимы.</span><span class="sxs-lookup"><span data-stu-id="69fcc-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="69fcc-130">Схема, описывающую этот элемент, расположена в виртуальном каталоге EWS компьютера, на Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="69fcc-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69fcc-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69fcc-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69fcc-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69fcc-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69fcc-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69fcc-133">Schema Name</span></span>  <br/> |<span data-ttu-id="69fcc-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="69fcc-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69fcc-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69fcc-135">Validation File</span></span>  <br/> |<span data-ttu-id="69fcc-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="69fcc-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69fcc-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69fcc-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="69fcc-138">False</span><span class="sxs-lookup"><span data-stu-id="69fcc-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69fcc-139">См. также</span><span class="sxs-lookup"><span data-stu-id="69fcc-139">See also</span></span>



[<span data-ttu-id="69fcc-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="69fcc-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="69fcc-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="69fcc-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="69fcc-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="69fcc-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="69fcc-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="69fcc-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="69fcc-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="69fcc-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

