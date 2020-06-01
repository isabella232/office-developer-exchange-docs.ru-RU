---
title: тимезонедефинитионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinitions
api_type:
- schema
ms.assetid: 9ca1584e-65b8-49ba-a408-e3e8597e6607
description: Элемент Тимезонедефинитионс представляет массив определений часовых поясов.
ms.openlocfilehash: 16a25eb4fdcad2554ebd19626d0a0bc7f6391ac5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468763"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="6514f-103">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="6514f-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="6514f-104">Элемент **тимезонедефинитионс** представляет массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="6514f-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="6514f-105">**аррайофтимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="6514f-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6514f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6514f-106">Attributes and elements</span></span>

<span data-ttu-id="6514f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6514f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6514f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6514f-108">Attributes</span></span>

<span data-ttu-id="6514f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6514f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6514f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6514f-110">Child elements</span></span>

|<span data-ttu-id="6514f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6514f-111">**Element**</span></span>|<span data-ttu-id="6514f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6514f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6514f-113">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="6514f-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="6514f-114">Задает периоды и переходы, определяющие часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="6514f-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6514f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6514f-115">Parent elements</span></span>

|<span data-ttu-id="6514f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6514f-116">**Element**</span></span>|<span data-ttu-id="6514f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6514f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6514f-118">жетсервертимезонесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6514f-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="6514f-119">Содержит состояние и результат запроса [операции GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6514f-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6514f-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="6514f-120">Remarks</span></span>

<span data-ttu-id="6514f-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6514f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6514f-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6514f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6514f-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6514f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6514f-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6514f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6514f-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6514f-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6514f-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6514f-126">Validation File</span></span>  <br/> |<span data-ttu-id="6514f-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6514f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6514f-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6514f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6514f-129">False</span><span class="sxs-lookup"><span data-stu-id="6514f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6514f-130">См. также</span><span class="sxs-lookup"><span data-stu-id="6514f-130">See also</span></span>



- [<span data-ttu-id="6514f-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6514f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

