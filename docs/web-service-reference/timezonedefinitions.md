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
ms.openlocfilehash: 0bc1b69ef564bb4e239d9845a4b1a0133292ff12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840190"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="dadce-103">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="dadce-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="dadce-104">Элемент **тимезонедефинитионс** представляет массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="dadce-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="dadce-105">**аррайофтимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="dadce-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dadce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dadce-106">Attributes and elements</span></span>

<span data-ttu-id="dadce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dadce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dadce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dadce-108">Attributes</span></span>

<span data-ttu-id="dadce-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dadce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dadce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dadce-110">Child elements</span></span>

|<span data-ttu-id="dadce-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dadce-111">**Element**</span></span>|<span data-ttu-id="dadce-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dadce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dadce-113">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="dadce-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="dadce-114">Задает периоды и переходы, определяющие часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="dadce-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dadce-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dadce-115">Parent elements</span></span>

|<span data-ttu-id="dadce-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dadce-116">**Element**</span></span>|<span data-ttu-id="dadce-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dadce-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dadce-118">жетсервертимезонесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="dadce-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="dadce-119">Содержит состояние и результат запроса [операции GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dadce-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dadce-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="dadce-120">Remarks</span></span>

<span data-ttu-id="dadce-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dadce-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dadce-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dadce-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dadce-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dadce-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dadce-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dadce-124">Schema Name</span></span>  <br/> |<span data-ttu-id="dadce-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dadce-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dadce-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dadce-126">Validation File</span></span>  <br/> |<span data-ttu-id="dadce-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dadce-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dadce-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dadce-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="dadce-129">False</span><span class="sxs-lookup"><span data-stu-id="dadce-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dadce-130">См. также</span><span class="sxs-lookup"><span data-stu-id="dadce-130">See also</span></span>



- [<span data-ttu-id="dadce-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dadce-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

