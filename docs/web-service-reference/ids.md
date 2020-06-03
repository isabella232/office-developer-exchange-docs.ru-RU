---
title: Идентификаторы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: Элемент ID содержит массив идентификаторов определения часовых поясов.
ms.openlocfilehash: 1c5a6974c8d3abc318ff122f3db09d8c3472dc65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457622"
---
# <a name="ids"></a><span data-ttu-id="a38c7-103">Идентификаторы</span><span class="sxs-lookup"><span data-stu-id="a38c7-103">Ids</span></span>

<span data-ttu-id="a38c7-104">Элемент **ID** содержит массив идентификаторов определения часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="a38c7-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="a38c7-105">**нонемптяррайофтимезонеидтипе**</span><span class="sxs-lookup"><span data-stu-id="a38c7-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a38c7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a38c7-106">Attributes and elements</span></span>

<span data-ttu-id="a38c7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a38c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a38c7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a38c7-108">Attributes</span></span>

<span data-ttu-id="a38c7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a38c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a38c7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a38c7-110">Child elements</span></span>

|<span data-ttu-id="a38c7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a38c7-111">**Element**</span></span>|<span data-ttu-id="a38c7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a38c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a38c7-113">ID (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="a38c7-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="a38c7-114">Элемент, определяющий отдельное определение часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a38c7-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a38c7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a38c7-115">Parent elements</span></span>

|<span data-ttu-id="a38c7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a38c7-116">**Element**</span></span>|<span data-ttu-id="a38c7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a38c7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a38c7-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="a38c7-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="a38c7-119">Определяет запрос на получение определений часовых поясов с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="a38c7-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="a38c7-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a38c7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a38c7-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a38c7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a38c7-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a38c7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a38c7-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a38c7-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a38c7-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a38c7-124">Validation File</span></span>  <br/> |<span data-ttu-id="a38c7-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a38c7-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a38c7-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a38c7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a38c7-127">False</span><span class="sxs-lookup"><span data-stu-id="a38c7-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a38c7-128">См. также</span><span class="sxs-lookup"><span data-stu-id="a38c7-128">See also</span></span>



- [<span data-ttu-id="a38c7-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a38c7-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

