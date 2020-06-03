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
description: Элемент Delegate определяет запрос на получение сведений о делегатах для почтового ящика. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: bd7fb55800b51eb2d69184bc4e04cdef3e6b9a89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461032"
---
# <a name="getdelegate"></a><span data-ttu-id="e8c7b-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="e8c7b-104">GetDelegate</span></span>

<span data-ttu-id="e8c7b-105">Элемент **Delegate** определяет запрос на получение сведений о делегатах для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="e8c7b-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e8c7b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="e8c7b-107">**жетделегатетипе**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8c7b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8c7b-108">Attributes and elements</span></span>

<span data-ttu-id="e8c7b-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8c7b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8c7b-110">Attributes</span></span>

|<span data-ttu-id="e8c7b-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-111">**Attribute**</span></span>|<span data-ttu-id="e8c7b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8c7b-113">**инклудепермиссионс**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="e8c7b-114">Указывает, содержит ли ответ параметры разрешений для каждого пользователя делегата.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="e8c7b-115">Значения атрибутов Инклудепермиссионс</span><span class="sxs-lookup"><span data-stu-id="e8c7b-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="e8c7b-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-116">**Value**</span></span>|<span data-ttu-id="e8c7b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8c7b-118">**True**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-118">**True**</span></span> <br/> |<span data-ttu-id="e8c7b-119">Пользовательские разрешения для делегатов возвращаются в дополнение к сведениям о пользователях, которые возвращаются в элементе [UserID](userid.md) .</span><span class="sxs-lookup"><span data-stu-id="e8c7b-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="e8c7b-120">**False**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-120">**False**</span></span> <br/> |<span data-ttu-id="e8c7b-121">Возвращаются сведения [UserID](userid.md) .</span><span class="sxs-lookup"><span data-stu-id="e8c7b-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8c7b-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8c7b-122">Child elements</span></span>

|<span data-ttu-id="e8c7b-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-123">**Element**</span></span>|<span data-ttu-id="e8c7b-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8c7b-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8c7b-125">Mailbox</span><span class="sxs-lookup"><span data-stu-id="e8c7b-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e8c7b-126">Определяет почтовый ящик субъекта.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e8c7b-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="e8c7b-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="e8c7b-128">Содержит массив делегированных пользователей для получения из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="e8c7b-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8c7b-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8c7b-130">Parent elements</span></span>

<span data-ttu-id="e8c7b-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8c7b-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="e8c7b-132">Remarks</span></span>

<span data-ttu-id="e8c7b-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8c7b-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8c7b-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8c7b-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8c7b-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8c7b-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8c7b-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8c7b-136">Schema Name</span></span>  <br/> |<span data-ttu-id="e8c7b-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e8c7b-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8c7b-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8c7b-138">Validation File</span></span>  <br/> |<span data-ttu-id="e8c7b-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e8c7b-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8c7b-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8c7b-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8c7b-141">False</span><span class="sxs-lookup"><span data-stu-id="e8c7b-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8c7b-142">См. также</span><span class="sxs-lookup"><span data-stu-id="e8c7b-142">See also</span></span>



[<span data-ttu-id="e8c7b-143">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="e8c7b-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="e8c7b-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e8c7b-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

