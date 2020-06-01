---
title: митингрекуествассент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestWasSent
api_type:
- schema
ms.assetid: 9192400a-8eef-4147-9f94-aa8ea91b41d8
description: Элемент Митингрекуествассент указывает, было ли приглашение на собрание отправлено запрошенным участникам.
ms.openlocfilehash: d5005eb86d5f8d2f438a69e634f0617c2311d720
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465767"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="f204e-103">митингрекуествассент</span><span class="sxs-lookup"><span data-stu-id="f204e-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="f204e-104">Элемент **митингрекуествассент** указывает, было ли приглашение на собрание отправлено запрошенным участникам.</span><span class="sxs-lookup"><span data-stu-id="f204e-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="f204e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f204e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f204e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f204e-106">Attributes and elements</span></span>

<span data-ttu-id="f204e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f204e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f204e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f204e-108">Attributes</span></span>

<span data-ttu-id="f204e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f204e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f204e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f204e-110">Child elements</span></span>

<span data-ttu-id="f204e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f204e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f204e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f204e-112">Parent elements</span></span>

|<span data-ttu-id="f204e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f204e-113">**Element**</span></span>|<span data-ttu-id="f204e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f204e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f204e-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="f204e-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f204e-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="f204e-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f204e-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="f204e-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f204e-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f204e-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f204e-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f204e-119">Text value</span></span>

<span data-ttu-id="f204e-120">Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="f204e-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="f204e-121">Значение **true** указывает на то, что приглашение на собрание было отправлено.</span><span class="sxs-lookup"><span data-stu-id="f204e-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="f204e-122">Значение **false** указывает на то, что приглашение на собрание не было отправлено.</span><span class="sxs-lookup"><span data-stu-id="f204e-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f204e-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="f204e-123">Remarks</span></span>

<span data-ttu-id="f204e-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f204e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f204e-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f204e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f204e-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f204e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f204e-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f204e-127">Schema name</span></span>  <br/> |<span data-ttu-id="f204e-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f204e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f204e-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f204e-129">Validation file</span></span>  <br/> |<span data-ttu-id="f204e-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f204e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f204e-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f204e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="f204e-132">False</span><span class="sxs-lookup"><span data-stu-id="f204e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f204e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f204e-133">See also</span></span>



- [<span data-ttu-id="f204e-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f204e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

