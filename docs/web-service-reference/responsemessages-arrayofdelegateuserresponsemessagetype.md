---
title: Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)
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
description: Элемент Респонсемессажес содержит ответные сообщения для запроса на управление делегированием веб-служб Exchange.
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465459"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="bc3d9-103">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="bc3d9-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="bc3d9-104">Элемент **респонсемессажес** содержит ответные сообщения для запроса на управление делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="bc3d9-105">**аррайофделегатеусерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="bc3d9-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc3d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc3d9-106">Attributes and elements</span></span>

<span data-ttu-id="bc3d9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc3d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc3d9-108">Attributes</span></span>

<span data-ttu-id="bc3d9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc3d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc3d9-110">Child elements</span></span>

|<span data-ttu-id="bc3d9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc3d9-111">**Element**</span></span>|<span data-ttu-id="bc3d9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc3d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc3d9-113">делегатеусерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="bc3d9-114">Содержит сообщения ответа для операций управления делегированием.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc3d9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc3d9-115">Parent elements</span></span>

|<span data-ttu-id="bc3d9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc3d9-116">**Element**</span></span>|<span data-ttu-id="bc3d9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc3d9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc3d9-118">аддделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="bc3d9-119">Содержит состояние и результат запроса [операции AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc3d9-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="bc3d9-120">жетделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="bc3d9-121">Содержит состояние и результат запроса [операции Delegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc3d9-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="bc3d9-122">упдатеделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="bc3d9-123">Содержит состояние и результат запроса [операции UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc3d9-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="bc3d9-124">ремоведелегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="bc3d9-125">Содержит состояние и результат запроса [операции RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc3d9-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc3d9-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc3d9-126">Remarks</span></span>

<span data-ttu-id="bc3d9-127">Этот элемент используется в [операции AddDelegate](adddelegate-operation.md), [операции-делегата](getdelegate-operation.md), [операции UpdateDelegate](updatedelegate-operation.md)и [операции RemoveDelegate](removedelegate-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bc3d9-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="bc3d9-128">Отклики операции управления делегированием структурированы иначе, чем другие ответы.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="bc3d9-129">Сообщения ответа управления представителями строго типизированы.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="bc3d9-130">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc3d9-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc3d9-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc3d9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc3d9-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc3d9-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc3d9-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc3d9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bc3d9-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc3d9-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc3d9-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc3d9-135">Validation File</span></span>  <br/> |<span data-ttu-id="bc3d9-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc3d9-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc3d9-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc3d9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc3d9-138">False</span><span class="sxs-lookup"><span data-stu-id="bc3d9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc3d9-139">См. также</span><span class="sxs-lookup"><span data-stu-id="bc3d9-139">See also</span></span>



[<span data-ttu-id="bc3d9-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="bc3d9-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="bc3d9-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="bc3d9-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="bc3d9-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="bc3d9-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="bc3d9-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="bc3d9-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="bc3d9-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc3d9-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

