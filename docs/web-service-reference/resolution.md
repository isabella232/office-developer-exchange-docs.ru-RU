---
title: Разрешение
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
ms.openlocfilehash: d65f6401e54a4397cad1bfcc85384f644fbae405
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835156"
---
# <a name="resolution"></a><span data-ttu-id="8cf08-103">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8cf08-103">Resolution</span></span>

<span data-ttu-id="8cf08-104">Элемент **Resolution** содержит одну разрешенную сущность.</span><span class="sxs-lookup"><span data-stu-id="8cf08-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="8cf08-105">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="8cf08-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="8cf08-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="8cf08-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="8cf08-107">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="8cf08-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="8cf08-108">Авторешение</span><span class="sxs-lookup"><span data-stu-id="8cf08-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="8cf08-109">Resolution</span><span class="sxs-lookup"><span data-stu-id="8cf08-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="8cf08-110">**ресолутионтипе**</span><span class="sxs-lookup"><span data-stu-id="8cf08-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8cf08-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8cf08-111">Attributes and elements</span></span>

<span data-ttu-id="8cf08-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8cf08-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8cf08-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8cf08-113">Attributes</span></span>

<span data-ttu-id="8cf08-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="8cf08-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8cf08-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8cf08-115">Child elements</span></span>

|<span data-ttu-id="8cf08-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8cf08-116">**Element**</span></span>|<span data-ttu-id="8cf08-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8cf08-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cf08-118">Mailbox</span><span class="sxs-lookup"><span data-stu-id="8cf08-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8cf08-119">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8cf08-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="8cf08-120">Контакт</span><span class="sxs-lookup"><span data-stu-id="8cf08-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="8cf08-121">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="8cf08-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8cf08-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8cf08-122">Parent elements</span></span>

|<span data-ttu-id="8cf08-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8cf08-123">**Element**</span></span>|<span data-ttu-id="8cf08-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8cf08-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cf08-125">Авторешение</span><span class="sxs-lookup"><span data-stu-id="8cf08-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="8cf08-126">Содержит массив разрешений для неоднозначного имени.</span><span class="sxs-lookup"><span data-stu-id="8cf08-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8cf08-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="8cf08-127">Remarks</span></span>

<span data-ttu-id="8cf08-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8cf08-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8cf08-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8cf08-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8cf08-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8cf08-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8cf08-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8cf08-131">Schema name</span></span>  <br/> |<span data-ttu-id="8cf08-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8cf08-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8cf08-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8cf08-133">Validation file</span></span>  <br/> |<span data-ttu-id="8cf08-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8cf08-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8cf08-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8cf08-135">Can be empty</span></span>  <br/> |<span data-ttu-id="8cf08-136">False</span><span class="sxs-lookup"><span data-stu-id="8cf08-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8cf08-137">См. также</span><span class="sxs-lookup"><span data-stu-id="8cf08-137">See also</span></span>



[<span data-ttu-id="8cf08-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8cf08-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="8cf08-139">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="8cf08-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="8cf08-140">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8cf08-140">ResolveNames operation</span></span>](resolvenames-operation.md)

