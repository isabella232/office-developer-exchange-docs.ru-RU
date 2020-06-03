---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: Элемент UserId содержит массив делегированных пользователей, которые необходимо получить или удалить из почтового ящика участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: de4661226c154ef0d2d5ac55c57405e20c4d2aee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459779"
---
# <a name="userids"></a><span data-ttu-id="21ee1-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="21ee1-104">UserIds</span></span>

<span data-ttu-id="21ee1-105">Элемент **UserID** содержит массив делегированных пользователей, которые необходимо получить или удалить из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="21ee1-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="21ee1-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="21ee1-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="21ee1-107">**аррайофусеридтипе**</span><span class="sxs-lookup"><span data-stu-id="21ee1-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21ee1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="21ee1-108">Attributes and elements</span></span>

<span data-ttu-id="21ee1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="21ee1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21ee1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="21ee1-110">Attributes</span></span>

<span data-ttu-id="21ee1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="21ee1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21ee1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="21ee1-112">Child elements</span></span>

|<span data-ttu-id="21ee1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="21ee1-113">**Element**</span></span>|<span data-ttu-id="21ee1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="21ee1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21ee1-115">UserId</span><span class="sxs-lookup"><span data-stu-id="21ee1-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="21ee1-116">Определяет делегат для получения или удаления из почтового ящика субъекта.</span><span class="sxs-lookup"><span data-stu-id="21ee1-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="21ee1-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="21ee1-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21ee1-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="21ee1-118">Parent elements</span></span>

|<span data-ttu-id="21ee1-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="21ee1-119">**Element**</span></span>|<span data-ttu-id="21ee1-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="21ee1-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21ee1-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="21ee1-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="21ee1-122">Определяет запрос на получение сведений о делегатах для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="21ee1-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="21ee1-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="21ee1-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="21ee1-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="21ee1-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="21ee1-125">Определяет запрос на удаление делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="21ee1-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="21ee1-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="21ee1-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21ee1-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="21ee1-127">Remarks</span></span>

<span data-ttu-id="21ee1-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="21ee1-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21ee1-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="21ee1-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21ee1-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="21ee1-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21ee1-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="21ee1-131">Schema Name</span></span>  <br/> |<span data-ttu-id="21ee1-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="21ee1-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21ee1-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="21ee1-133">Validation File</span></span>  <br/> |<span data-ttu-id="21ee1-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="21ee1-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21ee1-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="21ee1-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="21ee1-136">False</span><span class="sxs-lookup"><span data-stu-id="21ee1-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21ee1-137">См. также</span><span class="sxs-lookup"><span data-stu-id="21ee1-137">See also</span></span>



[<span data-ttu-id="21ee1-138">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="21ee1-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="21ee1-139">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="21ee1-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="21ee1-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="21ee1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

