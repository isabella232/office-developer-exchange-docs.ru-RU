---
title: Организатор
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
description: Элемент Organizer представляет организатора собрания.
ms.openlocfilehash: c1188c9b3a894e86a08b8869045c3647e394f506
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462418"
---
# <a name="organizer"></a><span data-ttu-id="4f6d3-103">Организатор</span><span class="sxs-lookup"><span data-stu-id="4f6d3-103">Organizer</span></span>

<span data-ttu-id="4f6d3-104">Элемент **Organizer** представляет организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="4f6d3-105">**синглереЦипиенттипе**</span><span class="sxs-lookup"><span data-stu-id="4f6d3-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4f6d3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f6d3-106">Attributes and elements</span></span>

<span data-ttu-id="4f6d3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f6d3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f6d3-108">Attributes</span></span>

<span data-ttu-id="4f6d3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f6d3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f6d3-110">Child elements</span></span>

|<span data-ttu-id="4f6d3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f6d3-111">**Element**</span></span>|<span data-ttu-id="4f6d3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f6d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f6d3-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4f6d3-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="4f6d3-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f6d3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f6d3-115">Parent elements</span></span>

|<span data-ttu-id="4f6d3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f6d3-116">**Element**</span></span>|<span data-ttu-id="4f6d3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f6d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f6d3-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="4f6d3-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4f6d3-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4f6d3-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="4f6d3-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4f6d3-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f6d3-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f6d3-122">Remarks</span></span>

<span data-ttu-id="4f6d3-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4f6d3-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f6d3-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f6d3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f6d3-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f6d3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f6d3-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f6d3-126">Schema name</span></span>  <br/> |<span data-ttu-id="4f6d3-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4f6d3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f6d3-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f6d3-128">Validation file</span></span>  <br/> |<span data-ttu-id="4f6d3-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4f6d3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f6d3-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f6d3-130">Can be empty</span></span>  <br/> |<span data-ttu-id="4f6d3-131">False</span><span class="sxs-lookup"><span data-stu-id="4f6d3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f6d3-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4f6d3-132">See also</span></span>

- [<span data-ttu-id="4f6d3-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f6d3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

