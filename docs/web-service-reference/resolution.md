---
title: Решение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resolution
api_type:
- schema
ms.assetid: 573bed4b-d7b1-4baf-b16f-0795cdebf1a7
description: Элемент Resolution содержит одну разрешенную сущность.
ms.openlocfilehash: 63c80f3c8d7dabf7e6dc1494df04c0be821b28bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468287"
---
# <a name="resolution"></a><span data-ttu-id="12bd4-103">Решение</span><span class="sxs-lookup"><span data-stu-id="12bd4-103">Resolution</span></span>

<span data-ttu-id="12bd4-104">Элемент **Resolution** содержит одну разрешенную сущность.</span><span class="sxs-lookup"><span data-stu-id="12bd4-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="12bd4-105">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="12bd4-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="12bd4-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="12bd4-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="12bd4-107">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="12bd4-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="12bd4-108">Авторешение</span><span class="sxs-lookup"><span data-stu-id="12bd4-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="12bd4-109">Resolution</span><span class="sxs-lookup"><span data-stu-id="12bd4-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="12bd4-110">**ресолутионтипе**</span><span class="sxs-lookup"><span data-stu-id="12bd4-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12bd4-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="12bd4-111">Attributes and elements</span></span>

<span data-ttu-id="12bd4-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="12bd4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12bd4-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="12bd4-113">Attributes</span></span>

<span data-ttu-id="12bd4-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="12bd4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12bd4-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="12bd4-115">Child elements</span></span>

|<span data-ttu-id="12bd4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12bd4-116">**Element**</span></span>|<span data-ttu-id="12bd4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12bd4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bd4-118">Mailbox</span><span class="sxs-lookup"><span data-stu-id="12bd4-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="12bd4-119">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12bd4-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="12bd4-120">Контакт</span><span class="sxs-lookup"><span data-stu-id="12bd4-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="12bd4-121">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="12bd4-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12bd4-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="12bd4-122">Parent elements</span></span>

|<span data-ttu-id="12bd4-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12bd4-123">**Element**</span></span>|<span data-ttu-id="12bd4-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12bd4-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bd4-125">Авторешение</span><span class="sxs-lookup"><span data-stu-id="12bd4-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="12bd4-126">Содержит массив разрешений для неоднозначного имени.</span><span class="sxs-lookup"><span data-stu-id="12bd4-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12bd4-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="12bd4-127">Remarks</span></span>

<span data-ttu-id="12bd4-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="12bd4-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12bd4-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="12bd4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12bd4-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="12bd4-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12bd4-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="12bd4-131">Schema name</span></span>  <br/> |<span data-ttu-id="12bd4-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="12bd4-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="12bd4-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="12bd4-133">Validation file</span></span>  <br/> |<span data-ttu-id="12bd4-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="12bd4-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12bd4-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="12bd4-135">Can be empty</span></span>  <br/> |<span data-ttu-id="12bd4-136">False</span><span class="sxs-lookup"><span data-stu-id="12bd4-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12bd4-137">См. также</span><span class="sxs-lookup"><span data-stu-id="12bd4-137">See also</span></span>



[<span data-ttu-id="12bd4-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="12bd4-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="12bd4-139">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="12bd4-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="12bd4-140">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="12bd4-140">ResolveNames operation</span></span>](resolvenames-operation.md)

