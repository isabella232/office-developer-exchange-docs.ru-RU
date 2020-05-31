---
title: делегатеусер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: Элемент Делегатеусер определяет одного делегата для добавления или обновления в почтовом ящике или делегата, возвращенного в ответе управления представителями. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762012"
---
# <a name="delegateuser"></a><span data-ttu-id="b397c-104">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="b397c-104">DelegateUser</span></span>

<span data-ttu-id="b397c-105">Элемент **делегатеусер** определяет одного делегата для добавления или обновления в почтовом ящике или делегата, возвращенного в ответе управления представителями.</span><span class="sxs-lookup"><span data-stu-id="b397c-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="b397c-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b397c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="b397c-107">**делегатеусертипе**</span><span class="sxs-lookup"><span data-stu-id="b397c-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b397c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b397c-108">Attributes and elements</span></span>

<span data-ttu-id="b397c-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b397c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b397c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b397c-110">Attributes</span></span>

<span data-ttu-id="b397c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b397c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b397c-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b397c-112">Child elements</span></span>

|<span data-ttu-id="b397c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b397c-113">**Element**</span></span>|<span data-ttu-id="b397c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b397c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b397c-115">UserId</span><span class="sxs-lookup"><span data-stu-id="b397c-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="b397c-116">Определяет делегата.</span><span class="sxs-lookup"><span data-stu-id="b397c-116">Identifies the delegate.</span></span> <span data-ttu-id="b397c-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b397c-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b397c-118">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="b397c-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="b397c-119">Содержит параметры уровня разрешений делегата.</span><span class="sxs-lookup"><span data-stu-id="b397c-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="b397c-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b397c-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b397c-121">рецеивекопиесофмитингмессажес</span><span class="sxs-lookup"><span data-stu-id="b397c-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="b397c-122">Указывает, получает ли делегат копии сообщений, связанных с собранием, которые адресованы участнику.</span><span class="sxs-lookup"><span data-stu-id="b397c-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="b397c-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b397c-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b397c-124">виевприватеитемс</span><span class="sxs-lookup"><span data-stu-id="b397c-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="b397c-125">Указывает, имеет ли представитель разрешение на просмотр частных элементов календаря в почтовом ящике субъекта.</span><span class="sxs-lookup"><span data-stu-id="b397c-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="b397c-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b397c-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b397c-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b397c-127">Parent elements</span></span>

|<span data-ttu-id="b397c-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b397c-128">**Element**</span></span>|<span data-ttu-id="b397c-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b397c-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b397c-130">делегатеусерс</span><span class="sxs-lookup"><span data-stu-id="b397c-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="b397c-131">Содержит идентификаторы делегатов, которые добавляются или обновляются в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b397c-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b397c-132">делегатеусерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="b397c-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="b397c-133">Содержит сообщения ответа для операций управления делегированием.</span><span class="sxs-lookup"><span data-stu-id="b397c-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="b397c-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b397c-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b397c-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="b397c-135">Remarks</span></span>

<span data-ttu-id="b397c-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b397c-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b397c-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b397c-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b397c-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b397c-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b397c-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b397c-139">Schema Name</span></span>  <br/> |<span data-ttu-id="b397c-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b397c-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="b397c-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b397c-141">Validation File</span></span>  <br/> |<span data-ttu-id="b397c-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b397c-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b397c-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b397c-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="b397c-144">False</span><span class="sxs-lookup"><span data-stu-id="b397c-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b397c-145">См. также</span><span class="sxs-lookup"><span data-stu-id="b397c-145">See also</span></span>

- [<span data-ttu-id="b397c-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b397c-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="b397c-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b397c-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="b397c-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b397c-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b397c-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="b397c-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

