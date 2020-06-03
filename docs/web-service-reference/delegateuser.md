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
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458805"
---
# <a name="delegateuser"></a><span data-ttu-id="79511-104">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="79511-104">DelegateUser</span></span>

<span data-ttu-id="79511-105">Элемент **делегатеусер** определяет одного делегата для добавления или обновления в почтовом ящике или делегата, возвращенного в ответе управления представителями.</span><span class="sxs-lookup"><span data-stu-id="79511-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="79511-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="79511-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="79511-107">**делегатеусертипе**</span><span class="sxs-lookup"><span data-stu-id="79511-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="79511-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="79511-108">Attributes and elements</span></span>

<span data-ttu-id="79511-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="79511-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79511-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="79511-110">Attributes</span></span>

<span data-ttu-id="79511-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="79511-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79511-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="79511-112">Child elements</span></span>

|<span data-ttu-id="79511-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="79511-113">**Element**</span></span>|<span data-ttu-id="79511-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79511-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79511-115">UserId</span><span class="sxs-lookup"><span data-stu-id="79511-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="79511-116">Определяет делегата.</span><span class="sxs-lookup"><span data-stu-id="79511-116">Identifies the delegate.</span></span> <span data-ttu-id="79511-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="79511-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="79511-118">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="79511-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="79511-119">Содержит параметры уровня разрешений делегата.</span><span class="sxs-lookup"><span data-stu-id="79511-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="79511-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="79511-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="79511-121">рецеивекопиесофмитингмессажес</span><span class="sxs-lookup"><span data-stu-id="79511-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="79511-122">Указывает, получает ли делегат копии сообщений, связанных с собранием, которые адресованы участнику.</span><span class="sxs-lookup"><span data-stu-id="79511-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="79511-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="79511-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="79511-124">виевприватеитемс</span><span class="sxs-lookup"><span data-stu-id="79511-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="79511-125">Указывает, имеет ли представитель разрешение на просмотр частных элементов календаря в почтовом ящике субъекта.</span><span class="sxs-lookup"><span data-stu-id="79511-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="79511-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="79511-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79511-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="79511-127">Parent elements</span></span>

|<span data-ttu-id="79511-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="79511-128">**Element**</span></span>|<span data-ttu-id="79511-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79511-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79511-130">делегатеусерс</span><span class="sxs-lookup"><span data-stu-id="79511-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="79511-131">Содержит идентификаторы делегатов, которые добавляются или обновляются в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="79511-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="79511-132">делегатеусерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="79511-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="79511-133">Содержит сообщения ответа для операций управления делегированием.</span><span class="sxs-lookup"><span data-stu-id="79511-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="79511-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="79511-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="79511-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="79511-135">Remarks</span></span>

<span data-ttu-id="79511-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="79511-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79511-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="79511-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79511-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="79511-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79511-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="79511-139">Schema Name</span></span>  <br/> |<span data-ttu-id="79511-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="79511-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="79511-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="79511-141">Validation File</span></span>  <br/> |<span data-ttu-id="79511-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="79511-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79511-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="79511-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="79511-144">False</span><span class="sxs-lookup"><span data-stu-id="79511-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79511-145">См. также</span><span class="sxs-lookup"><span data-stu-id="79511-145">See also</span></span>

- [<span data-ttu-id="79511-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="79511-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="79511-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="79511-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="79511-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="79511-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="79511-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="79511-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

