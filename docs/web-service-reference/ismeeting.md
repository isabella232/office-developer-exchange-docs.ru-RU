---
title: "\"Собрание\""
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: Элемент "собрание" указывает, является ли элемент календаря собранием или встречей.
ms.openlocfilehash: fd72766977567210cd08b47d0723cd73aa53a622
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465970"
---
# <a name="ismeeting"></a><span data-ttu-id="646b9-103">"Собрание"</span><span class="sxs-lookup"><span data-stu-id="646b9-103">IsMeeting</span></span>

<span data-ttu-id="646b9-104">Элемент " **собрание** " указывает, является ли элемент календаря собранием или встречей.</span><span class="sxs-lookup"><span data-stu-id="646b9-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="646b9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="646b9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="646b9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="646b9-106">Attributes and elements</span></span>

<span data-ttu-id="646b9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="646b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="646b9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="646b9-108">Attributes</span></span>

<span data-ttu-id="646b9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="646b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="646b9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="646b9-110">Child elements</span></span>

<span data-ttu-id="646b9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="646b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="646b9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="646b9-112">Parent elements</span></span>

|<span data-ttu-id="646b9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="646b9-113">**Element**</span></span>|<span data-ttu-id="646b9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="646b9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="646b9-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="646b9-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="646b9-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="646b9-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="646b9-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="646b9-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="646b9-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="646b9-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="646b9-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="646b9-119">Text value</span></span>

<span data-ttu-id="646b9-120">Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="646b9-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="646b9-121">Значение **true** указывает, что элемент календаря является собранием.</span><span class="sxs-lookup"><span data-stu-id="646b9-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="646b9-122">Значение **false** указывает, что элемент календаря является встречей.</span><span class="sxs-lookup"><span data-stu-id="646b9-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="646b9-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="646b9-123">Remarks</span></span>

<span data-ttu-id="646b9-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="646b9-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="646b9-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="646b9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="646b9-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="646b9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="646b9-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="646b9-127">Schema name</span></span>  <br/> |<span data-ttu-id="646b9-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="646b9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="646b9-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="646b9-129">Validation file</span></span>  <br/> |<span data-ttu-id="646b9-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="646b9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="646b9-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="646b9-131">Can be empty</span></span>  <br/> |<span data-ttu-id="646b9-132">False</span><span class="sxs-lookup"><span data-stu-id="646b9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="646b9-133">См. также</span><span class="sxs-lookup"><span data-stu-id="646b9-133">See also</span></span>



- [<span data-ttu-id="646b9-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="646b9-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

