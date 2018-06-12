---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: Элемент GetDelegate определяет запрос на получение сведений о делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762745"
---
# <a name="getdelegate"></a><span data-ttu-id="1328c-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="1328c-104">GetDelegate</span></span>

<span data-ttu-id="1328c-105">Элемент **GetDelegate** определяет запрос на получение сведений о делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="1328c-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="1328c-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1328c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="1328c-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="1328c-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1328c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1328c-108">Attributes and elements</span></span>

<span data-ttu-id="1328c-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1328c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1328c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1328c-110">Attributes</span></span>

|<span data-ttu-id="1328c-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1328c-111">**Attribute**</span></span>|<span data-ttu-id="1328c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1328c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1328c-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="1328c-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="1328c-114">Показывает, содержит ли ответ параметры разрешений для каждого пользователя делегатом.</span><span class="sxs-lookup"><span data-stu-id="1328c-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="1328c-115">Значения атрибутов IncludePermissions</span><span class="sxs-lookup"><span data-stu-id="1328c-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="1328c-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1328c-116">**Value**</span></span>|<span data-ttu-id="1328c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1328c-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1328c-118">**Значение true**</span><span class="sxs-lookup"><span data-stu-id="1328c-118">**True**</span></span> <br/> |<span data-ttu-id="1328c-119">Делегирование пользователя, в дополнение к информации пользователя делегата, который возвращается в элемент [UserId](userid.md) возвращаются разрешения.</span><span class="sxs-lookup"><span data-stu-id="1328c-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="1328c-120">**Значение false**</span><span class="sxs-lookup"><span data-stu-id="1328c-120">**False**</span></span> <br/> |<span data-ttu-id="1328c-121">Возвращается информация [идентификатор пользователя](userid.md) .</span><span class="sxs-lookup"><span data-stu-id="1328c-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1328c-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1328c-122">Child elements</span></span>

|<span data-ttu-id="1328c-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1328c-123">**Element**</span></span>|<span data-ttu-id="1328c-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1328c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1328c-125">Mailbox</span><span class="sxs-lookup"><span data-stu-id="1328c-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="1328c-126">Определяет основного сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="1328c-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1328c-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="1328c-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="1328c-128">Содержит массив делегат пользователям получать из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="1328c-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="1328c-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="1328c-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1328c-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1328c-130">Parent elements</span></span>

<span data-ttu-id="1328c-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="1328c-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1328c-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="1328c-132">Remarks</span></span>

<span data-ttu-id="1328c-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1328c-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1328c-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1328c-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1328c-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1328c-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1328c-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1328c-136">Schema Name</span></span>  <br/> |<span data-ttu-id="1328c-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1328c-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1328c-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1328c-138">Validation File</span></span>  <br/> |<span data-ttu-id="1328c-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1328c-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1328c-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1328c-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="1328c-141">False</span><span class="sxs-lookup"><span data-stu-id="1328c-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1328c-142">См. также</span><span class="sxs-lookup"><span data-stu-id="1328c-142">See also</span></span>



[<span data-ttu-id="1328c-143">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="1328c-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="1328c-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1328c-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

