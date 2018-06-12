---
title: UnresolvedEntry
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
description: Элемент UnresolvedEntry содержит имя контакта или список рассылки для разрешения.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840300"
---
# <a name="unresolvedentry"></a><span data-ttu-id="07148-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="07148-103">UnresolvedEntry</span></span>

<span data-ttu-id="07148-104">Элемент **UnresolvedEntry** содержит имя контакта или список рассылки для разрешения.</span><span class="sxs-lookup"><span data-stu-id="07148-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="07148-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="07148-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="07148-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="07148-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="07148-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="07148-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07148-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07148-108">Attributes and elements</span></span>

<span data-ttu-id="07148-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="07148-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07148-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07148-110">Attributes</span></span>

<span data-ttu-id="07148-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="07148-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07148-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07148-112">Child elements</span></span>

<span data-ttu-id="07148-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="07148-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07148-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07148-114">Parent elements</span></span>

|<span data-ttu-id="07148-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07148-115">**Element**</span></span>|<span data-ttu-id="07148-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07148-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07148-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="07148-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="07148-118">Определяет запрос для разрешения неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="07148-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07148-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="07148-119">Text value</span></span>

<span data-ttu-id="07148-120">Текстовое значение представляет имя общей списка рассылки или контактов.</span><span class="sxs-lookup"><span data-stu-id="07148-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="07148-121">Минимальная длина строки — один символ.</span><span class="sxs-lookup"><span data-stu-id="07148-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="07148-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="07148-122">Remarks</span></span>

<span data-ttu-id="07148-123">Текстовое значение этого элемента используется для разрешения имен для следующих полей:</span><span class="sxs-lookup"><span data-stu-id="07148-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="07148-124">Имя</span><span class="sxs-lookup"><span data-stu-id="07148-124">First name</span></span>
    
- <span data-ttu-id="07148-125">Фамилия</span><span class="sxs-lookup"><span data-stu-id="07148-125">Last name</span></span>
    
- <span data-ttu-id="07148-126">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="07148-126">Display name</span></span>
    
- <span data-ttu-id="07148-127">Полное имя</span><span class="sxs-lookup"><span data-stu-id="07148-127">Full name</span></span>
    
- <span data-ttu-id="07148-128">Office</span><span class="sxs-lookup"><span data-stu-id="07148-128">Office</span></span>
    
- <span data-ttu-id="07148-129">Alias</span><span class="sxs-lookup"><span data-stu-id="07148-129">Alias</span></span>
    
- <span data-ttu-id="07148-130">SMTP-адрес</span><span class="sxs-lookup"><span data-stu-id="07148-130">SMTP address</span></span>
    
<span data-ttu-id="07148-131">Адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip, сохраняются в нескольких значений массива.</span><span class="sxs-lookup"><span data-stu-id="07148-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="07148-132">[Операция ResolveNames](resolvenames-operation.md) выполняет частичное соответствие каждого значения этого массива, при добавлении типа маршрутизации в начале неизвестное имя, например «sip:User1@Contoso.com».</span><span class="sxs-lookup"><span data-stu-id="07148-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="07148-133">Если не указать тип маршрутизации, операция **ResolveNames** по умолчанию для типа маршрутизации smtp, соответствует свойству основной адрес SMTP и поиск нескольких значений массива.</span><span class="sxs-lookup"><span data-stu-id="07148-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="07148-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="07148-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07148-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07148-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07148-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07148-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07148-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07148-137">Schema Name</span></span>  <br/> |<span data-ttu-id="07148-138">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="07148-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07148-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07148-139">Validation File</span></span>  <br/> |<span data-ttu-id="07148-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="07148-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07148-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07148-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="07148-142">False</span><span class="sxs-lookup"><span data-stu-id="07148-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07148-143">См. также</span><span class="sxs-lookup"><span data-stu-id="07148-143">See also</span></span>



[<span data-ttu-id="07148-144">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="07148-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="07148-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="07148-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

