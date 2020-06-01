---
title: С отменой
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: Элемент, который должен быть отменен, указывает, отменена ли встреча или собрание.
ms.openlocfilehash: 946c9d956da9cf31e9fa08d4ab6f4950b11214b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455571"
---
# <a name="iscancelled"></a><span data-ttu-id="9804d-103">С отменой</span><span class="sxs-lookup"><span data-stu-id="9804d-103">IsCancelled</span></span>

<span data-ttu-id="9804d-104">Элемент, который должен **быть отменен,** указывает, отменена ли встреча или собрание.</span><span class="sxs-lookup"><span data-stu-id="9804d-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="9804d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9804d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9804d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9804d-106">Attributes and elements</span></span>

<span data-ttu-id="9804d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9804d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9804d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9804d-108">Attributes</span></span>

<span data-ttu-id="9804d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9804d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9804d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9804d-110">Child elements</span></span>

<span data-ttu-id="9804d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9804d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9804d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9804d-112">Parent elements</span></span>

|<span data-ttu-id="9804d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9804d-113">**Element**</span></span>|<span data-ttu-id="9804d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9804d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9804d-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="9804d-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9804d-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="9804d-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9804d-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9804d-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9804d-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9804d-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9804d-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9804d-119">Text value</span></span>

<span data-ttu-id="9804d-120">Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="9804d-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="9804d-121">Значение **true** указывает, что элемент календаря был отменен.</span><span class="sxs-lookup"><span data-stu-id="9804d-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="9804d-122">Значение **false** указывает, что элемент календаря не был отменен.</span><span class="sxs-lookup"><span data-stu-id="9804d-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9804d-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="9804d-123">Remarks</span></span>

<span data-ttu-id="9804d-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9804d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9804d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9804d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9804d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9804d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9804d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9804d-127">Schema name</span></span>  <br/> |<span data-ttu-id="9804d-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9804d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9804d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9804d-129">Validation file</span></span>  <br/> |<span data-ttu-id="9804d-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9804d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9804d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9804d-131">Can be empty</span></span>  <br/> |<span data-ttu-id="9804d-132">False</span><span class="sxs-lookup"><span data-stu-id="9804d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9804d-133">См. также</span><span class="sxs-lookup"><span data-stu-id="9804d-133">See also</span></span>



- [<span data-ttu-id="9804d-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9804d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

