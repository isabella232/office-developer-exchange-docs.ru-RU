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
description: Элемент ConvertId определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемами форматами Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452540"
---
# <a name="convertid"></a><span data-ttu-id="0913d-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="0913d-104">ConvertId</span></span>

<span data-ttu-id="0913d-105">Элемент **ConvertId** определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемами форматами Exchange.</span><span class="sxs-lookup"><span data-stu-id="0913d-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="0913d-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0913d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="0913d-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="0913d-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0913d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0913d-108">Attributes and elements</span></span>

<span data-ttu-id="0913d-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0913d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0913d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0913d-110">Attributes</span></span>

|<span data-ttu-id="0913d-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0913d-111">**Attribute**</span></span>|<span data-ttu-id="0913d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0913d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0913d-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="0913d-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="0913d-114">Описывает формат идентификатора, который будет возвращен для всех преобразованных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="0913d-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="0913d-115">DestinationFormat описывается с помощью IdFormatType.</span><span class="sxs-lookup"><span data-stu-id="0913d-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="0913d-116">Атрибут DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="0913d-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="0913d-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0913d-117">**Value**</span></span>|<span data-ttu-id="0913d-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0913d-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0913d-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="0913d-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="0913d-120">Представляет формат идентификатора, используемый для идентификаторов веб-служб Exchange, предоставленных в первоначальной версии выпуска Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="0913d-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="0913d-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="0913d-121">**EwsId**</span></span> <br/> |<span data-ttu-id="0913d-122">Представляет формат идентификатора, используемый для идентификаторов веб-служб Exchange, начиная с Exchange Server 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0913d-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="0913d-123">**EntryId**</span><span class="sxs-lookup"><span data-stu-id="0913d-123">**EntryId**</span></span> <br/> |<span data-ttu-id="0913d-124">Представляет идентификатор MAPI, как в свойстве PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="0913d-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="0913d-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="0913d-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="0913d-126">Представляет идентификатор события календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="0913d-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="0913d-127">Это представление свойства, закодированное в PR_ENTRYID кодировки.</span><span class="sxs-lookup"><span data-stu-id="0913d-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="0913d-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="0913d-128">**StoreId**</span></span> <br/> |<span data-ttu-id="0913d-129">Представляет идентификатор магазина Exchange.</span><span class="sxs-lookup"><span data-stu-id="0913d-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="0913d-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="0913d-130">**OwaId**</span></span> <br/> |<span data-ttu-id="0913d-131">Представляет формат идентификатора Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="0913d-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0913d-132">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0913d-132">Child elements</span></span>

|<span data-ttu-id="0913d-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0913d-133">**Element**</span></span>|<span data-ttu-id="0913d-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0913d-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0913d-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="0913d-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="0913d-136">Содержит идентификаторы источника, которые необходимо преобразовать.</span><span class="sxs-lookup"><span data-stu-id="0913d-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0913d-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0913d-137">Parent elements</span></span>

<span data-ttu-id="0913d-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="0913d-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0913d-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="0913d-139">Remarks</span></span>

<span data-ttu-id="0913d-140">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0913d-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0913d-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0913d-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0913d-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0913d-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0913d-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0913d-143">Schema Name</span></span>  <br/> |<span data-ttu-id="0913d-144">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="0913d-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="0913d-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0913d-145">Validation File</span></span>  <br/> |<span data-ttu-id="0913d-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0913d-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0913d-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0913d-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="0913d-148">False</span><span class="sxs-lookup"><span data-stu-id="0913d-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0913d-149">См. также</span><span class="sxs-lookup"><span data-stu-id="0913d-149">See also</span></span>



[<span data-ttu-id="0913d-150">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="0913d-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="0913d-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0913d-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0913d-152">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="0913d-152">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

