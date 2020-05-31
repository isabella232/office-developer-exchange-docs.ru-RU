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
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762920"
---
# <a name="getservertimezones"></a><span data-ttu-id="9ebff-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="9ebff-103">GetServerTimeZones</span></span>

<span data-ttu-id="9ebff-104">Элемент **GetServerTimeZones** является корневым элементом запроса для получения определений часовых поясов с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ebff-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="9ebff-105">**жетсервертимезонестипе**</span><span class="sxs-lookup"><span data-stu-id="9ebff-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ebff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9ebff-106">Attributes and elements</span></span>

<span data-ttu-id="9ebff-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9ebff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ebff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9ebff-108">Attributes</span></span>

|<span data-ttu-id="9ebff-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9ebff-109">**Attribute**</span></span>|<span data-ttu-id="9ebff-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ebff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ebff-111">**ретурнфуллтимезонедата**</span><span class="sxs-lookup"><span data-stu-id="9ebff-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="9ebff-112">Указывает, возвращает ли [Операция GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="9ebff-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="9ebff-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9ebff-113">This attribute is optional.</span></span> <span data-ttu-id="9ebff-114">Значение по умолчанию  **true**.</span><span class="sxs-lookup"><span data-stu-id="9ebff-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="9ebff-115">Атрибут Ретурнфуллтимезонедата</span><span class="sxs-lookup"><span data-stu-id="9ebff-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="9ebff-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9ebff-116">**Value**</span></span>|<span data-ttu-id="9ebff-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ebff-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ebff-118">**относится**</span><span class="sxs-lookup"><span data-stu-id="9ebff-118">**true**</span></span> <br/> |<span data-ttu-id="9ebff-119">Получение полных определений для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="9ebff-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="9ebff-120">**значения**</span><span class="sxs-lookup"><span data-stu-id="9ebff-120">**false**</span></span> <br/> |<span data-ttu-id="9ebff-121">Возвращает только имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="9ebff-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9ebff-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9ebff-122">Child elements</span></span>

|<span data-ttu-id="9ebff-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9ebff-123">**Element**</span></span>|<span data-ttu-id="9ebff-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ebff-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ebff-125">Идентификаторы</span><span class="sxs-lookup"><span data-stu-id="9ebff-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="9ebff-126">Содержит массив идентификаторов определения часовых поясов, которые задают запрошенные определения часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="9ebff-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="9ebff-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9ebff-127">This element is optional.</span></span> <span data-ttu-id="9ebff-128">Если этот элемент не включен в запрос [операции GetServerTimeZones](getservertimezones-operation.md) , все определения часовых поясов, доступные на сервере, возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="9ebff-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ebff-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9ebff-129">Parent elements</span></span>

<span data-ttu-id="9ebff-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="9ebff-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9ebff-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="9ebff-131">Remarks</span></span>

<span data-ttu-id="9ebff-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9ebff-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ebff-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9ebff-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ebff-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9ebff-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9ebff-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9ebff-135">Schema Name</span></span>  <br/> |<span data-ttu-id="9ebff-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9ebff-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9ebff-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9ebff-137">Validation File</span></span>  <br/> |<span data-ttu-id="9ebff-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9ebff-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ebff-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9ebff-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ebff-140">False</span><span class="sxs-lookup"><span data-stu-id="9ebff-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ebff-141">См. также</span><span class="sxs-lookup"><span data-stu-id="9ebff-141">See also</span></span>



[<span data-ttu-id="9ebff-142">Операция GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="9ebff-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="9ebff-143">жетсервертимезонесреспонсе</span><span class="sxs-lookup"><span data-stu-id="9ebff-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="9ebff-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9ebff-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

