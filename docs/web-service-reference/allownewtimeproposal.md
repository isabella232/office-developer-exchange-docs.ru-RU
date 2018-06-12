---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: Элемент AllowNewTimeProposal указывает, можно ли участником предлагаться собрание для собрания.
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761369"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="29b6a-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="29b6a-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="29b6a-104">Элемент **AllowNewTimeProposal** указывает, можно ли участником предлагаться собрание для собрания.</span><span class="sxs-lookup"><span data-stu-id="29b6a-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="29b6a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="29b6a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29b6a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29b6a-106">Attributes and elements</span></span>

<span data-ttu-id="29b6a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="29b6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29b6a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29b6a-108">Attributes</span></span>

<span data-ttu-id="29b6a-109">Нет</span><span class="sxs-lookup"><span data-stu-id="29b6a-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29b6a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29b6a-110">Child elements</span></span>

<span data-ttu-id="29b6a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="29b6a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29b6a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29b6a-112">Parent elements</span></span>

|<span data-ttu-id="29b6a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29b6a-113">**Element**</span></span>|<span data-ttu-id="29b6a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29b6a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29b6a-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="29b6a-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="29b6a-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="29b6a-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="29b6a-117">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="29b6a-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="29b6a-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="29b6a-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29b6a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="29b6a-119">Text value</span></span>

<span data-ttu-id="29b6a-120">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="29b6a-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="29b6a-121">Значение **true** указывает, что можно создать новое предложение для время собрания; значение **false** указывает, что новые предложения времени не допускается.</span><span class="sxs-lookup"><span data-stu-id="29b6a-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="29b6a-122">Это значение устанавливается организатора в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="29b6a-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="29b6a-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="29b6a-123">Remarks</span></span>

<span data-ttu-id="29b6a-124">Свойство AllowNewTimeProposal чтения записи для организатора элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="29b6a-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="29b6a-125">Оно доступно только для чтения, для приглашений на собрания и элементы календаря участников.</span><span class="sxs-lookup"><span data-stu-id="29b6a-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="29b6a-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="29b6a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="29b6a-127">Веб-служб Exchange не поддерживает новые сообщения предложения времени.</span><span class="sxs-lookup"><span data-stu-id="29b6a-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="29b6a-128">Получение свойств, относящихся к сообщениям предложение нового времени, используйте расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="29b6a-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="29b6a-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29b6a-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29b6a-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29b6a-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29b6a-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29b6a-131">Schema name</span></span>  <br/> |<span data-ttu-id="29b6a-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="29b6a-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="29b6a-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29b6a-133">Validation file</span></span>  <br/> |<span data-ttu-id="29b6a-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="29b6a-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29b6a-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29b6a-135">Can be empty</span></span>  <br/> |<span data-ttu-id="29b6a-136">False</span><span class="sxs-lookup"><span data-stu-id="29b6a-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29b6a-137">См. также</span><span class="sxs-lookup"><span data-stu-id="29b6a-137">See also</span></span>

- [<span data-ttu-id="29b6a-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="29b6a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

