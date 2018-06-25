---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: Элемент EnhancedLocation определяет сведения о расположении таких как имя, адрес и необязательные замечания о расположении.
ms.openlocfilehash: 90397cfc622fed40c561d30c13d6617eb979a68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762361"
---
# <a name="enhancedlocation"></a><span data-ttu-id="52808-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="52808-103">EnhancedLocation</span></span>

<span data-ttu-id="52808-104">Элемент **EnhancedLocation** определяет сведения о расположении таких как имя, адрес и необязательные замечания о расположении.</span><span class="sxs-lookup"><span data-stu-id="52808-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="52808-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="52808-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52808-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="52808-106">Attributes and elements</span></span>

<span data-ttu-id="52808-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="52808-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52808-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="52808-108">Attributes</span></span>

<span data-ttu-id="52808-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="52808-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52808-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="52808-110">Child elements</span></span>

|<span data-ttu-id="52808-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52808-111">**Element**</span></span>|<span data-ttu-id="52808-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52808-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52808-113">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="52808-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="52808-114">Задает отображаемое имя папки, контактов, список рассылки, делегата, расположение или правило.</span><span class="sxs-lookup"><span data-stu-id="52808-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="52808-115">Заметки</span><span class="sxs-lookup"><span data-stu-id="52808-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="52808-116">Содержит дополнительные примечания, добавлена пользователем.</span><span class="sxs-lookup"><span data-stu-id="52808-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="52808-117">PostalAddress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="52808-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="52808-118">Указывает почтовый адрес для пользователя.</span><span class="sxs-lookup"><span data-stu-id="52808-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52808-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="52808-119">Parent elements</span></span>

|<span data-ttu-id="52808-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52808-120">**Element**</span></span>|<span data-ttu-id="52808-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52808-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52808-122">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="52808-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="52808-123">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="52808-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="52808-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="52808-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="52808-125">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="52808-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="52808-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="52808-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="52808-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="52808-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="52808-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="52808-128">Remarks</span></span>

<span data-ttu-id="52808-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="52808-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="52808-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="52808-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52808-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="52808-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52808-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="52808-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52808-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="52808-133">Schema Name</span></span>  <br/> |<span data-ttu-id="52808-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="52808-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="52808-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="52808-135">Validation File</span></span>  <br/> |<span data-ttu-id="52808-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52808-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="52808-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="52808-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="52808-138">См. также</span><span class="sxs-lookup"><span data-stu-id="52808-138">See also</span></span>



- [<span data-ttu-id="52808-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="52808-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

