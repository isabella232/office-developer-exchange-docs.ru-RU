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
description: Элемент решение содержит одного объекта разрешения.
ms.openlocfilehash: d65f6401e54a4397cad1bfcc85384f644fbae405
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835156"
---
# <a name="resolution"></a><span data-ttu-id="e7174-103">Решение</span><span class="sxs-lookup"><span data-stu-id="e7174-103">Resolution</span></span>

<span data-ttu-id="e7174-104">Элемент **решение** содержит одного объекта разрешения.</span><span class="sxs-lookup"><span data-stu-id="e7174-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="e7174-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e7174-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="e7174-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e7174-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="e7174-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e7174-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="e7174-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="e7174-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="e7174-109">Решение</span><span class="sxs-lookup"><span data-stu-id="e7174-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="e7174-110">**ResolutionType**</span><span class="sxs-lookup"><span data-stu-id="e7174-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7174-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7174-111">Attributes and elements</span></span>

<span data-ttu-id="e7174-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e7174-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7174-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7174-113">Attributes</span></span>

<span data-ttu-id="e7174-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="e7174-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7174-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7174-115">Child elements</span></span>

|<span data-ttu-id="e7174-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7174-116">**Element**</span></span>|<span data-ttu-id="e7174-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7174-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7174-118">Mailbox</span><span class="sxs-lookup"><span data-stu-id="e7174-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e7174-119">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7174-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="e7174-120">Контакт</span><span class="sxs-lookup"><span data-stu-id="e7174-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e7174-121">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7174-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7174-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7174-122">Parent elements</span></span>

|<span data-ttu-id="e7174-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7174-123">**Element**</span></span>|<span data-ttu-id="e7174-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7174-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7174-125">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="e7174-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="e7174-126">Содержит набор разрешений для разрешения неоднозначных псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="e7174-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7174-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="e7174-127">Remarks</span></span>

<span data-ttu-id="e7174-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e7174-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7174-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7174-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7174-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7174-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7174-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7174-131">Schema name</span></span>  <br/> |<span data-ttu-id="e7174-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e7174-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7174-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7174-133">Validation file</span></span>  <br/> |<span data-ttu-id="e7174-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7174-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7174-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7174-135">Can be empty</span></span>  <br/> |<span data-ttu-id="e7174-136">False</span><span class="sxs-lookup"><span data-stu-id="e7174-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7174-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e7174-137">See also</span></span>



[<span data-ttu-id="e7174-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e7174-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="e7174-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e7174-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="e7174-140">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e7174-140">ResolveNames operation</span></span>](resolvenames-operation.md)

