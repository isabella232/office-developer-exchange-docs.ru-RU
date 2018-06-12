---
title: Organizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Organizer
api_type:
- schema
ms.assetid: 63892b57-3805-4d60-b9f7-20552a69c241
description: Элемент организатора представляет организатора собрания.
ms.openlocfilehash: b723578a1b52cd5f6e9bd869a15430453adfa291
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834662"
---
# <a name="organizer"></a><span data-ttu-id="05f1d-103">Organizer</span><span class="sxs-lookup"><span data-stu-id="05f1d-103">Organizer</span></span>

<span data-ttu-id="05f1d-104">Элемент **организатора** представляет организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="05f1d-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="05f1d-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="05f1d-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="05f1d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="05f1d-106">Attributes and elements</span></span>

<span data-ttu-id="05f1d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="05f1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05f1d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="05f1d-108">Attributes</span></span>

<span data-ttu-id="05f1d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="05f1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05f1d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="05f1d-110">Child elements</span></span>

|<span data-ttu-id="05f1d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="05f1d-111">**Element**</span></span>|<span data-ttu-id="05f1d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="05f1d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05f1d-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="05f1d-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="05f1d-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="05f1d-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05f1d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="05f1d-115">Parent elements</span></span>

|<span data-ttu-id="05f1d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="05f1d-116">**Element**</span></span>|<span data-ttu-id="05f1d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="05f1d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05f1d-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="05f1d-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="05f1d-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="05f1d-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05f1d-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="05f1d-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="05f1d-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="05f1d-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05f1d-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="05f1d-122">Remarks</span></span>

<span data-ttu-id="05f1d-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="05f1d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05f1d-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="05f1d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05f1d-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="05f1d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05f1d-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="05f1d-126">Schema name</span></span>  <br/> |<span data-ttu-id="05f1d-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="05f1d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="05f1d-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="05f1d-128">Validation file</span></span>  <br/> |<span data-ttu-id="05f1d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05f1d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05f1d-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="05f1d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="05f1d-131">False</span><span class="sxs-lookup"><span data-stu-id="05f1d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05f1d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="05f1d-132">See also</span></span>

- [<span data-ttu-id="05f1d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="05f1d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

