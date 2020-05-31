---
title: саурцеидс
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
description: Элемент Саурцеидс содержит идентификаторы источника для преобразования.
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835522"
---
# <a name="sourceids"></a><span data-ttu-id="11730-103">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="11730-103">SourceIds</span></span>

<span data-ttu-id="11730-104">Элемент **саурцеидс** содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="11730-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="11730-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="11730-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="11730-106">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="11730-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="11730-107">**нонемптяррайофалтернатеидстипе**</span><span class="sxs-lookup"><span data-stu-id="11730-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11730-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11730-108">Attributes and elements</span></span>

<span data-ttu-id="11730-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11730-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11730-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11730-110">Attributes</span></span>

<span data-ttu-id="11730-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="11730-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11730-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11730-112">Child elements</span></span>

|<span data-ttu-id="11730-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11730-113">**Element**</span></span>|<span data-ttu-id="11730-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11730-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11730-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="11730-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="11730-116">Описывает идентификатор элемента или папки, который требуется преобразовать.</span><span class="sxs-lookup"><span data-stu-id="11730-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="11730-117">алтернатепубликфолдерид</span><span class="sxs-lookup"><span data-stu-id="11730-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="11730-118">Описывает идентификатор общедоступной папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="11730-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="11730-119">алтернатепубликфолдеритемид</span><span class="sxs-lookup"><span data-stu-id="11730-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="11730-120">Описывает идентификатор элемента общедоступной папки, который требуется преобразовать.</span><span class="sxs-lookup"><span data-stu-id="11730-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11730-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11730-121">Parent elements</span></span>

|<span data-ttu-id="11730-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11730-122">**Element**</span></span>|<span data-ttu-id="11730-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11730-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11730-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="11730-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="11730-125">Определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемыми форматами Exchange.</span><span class="sxs-lookup"><span data-stu-id="11730-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11730-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="11730-126">Remarks</span></span>

<span data-ttu-id="11730-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="11730-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11730-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11730-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11730-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11730-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11730-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11730-130">Schema Name</span></span>  <br/> |<span data-ttu-id="11730-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="11730-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11730-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11730-132">Validation File</span></span>  <br/> |<span data-ttu-id="11730-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="11730-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11730-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11730-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="11730-135">False</span><span class="sxs-lookup"><span data-stu-id="11730-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11730-136">См. также</span><span class="sxs-lookup"><span data-stu-id="11730-136">See also</span></span>



[<span data-ttu-id="11730-137">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="11730-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="11730-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="11730-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="11730-139">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="11730-139">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

