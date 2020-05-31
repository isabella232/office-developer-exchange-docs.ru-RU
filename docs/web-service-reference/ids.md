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
ms.openlocfilehash: e4f8afb1292b3cb9f3990d4613b7461050976a59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833856"
---
# <a name="ids"></a><span data-ttu-id="bc1fc-103">Идентификаторы</span><span class="sxs-lookup"><span data-stu-id="bc1fc-103">Ids</span></span>

<span data-ttu-id="bc1fc-104">Элемент **ID** содержит массив идентификаторов определения часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="bc1fc-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="bc1fc-105">**нонемптяррайофтимезонеидтипе**</span><span class="sxs-lookup"><span data-stu-id="bc1fc-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc1fc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc1fc-106">Attributes and elements</span></span>

<span data-ttu-id="bc1fc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc1fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc1fc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc1fc-108">Attributes</span></span>

<span data-ttu-id="bc1fc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc1fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc1fc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc1fc-110">Child elements</span></span>

|<span data-ttu-id="bc1fc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc1fc-111">**Element**</span></span>|<span data-ttu-id="bc1fc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc1fc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc1fc-113">ID (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="bc1fc-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="bc1fc-114">Элемент, определяющий отдельное определение часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc1fc-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc1fc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc1fc-115">Parent elements</span></span>

|<span data-ttu-id="bc1fc-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc1fc-116">**Element**</span></span>|<span data-ttu-id="bc1fc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc1fc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc1fc-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="bc1fc-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="bc1fc-119">Определяет запрос на получение определений часовых поясов с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc1fc-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="bc1fc-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc1fc-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc1fc-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc1fc-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc1fc-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc1fc-122">Schema Name</span></span>  <br/> |<span data-ttu-id="bc1fc-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc1fc-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc1fc-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc1fc-124">Validation File</span></span>  <br/> |<span data-ttu-id="bc1fc-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc1fc-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc1fc-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc1fc-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc1fc-127">False</span><span class="sxs-lookup"><span data-stu-id="bc1fc-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc1fc-128">См. также</span><span class="sxs-lookup"><span data-stu-id="bc1fc-128">See also</span></span>



- [<span data-ttu-id="bc1fc-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc1fc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

