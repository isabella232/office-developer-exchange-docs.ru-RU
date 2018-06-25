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
description: Элемент GetServerTimeZones является корневым элементом в запросе на получение определений часовых поясов из Exchange server.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762920"
---
# <a name="getservertimezones"></a><span data-ttu-id="46c11-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="46c11-103">GetServerTimeZones</span></span>

<span data-ttu-id="46c11-104">Элемент **GetServerTimeZones** является корневым элементом в запросе на получение определений часовых поясов из Exchange server.</span><span class="sxs-lookup"><span data-stu-id="46c11-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="46c11-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="46c11-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46c11-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46c11-106">Attributes and elements</span></span>

<span data-ttu-id="46c11-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46c11-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46c11-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46c11-108">Attributes</span></span>

|<span data-ttu-id="46c11-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="46c11-109">**Attribute**</span></span>|<span data-ttu-id="46c11-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46c11-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46c11-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="46c11-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="46c11-112">Указывает, возвращает ли [операция GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="46c11-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="46c11-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="46c11-113">This attribute is optional.</span></span> <span data-ttu-id="46c11-114">Значение по умолчанию — **true**.</span><span class="sxs-lookup"><span data-stu-id="46c11-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="46c11-115">Атрибут ReturnFullTimeZoneData</span><span class="sxs-lookup"><span data-stu-id="46c11-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="46c11-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="46c11-116">**Value**</span></span>|<span data-ttu-id="46c11-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46c11-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46c11-118">**значение true**</span><span class="sxs-lookup"><span data-stu-id="46c11-118">**true**</span></span> <br/> |<span data-ttu-id="46c11-119">Возвращает полный определения для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="46c11-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="46c11-120">**false**</span><span class="sxs-lookup"><span data-stu-id="46c11-120">**false**</span></span> <br/> |<span data-ttu-id="46c11-121">Возвращает имя и идентификатор для каждого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="46c11-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="46c11-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46c11-122">Child elements</span></span>

|<span data-ttu-id="46c11-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46c11-123">**Element**</span></span>|<span data-ttu-id="46c11-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46c11-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46c11-125">Идентификаторы</span><span class="sxs-lookup"><span data-stu-id="46c11-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="46c11-126">Содержит массив идентификаторов определения часового пояса, который задает определения запрошенный часового пояса.</span><span class="sxs-lookup"><span data-stu-id="46c11-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="46c11-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="46c11-127">This element is optional.</span></span> <span data-ttu-id="46c11-128">Если этот элемент не включен в запрос [GetServerTimeZones операции](getservertimezones-operation.md) , все определения часового пояса, доступных на сервере возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="46c11-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46c11-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46c11-129">Parent elements</span></span>

<span data-ttu-id="46c11-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="46c11-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46c11-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="46c11-131">Remarks</span></span>

<span data-ttu-id="46c11-132">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46c11-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46c11-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46c11-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46c11-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46c11-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="46c11-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46c11-135">Schema Name</span></span>  <br/> |<span data-ttu-id="46c11-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="46c11-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="46c11-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46c11-137">Validation File</span></span>  <br/> |<span data-ttu-id="46c11-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="46c11-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46c11-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46c11-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="46c11-140">False</span><span class="sxs-lookup"><span data-stu-id="46c11-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46c11-141">См. также</span><span class="sxs-lookup"><span data-stu-id="46c11-141">See also</span></span>



[<span data-ttu-id="46c11-142">Операция GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="46c11-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="46c11-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="46c11-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="46c11-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46c11-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

