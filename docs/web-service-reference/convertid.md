---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: Элемент ConvertId определяет запрос на преобразование идентификаторы элементов и папок между форматы, поддерживаемые Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761825"
---
# <a name="convertid"></a><span data-ttu-id="ef39a-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ef39a-104">ConvertId</span></span>

<span data-ttu-id="ef39a-105">Элемент **ConvertId** определяет запрос на преобразование идентификаторы элементов и папок между форматы, поддерживаемые Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef39a-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="ef39a-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ef39a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="ef39a-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="ef39a-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef39a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ef39a-108">Attributes and elements</span></span>

<span data-ttu-id="ef39a-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ef39a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef39a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ef39a-110">Attributes</span></span>

|<span data-ttu-id="ef39a-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ef39a-111">**Attribute**</span></span>|<span data-ttu-id="ef39a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef39a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef39a-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="ef39a-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="ef39a-114">Описывает формат идентификатора, будут возвращены все преобразованные идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="ef39a-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="ef39a-115">Описывается DestinationFormat IdFormatType.</span><span class="sxs-lookup"><span data-stu-id="ef39a-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="ef39a-116">Атрибут DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="ef39a-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="ef39a-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ef39a-117">**Value**</span></span>|<span data-ttu-id="ef39a-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef39a-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef39a-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="ef39a-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="ef39a-120">Представляет идентификатор формата, который используется для идентификаторов веб-служб Exchange, которые предоставляются в первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="ef39a-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="ef39a-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="ef39a-121">**EwsId**</span></span> <br/> |<span data-ttu-id="ef39a-122">Представляет идентификатор формата, который используется для идентификаторов веб-служб Exchange, начиная с Exchange Server 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="ef39a-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="ef39a-123">**Идентификатор записи**</span><span class="sxs-lookup"><span data-stu-id="ef39a-123">**EntryId**</span></span> <br/> |<span data-ttu-id="ef39a-124">Представляет идентификатор MAPI, как и свойство PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="ef39a-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="ef39a-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="ef39a-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="ef39a-126">Представляет идентификатор события календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="ef39a-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="ef39a-127">Это представление шестнадцатеричном формате PR_ENTRYID свойства.</span><span class="sxs-lookup"><span data-stu-id="ef39a-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="ef39a-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="ef39a-128">**StoreId**</span></span> <br/> |<span data-ttu-id="ef39a-129">Представляет идентификатор хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef39a-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="ef39a-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="ef39a-130">**OwaId**</span></span> <br/> |<span data-ttu-id="ef39a-131">Представляет формат идентификатора Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="ef39a-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef39a-132">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ef39a-132">Child elements</span></span>

|<span data-ttu-id="ef39a-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ef39a-133">**Element**</span></span>|<span data-ttu-id="ef39a-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef39a-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef39a-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ef39a-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="ef39a-136">Содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="ef39a-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef39a-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ef39a-137">Parent elements</span></span>

<span data-ttu-id="ef39a-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="ef39a-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ef39a-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef39a-139">Remarks</span></span>

<span data-ttu-id="ef39a-140">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ef39a-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef39a-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ef39a-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef39a-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ef39a-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef39a-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ef39a-143">Schema Name</span></span>  <br/> |<span data-ttu-id="ef39a-144">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="ef39a-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="ef39a-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ef39a-145">Validation File</span></span>  <br/> |<span data-ttu-id="ef39a-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ef39a-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef39a-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ef39a-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef39a-148">False</span><span class="sxs-lookup"><span data-stu-id="ef39a-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef39a-149">См. также</span><span class="sxs-lookup"><span data-stu-id="ef39a-149">See also</span></span>



[<span data-ttu-id="ef39a-150">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="ef39a-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="ef39a-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ef39a-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ef39a-152">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="ef39a-152">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

