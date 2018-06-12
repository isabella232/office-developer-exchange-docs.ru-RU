---
title: UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: c6ae99c4-18b0-4136-90ab-12cf15e15f91
description: Элемент UpdateDelegate определяет запрос на обновление делегаты в почтовом ящике. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 32322e48acfa5f1058786162565a185a3e565d6e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840318"
---
# <a name="updatedelegate"></a><span data-ttu-id="57b74-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="57b74-104">UpdateDelegate</span></span>

<span data-ttu-id="57b74-105">Элемент **UpdateDelegate** определяет запрос на обновление делегаты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="57b74-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="57b74-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="57b74-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="57b74-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="57b74-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57b74-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57b74-108">Attributes and elements</span></span>

<span data-ttu-id="57b74-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="57b74-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57b74-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57b74-110">Attributes</span></span>

<span data-ttu-id="57b74-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="57b74-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57b74-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57b74-112">Child elements</span></span>

|<span data-ttu-id="57b74-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57b74-113">**Element**</span></span>|<span data-ttu-id="57b74-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57b74-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57b74-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="57b74-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="57b74-116">Содержит массив элементов [DelegateUser](delegateuser.md) , чтобы указать делегатов и обновления для применения к делегатам.</span><span class="sxs-lookup"><span data-stu-id="57b74-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="57b74-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="57b74-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="57b74-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="57b74-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="57b74-119">Определяет порядок обработки приглашений на собрания между делегата и участника.</span><span class="sxs-lookup"><span data-stu-id="57b74-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="57b74-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="57b74-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="57b74-121">Mailbox</span><span class="sxs-lookup"><span data-stu-id="57b74-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="57b74-122">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57b74-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57b74-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57b74-123">Parent elements</span></span>

<span data-ttu-id="57b74-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="57b74-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57b74-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="57b74-125">Remarks</span></span>

<span data-ttu-id="57b74-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="57b74-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57b74-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57b74-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57b74-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57b74-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57b74-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57b74-129">Schema Name</span></span>  <br/> |<span data-ttu-id="57b74-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="57b74-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57b74-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57b74-131">Validation File</span></span>  <br/> |<span data-ttu-id="57b74-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57b74-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57b74-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57b74-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="57b74-134">False</span><span class="sxs-lookup"><span data-stu-id="57b74-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57b74-135">См. также</span><span class="sxs-lookup"><span data-stu-id="57b74-135">See also</span></span>



[<span data-ttu-id="57b74-136">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="57b74-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="57b74-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57b74-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

