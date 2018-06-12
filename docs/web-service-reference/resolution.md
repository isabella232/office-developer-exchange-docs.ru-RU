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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835156"
---
# <a name="resolution"></a><span data-ttu-id="11c0c-103">Решение</span><span class="sxs-lookup"><span data-stu-id="11c0c-103">Resolution</span></span>

<span data-ttu-id="11c0c-104">Элемент **решение** содержит одного объекта разрешения.</span><span class="sxs-lookup"><span data-stu-id="11c0c-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="11c0c-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="11c0c-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="11c0c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="11c0c-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="11c0c-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="11c0c-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="11c0c-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="11c0c-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="11c0c-109">Решение</span><span class="sxs-lookup"><span data-stu-id="11c0c-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="11c0c-110">**ResolutionType**</span><span class="sxs-lookup"><span data-stu-id="11c0c-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11c0c-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11c0c-111">Attributes and elements</span></span>

<span data-ttu-id="11c0c-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="11c0c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11c0c-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11c0c-113">Attributes</span></span>

<span data-ttu-id="11c0c-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="11c0c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11c0c-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11c0c-115">Child elements</span></span>

|<span data-ttu-id="11c0c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11c0c-116">**Element**</span></span>|<span data-ttu-id="11c0c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11c0c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11c0c-118">Mailbox</span><span class="sxs-lookup"><span data-stu-id="11c0c-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="11c0c-119">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="11c0c-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="11c0c-120">Контакт</span><span class="sxs-lookup"><span data-stu-id="11c0c-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="11c0c-121">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="11c0c-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11c0c-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11c0c-122">Parent elements</span></span>

|<span data-ttu-id="11c0c-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11c0c-123">**Element**</span></span>|<span data-ttu-id="11c0c-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11c0c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11c0c-125">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="11c0c-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="11c0c-126">Содержит набор разрешений для разрешения неоднозначных псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="11c0c-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11c0c-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="11c0c-127">Remarks</span></span>

<span data-ttu-id="11c0c-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="11c0c-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11c0c-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11c0c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11c0c-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11c0c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11c0c-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11c0c-131">Schema name</span></span>  <br/> |<span data-ttu-id="11c0c-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="11c0c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="11c0c-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11c0c-133">Validation file</span></span>  <br/> |<span data-ttu-id="11c0c-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="11c0c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11c0c-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11c0c-135">Can be empty</span></span>  <br/> |<span data-ttu-id="11c0c-136">False</span><span class="sxs-lookup"><span data-stu-id="11c0c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11c0c-137">См. также</span><span class="sxs-lookup"><span data-stu-id="11c0c-137">See also</span></span>



[<span data-ttu-id="11c0c-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="11c0c-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="11c0c-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="11c0c-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="11c0c-140">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="11c0c-140">ResolveNames operation</span></span>](resolvenames-operation.md)

