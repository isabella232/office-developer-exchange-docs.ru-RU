---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: Элемент GetServerTimeZones является корневым элементом запроса для получения определений часовых поясов с сервера Exchange.
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460941"
---
# <a name="getservertimezones"></a><span data-ttu-id="a367a-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="a367a-103">GetServerTimeZones</span></span>

<span data-ttu-id="a367a-104">Элемент **GetServerTimeZones** является корневым элементом запроса для получения определений часовых поясов с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="a367a-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="a367a-105">**жетсервертимезонестипе**</span><span class="sxs-lookup"><span data-stu-id="a367a-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a367a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a367a-106">Attributes and elements</span></span>

<span data-ttu-id="a367a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a367a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a367a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a367a-108">Attributes</span></span>

|<span data-ttu-id="a367a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a367a-109">**Attribute**</span></span>|<span data-ttu-id="a367a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a367a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a367a-111">**ретурнфуллтимезонедата**</span><span class="sxs-lookup"><span data-stu-id="a367a-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="a367a-112">Указывает, возвращает ли [Операция GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a367a-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="a367a-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a367a-113">This attribute is optional.</span></span> <span data-ttu-id="a367a-114">Значение по умолчанию  **true**.</span><span class="sxs-lookup"><span data-stu-id="a367a-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="a367a-115">Атрибут Ретурнфуллтимезонедата</span><span class="sxs-lookup"><span data-stu-id="a367a-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="a367a-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a367a-116">**Value**</span></span>|<span data-ttu-id="a367a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a367a-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a367a-118">**относится**</span><span class="sxs-lookup"><span data-stu-id="a367a-118">**true**</span></span> <br/> |<span data-ttu-id="a367a-119">Получение полных определений для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a367a-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="a367a-120">**значения**</span><span class="sxs-lookup"><span data-stu-id="a367a-120">**false**</span></span> <br/> |<span data-ttu-id="a367a-121">Возвращает только имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a367a-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a367a-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a367a-122">Child elements</span></span>

|<span data-ttu-id="a367a-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a367a-123">**Element**</span></span>|<span data-ttu-id="a367a-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a367a-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a367a-125">Идентификаторы</span><span class="sxs-lookup"><span data-stu-id="a367a-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="a367a-126">Содержит массив идентификаторов определения часовых поясов, которые задают запрошенные определения часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="a367a-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="a367a-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a367a-127">This element is optional.</span></span> <span data-ttu-id="a367a-128">Если этот элемент не включен в запрос [операции GetServerTimeZones](getservertimezones-operation.md) , все определения часовых поясов, доступные на сервере, возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="a367a-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a367a-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a367a-129">Parent elements</span></span>

<span data-ttu-id="a367a-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="a367a-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a367a-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="a367a-131">Remarks</span></span>

<span data-ttu-id="a367a-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a367a-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a367a-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a367a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a367a-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a367a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a367a-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a367a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a367a-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a367a-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a367a-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a367a-137">Validation File</span></span>  <br/> |<span data-ttu-id="a367a-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a367a-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a367a-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a367a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a367a-140">False</span><span class="sxs-lookup"><span data-stu-id="a367a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a367a-141">См. также</span><span class="sxs-lookup"><span data-stu-id="a367a-141">See also</span></span>



[<span data-ttu-id="a367a-142">Операция GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="a367a-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="a367a-143">жетсервертимезонесреспонсе</span><span class="sxs-lookup"><span data-stu-id="a367a-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="a367a-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a367a-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

