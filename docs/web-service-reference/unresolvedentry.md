---
title: унресолведентри
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: Элемент Унресолведентри содержит имя контакта или списка рассылки, которые требуется разрешить.
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459842"
---
# <a name="unresolvedentry"></a><span data-ttu-id="f4529-103">унресолведентри</span><span class="sxs-lookup"><span data-stu-id="f4529-103">UnresolvedEntry</span></span>

<span data-ttu-id="f4529-104">Элемент **унресолведентри** содержит имя контакта или списка рассылки, которые требуется разрешить.</span><span class="sxs-lookup"><span data-stu-id="f4529-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="f4529-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f4529-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="f4529-106">унресолведентри</span><span class="sxs-lookup"><span data-stu-id="f4529-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="f4529-107">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="f4529-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4529-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4529-108">Attributes and elements</span></span>

<span data-ttu-id="f4529-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f4529-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4529-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4529-110">Attributes</span></span>

<span data-ttu-id="f4529-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4529-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4529-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4529-112">Child elements</span></span>

<span data-ttu-id="f4529-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4529-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4529-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4529-114">Parent elements</span></span>

|<span data-ttu-id="f4529-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4529-115">**Element**</span></span>|<span data-ttu-id="f4529-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4529-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4529-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f4529-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="f4529-118">Определяет запрос на разрешение неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="f4529-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4529-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f4529-119">Text value</span></span>

<span data-ttu-id="f4529-120">Текстовое значение представляет имя общедоступного контакта или списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="f4529-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="f4529-121">Минимальная длина строки — один символ.</span><span class="sxs-lookup"><span data-stu-id="f4529-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4529-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4529-122">Remarks</span></span>

<span data-ttu-id="f4529-123">Текстовое значение этого элемента используется для сопоставления имен со следующими полями:</span><span class="sxs-lookup"><span data-stu-id="f4529-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="f4529-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f4529-124">First name</span></span>
    
- <span data-ttu-id="f4529-125">Фамилия</span><span class="sxs-lookup"><span data-stu-id="f4529-125">Last name</span></span>
    
- <span data-ttu-id="f4529-126">Различающееся имя (DN)</span><span class="sxs-lookup"><span data-stu-id="f4529-126">Display name</span></span>
    
- <span data-ttu-id="f4529-127">Полное имя</span><span class="sxs-lookup"><span data-stu-id="f4529-127">Full name</span></span>
    
- <span data-ttu-id="f4529-128">Office</span><span class="sxs-lookup"><span data-stu-id="f4529-128">Office</span></span>
    
- <span data-ttu-id="f4529-129">Alias</span><span class="sxs-lookup"><span data-stu-id="f4529-129">Alias</span></span>
    
- <span data-ttu-id="f4529-130">SMTP-адрес</span><span class="sxs-lookup"><span data-stu-id="f4529-130">SMTP address</span></span>
    
<span data-ttu-id="f4529-131">Адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, сохраняются в массиве с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="f4529-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="f4529-132">[Операция ResolveNames](resolvenames-operation.md) выполняет частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP:user1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="f4529-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="f4529-133">Если не указать тип маршрутизации, операция **ResolveNames** по умолчанию будет иметь тип маршрутизации SMTP, сопоставлять его с основным СВОЙСТВОМ SMTP-адреса, а не выполнять поиск по многозначному массиву.</span><span class="sxs-lookup"><span data-stu-id="f4529-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="f4529-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4529-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4529-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4529-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4529-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4529-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4529-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4529-137">Schema Name</span></span>  <br/> |<span data-ttu-id="f4529-138">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f4529-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4529-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4529-139">Validation File</span></span>  <br/> |<span data-ttu-id="f4529-140">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f4529-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4529-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4529-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4529-142">False</span><span class="sxs-lookup"><span data-stu-id="f4529-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4529-143">См. также</span><span class="sxs-lookup"><span data-stu-id="f4529-143">See also</span></span>



[<span data-ttu-id="f4529-144">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f4529-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="f4529-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4529-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

