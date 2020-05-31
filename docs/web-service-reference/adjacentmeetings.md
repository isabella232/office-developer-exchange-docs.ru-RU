---
title: аджацентмитингс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: Элемент Аджацентмитингс определяет все элементы календаря, смежные с временем собрания.
ms.openlocfilehash: 9ab818f4f67c32c01101cc595ccb92424a872ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761360"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="18044-103">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="18044-103">AdjacentMeetings</span></span>

<span data-ttu-id="18044-104">Элемент **аджацентмитингс** определяет все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="18044-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="18044-105">**нонемптяррайофаллитемстипе**</span><span class="sxs-lookup"><span data-stu-id="18044-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18044-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="18044-106">Attributes and elements</span></span>

<span data-ttu-id="18044-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="18044-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18044-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="18044-108">Attributes</span></span>

<span data-ttu-id="18044-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="18044-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18044-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="18044-110">Child elements</span></span>

|<span data-ttu-id="18044-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="18044-111">**Element**</span></span>|<span data-ttu-id="18044-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="18044-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18044-113">календаритем</span><span class="sxs-lookup"><span data-stu-id="18044-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="18044-114">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="18044-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18044-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="18044-115">Parent elements</span></span>

|<span data-ttu-id="18044-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="18044-116">**Element**</span></span>|<span data-ttu-id="18044-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="18044-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18044-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="18044-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="18044-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="18044-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="18044-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="18044-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="18044-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="18044-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18044-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="18044-122">Remarks</span></span>

<span data-ttu-id="18044-123">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="18044-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="18044-124">Несмотря на то что в схеме допустимы дополнительные дочерние элементы, элемент [календаритем](calendaritem.md) является единственным дочерним элементом, который веб-службы Exchange (EWS) будут возвращать в элементе **аджацентмитингс** .</span><span class="sxs-lookup"><span data-stu-id="18044-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="18044-125">В этой статье не перечислены дочерние элементы, допустимые для схемы, но не возвращенные службой EWS.</span><span class="sxs-lookup"><span data-stu-id="18044-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="18044-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="18044-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18044-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="18044-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18044-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="18044-128">Schema Name</span></span>  <br/> |<span data-ttu-id="18044-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="18044-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="18044-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="18044-130">Validation File</span></span>  <br/> |<span data-ttu-id="18044-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="18044-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18044-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="18044-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="18044-133">False</span><span class="sxs-lookup"><span data-stu-id="18044-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18044-134">См. также</span><span class="sxs-lookup"><span data-stu-id="18044-134">See also</span></span>

- [<span data-ttu-id="18044-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="18044-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

