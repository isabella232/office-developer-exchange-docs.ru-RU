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
ms.openlocfilehash: 277ae96fdbc30f1b39ef20553e10ff1de3ff7a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840424"
---
# <a name="userids"></a><span data-ttu-id="fee9e-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="fee9e-104">UserIds</span></span>

<span data-ttu-id="fee9e-105">Элемент **UserID** содержит массив делегированных пользователей, которые необходимо получить или удалить из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="fee9e-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="fee9e-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fee9e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="fee9e-107">**аррайофусеридтипе**</span><span class="sxs-lookup"><span data-stu-id="fee9e-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fee9e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fee9e-108">Attributes and elements</span></span>

<span data-ttu-id="fee9e-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fee9e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fee9e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fee9e-110">Attributes</span></span>

<span data-ttu-id="fee9e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fee9e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fee9e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fee9e-112">Child elements</span></span>

|<span data-ttu-id="fee9e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fee9e-113">**Element**</span></span>|<span data-ttu-id="fee9e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fee9e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fee9e-115">UserId</span><span class="sxs-lookup"><span data-stu-id="fee9e-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="fee9e-116">Определяет делегат для получения или удаления из почтового ящика субъекта.</span><span class="sxs-lookup"><span data-stu-id="fee9e-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="fee9e-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="fee9e-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fee9e-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fee9e-118">Parent elements</span></span>

|<span data-ttu-id="fee9e-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fee9e-119">**Element**</span></span>|<span data-ttu-id="fee9e-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fee9e-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fee9e-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="fee9e-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="fee9e-122">Определяет запрос на получение сведений о делегатах для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fee9e-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="fee9e-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="fee9e-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="fee9e-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="fee9e-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="fee9e-125">Определяет запрос на удаление делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fee9e-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="fee9e-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="fee9e-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fee9e-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="fee9e-127">Remarks</span></span>

<span data-ttu-id="fee9e-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fee9e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fee9e-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fee9e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fee9e-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fee9e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fee9e-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fee9e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fee9e-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fee9e-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fee9e-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fee9e-133">Validation File</span></span>  <br/> |<span data-ttu-id="fee9e-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fee9e-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fee9e-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fee9e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fee9e-136">False</span><span class="sxs-lookup"><span data-stu-id="fee9e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fee9e-137">См. также</span><span class="sxs-lookup"><span data-stu-id="fee9e-137">See also</span></span>



[<span data-ttu-id="fee9e-138">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="fee9e-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="fee9e-139">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="fee9e-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="fee9e-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fee9e-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

