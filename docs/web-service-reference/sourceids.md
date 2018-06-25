---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: Элемент SourceIds содержит идентификаторы источника для преобразования.
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835522"
---
# <a name="sourceids"></a><span data-ttu-id="682ae-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="682ae-103">SourceIds</span></span>

<span data-ttu-id="682ae-104">Элемент **SourceIds** содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="682ae-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="682ae-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="682ae-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="682ae-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="682ae-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="682ae-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="682ae-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="682ae-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="682ae-108">Attributes and elements</span></span>

<span data-ttu-id="682ae-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="682ae-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="682ae-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="682ae-110">Attributes</span></span>

<span data-ttu-id="682ae-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="682ae-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="682ae-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="682ae-112">Child elements</span></span>

|<span data-ttu-id="682ae-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="682ae-113">**Element**</span></span>|<span data-ttu-id="682ae-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="682ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="682ae-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="682ae-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="682ae-116">Описывает идентификатор элемента или папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="682ae-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="682ae-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="682ae-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="682ae-118">Описывает идентификатор общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="682ae-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="682ae-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="682ae-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="682ae-120">Описывает идентификатор элемента общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="682ae-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="682ae-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="682ae-121">Parent elements</span></span>

|<span data-ttu-id="682ae-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="682ae-122">**Element**</span></span>|<span data-ttu-id="682ae-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="682ae-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="682ae-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="682ae-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="682ae-125">Определяет запрос на преобразование идентификаторы элементов и папок между Exchange поддерживаемые форматы.</span><span class="sxs-lookup"><span data-stu-id="682ae-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="682ae-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="682ae-126">Remarks</span></span>

<span data-ttu-id="682ae-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="682ae-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="682ae-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="682ae-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="682ae-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="682ae-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="682ae-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="682ae-130">Schema Name</span></span>  <br/> |<span data-ttu-id="682ae-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="682ae-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="682ae-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="682ae-132">Validation File</span></span>  <br/> |<span data-ttu-id="682ae-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="682ae-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="682ae-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="682ae-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="682ae-135">False</span><span class="sxs-lookup"><span data-stu-id="682ae-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="682ae-136">См. также</span><span class="sxs-lookup"><span data-stu-id="682ae-136">See also</span></span>



[<span data-ttu-id="682ae-137">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="682ae-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="682ae-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="682ae-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="682ae-139">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="682ae-139">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

