---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: Элемент DeliverMeetingRequests определяет порядок обработки приглашений на собрания между делегата и участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762063"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="7e2ec-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="7e2ec-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="7e2ec-105">Элемент **DeliverMeetingRequests** определяет порядок обработки приглашений на собрания между делегата и участника.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="7e2ec-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7e2ec-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="7e2ec-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e2ec-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e2ec-108">Attributes and elements</span></span>

<span data-ttu-id="7e2ec-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e2ec-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e2ec-110">Attributes</span></span>

<span data-ttu-id="7e2ec-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e2ec-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e2ec-112">Child elements</span></span>

<span data-ttu-id="7e2ec-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e2ec-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e2ec-114">Parent elements</span></span>

|<span data-ttu-id="7e2ec-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-115">**Element**</span></span>|<span data-ttu-id="7e2ec-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e2ec-117">Метод AddDelegate</span><span class="sxs-lookup"><span data-stu-id="7e2ec-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="7e2ec-118">Определяет запрос на Добавление делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="7e2ec-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="7e2ec-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="7e2ec-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="7e2ec-121">Определяет запрос на обновление делегаты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="7e2ec-122">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="7e2ec-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="7e2ec-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="7e2ec-124">Содержит состояние и результат запроса GetDelegate.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="7e2ec-125">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e2ec-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7e2ec-126">Text value</span></span>

<span data-ttu-id="7e2ec-127">В следующей таблице приведены возможные значения для элемента **DeliverMeetingRequests** .</span><span class="sxs-lookup"><span data-stu-id="7e2ec-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="7e2ec-128">**Значения элементов DeliverMeetingRequests**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="7e2ec-129">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-129">**Value**</span></span>|<span data-ttu-id="7e2ec-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e2ec-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e2ec-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="7e2ec-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="7e2ec-132">Приглашения на собрания пересылку делегата и перемещено в папку «Удаленные» в почтовом ящике участника.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="7e2ec-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="7e2ec-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="7e2ec-134">Приглашения на собрания, пересылаются на делегат и оставаться в папке "Входящие" в почтовом ящике участника.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="7e2ec-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="7e2ec-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="7e2ec-136">Приглашения на собрания, пересылаются на делегат и оставаться в папке "Входящие" в почтовом ящике участника, но кнопки принять, под вопросом и отклонить не отображаются в области чтения Microsoft Office Outlook.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="7e2ec-137">NoForward</span><span class="sxs-lookup"><span data-stu-id="7e2ec-137">NoForward</span></span>  <br/> |<span data-ttu-id="7e2ec-138">Приглашения на собрания не перенаправляются на делегат.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e2ec-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="7e2ec-139">Remarks</span></span>

<span data-ttu-id="7e2ec-140">Параметр **DeliverMeetingRequests** влияет на все делегаты в почтовом ящике участника.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="7e2ec-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e2ec-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e2ec-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e2ec-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e2ec-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e2ec-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e2ec-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e2ec-144">Schema Name</span></span>  <br/> |<span data-ttu-id="7e2ec-145">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7e2ec-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e2ec-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e2ec-146">Validation File</span></span>  <br/> |<span data-ttu-id="7e2ec-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e2ec-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e2ec-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e2ec-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e2ec-149">False</span><span class="sxs-lookup"><span data-stu-id="7e2ec-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e2ec-150">См. также</span><span class="sxs-lookup"><span data-stu-id="7e2ec-150">See also</span></span>

- [<span data-ttu-id="7e2ec-151">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="7e2ec-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="7e2ec-152">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="7e2ec-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="7e2ec-153">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="7e2ec-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="7e2ec-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e2ec-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="7e2ec-155">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="7e2ec-155">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

