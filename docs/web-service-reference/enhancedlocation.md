---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: Элемент Енханцедлокатион указывает сведения о расположении, такие как имя, адрес и дополнительные примечания о расположении.
ms.openlocfilehash: 06ec800b763ef61af51da03ca8a340f6ac4d2a8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462959"
---
# <a name="enhancedlocation"></a><span data-ttu-id="bfb6c-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="bfb6c-103">EnhancedLocation</span></span>

<span data-ttu-id="bfb6c-104">Элемент **енханцедлокатион** указывает сведения о расположении, такие как имя, адрес и дополнительные примечания о расположении.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="bfb6c-105">**енханцедлокатионтипе**</span><span class="sxs-lookup"><span data-stu-id="bfb6c-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfb6c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bfb6c-106">Attributes and elements</span></span>

<span data-ttu-id="bfb6c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfb6c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bfb6c-108">Attributes</span></span>

<span data-ttu-id="bfb6c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfb6c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bfb6c-110">Child elements</span></span>

|<span data-ttu-id="bfb6c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bfb6c-111">**Element**</span></span>|<span data-ttu-id="bfb6c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bfb6c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfb6c-113">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="bfb6c-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="bfb6c-114">Определяет отображаемое имя папки, контакта, списка рассылки, делегата, расположения или правила.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="bfb6c-115">Метка</span><span class="sxs-lookup"><span data-stu-id="bfb6c-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="bfb6c-116">Содержит дополнительные примечания, добавленные пользователем.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="bfb6c-117">Посталаддресс (Персонапосталаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="bfb6c-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="bfb6c-118">Указывает почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfb6c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bfb6c-119">Parent elements</span></span>

|<span data-ttu-id="bfb6c-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bfb6c-120">**Element**</span></span>|<span data-ttu-id="bfb6c-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bfb6c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfb6c-122">календаритем</span><span class="sxs-lookup"><span data-stu-id="bfb6c-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="bfb6c-123">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="bfb6c-124">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="bfb6c-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="bfb6c-125">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bfb6c-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="bfb6c-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="bfb6c-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bfb6c-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="bfb6c-128">Remarks</span></span>

<span data-ttu-id="bfb6c-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bfb6c-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfb6c-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfb6c-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bfb6c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfb6c-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bfb6c-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfb6c-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bfb6c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bfb6c-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="bfb6c-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="bfb6c-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bfb6c-135">Validation File</span></span>  <br/> |<span data-ttu-id="bfb6c-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bfb6c-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfb6c-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bfb6c-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bfb6c-138">См. также</span><span class="sxs-lookup"><span data-stu-id="bfb6c-138">See also</span></span>



- [<span data-ttu-id="bfb6c-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bfb6c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

