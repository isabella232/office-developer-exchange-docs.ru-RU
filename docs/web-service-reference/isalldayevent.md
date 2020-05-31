---
title: исаллдайевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: Элемент Исаллдайевент указывает, представляет ли элемент календаря или приглашение на собрание событие на целый день.
ms.openlocfilehash: 81cf1e7d8338275540f264de7cbf194005e7770c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833983"
---
# <a name="isalldayevent"></a><span data-ttu-id="20cad-103">исаллдайевент</span><span class="sxs-lookup"><span data-stu-id="20cad-103">IsAllDayEvent</span></span>

<span data-ttu-id="20cad-104">Элемент **исаллдайевент** указывает, представляет ли элемент календаря или приглашение на собрание событие на целый день.</span><span class="sxs-lookup"><span data-stu-id="20cad-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="20cad-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="20cad-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20cad-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20cad-106">Attributes and elements</span></span>

<span data-ttu-id="20cad-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="20cad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20cad-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20cad-108">Attributes</span></span>

<span data-ttu-id="20cad-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="20cad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20cad-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20cad-110">Child elements</span></span>

<span data-ttu-id="20cad-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="20cad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20cad-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20cad-112">Parent elements</span></span>

|<span data-ttu-id="20cad-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20cad-113">**Element**</span></span>|<span data-ttu-id="20cad-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20cad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20cad-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="20cad-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="20cad-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="20cad-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="20cad-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="20cad-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="20cad-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="20cad-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20cad-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="20cad-119">Text value</span></span>

<span data-ttu-id="20cad-120">Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="20cad-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="20cad-121">Значение **true** указывает, что элемент представляет событие на целый день.</span><span class="sxs-lookup"><span data-stu-id="20cad-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="20cad-122">Значение **false** указывает, что элемент занимает меньше рабочих часов пользователя.</span><span class="sxs-lookup"><span data-stu-id="20cad-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="20cad-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="20cad-123">Remarks</span></span>

<span data-ttu-id="20cad-124">Событие на целый день охватывает продолжительность рабочего времени, определенного для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="20cad-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="20cad-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="20cad-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20cad-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="20cad-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20cad-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="20cad-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20cad-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="20cad-128">Schema name</span></span>  <br/> |<span data-ttu-id="20cad-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="20cad-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="20cad-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="20cad-130">Validation file</span></span>  <br/> |<span data-ttu-id="20cad-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="20cad-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20cad-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="20cad-132">Can be empty</span></span>  <br/> |<span data-ttu-id="20cad-133">False</span><span class="sxs-lookup"><span data-stu-id="20cad-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20cad-134">См. также</span><span class="sxs-lookup"><span data-stu-id="20cad-134">See also</span></span>



- [<span data-ttu-id="20cad-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="20cad-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

