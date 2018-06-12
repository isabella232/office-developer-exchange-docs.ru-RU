---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: Элемент AlternatePublicFolderItemId описывает идентификатор элемента общей папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761376"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="a7d49-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="a7d49-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="a7d49-105">Элемент **AlternatePublicFolderItemId** описывает идентификатор элемента общей папки для преобразования в другой формат идентификатора.</span><span class="sxs-lookup"><span data-stu-id="a7d49-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="a7d49-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a7d49-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="a7d49-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="a7d49-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="a7d49-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="a7d49-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="a7d49-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="a7d49-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="a7d49-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="a7d49-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7d49-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7d49-111">Attributes and elements</span></span>

<span data-ttu-id="a7d49-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a7d49-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7d49-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7d49-113">Attributes</span></span>

|<span data-ttu-id="a7d49-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a7d49-114">**Attribute**</span></span>|<span data-ttu-id="a7d49-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7d49-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7d49-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="a7d49-116">FolderId</span></span>  <br/> |<span data-ttu-id="a7d49-117">Определяет общую папку, содержащую элемент общей папки.</span><span class="sxs-lookup"><span data-stu-id="a7d49-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="a7d49-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a7d49-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a7d49-119">Формат</span><span class="sxs-lookup"><span data-stu-id="a7d49-119">Format</span></span>  <br/> |<span data-ttu-id="a7d49-120">Определяет формат, который описывает идентификатор элемента общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="a7d49-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="a7d49-121">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a7d49-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a7d49-122">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="a7d49-122">ItemId</span></span>  <br/> |<span data-ttu-id="a7d49-123">Идентификатор элемента общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="a7d49-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="a7d49-124">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a7d49-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="a7d49-125">Значения атрибутов формата</span><span class="sxs-lookup"><span data-stu-id="a7d49-125">Format attribute values</span></span>

|<span data-ttu-id="a7d49-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a7d49-126">**Value**</span></span>|<span data-ttu-id="a7d49-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7d49-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7d49-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="a7d49-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="a7d49-129">Описываются идентификаторы, которые создаются веб-служб Exchange в первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="a7d49-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="a7d49-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="a7d49-130">EwsId</span></span>  <br/> |<span data-ttu-id="a7d49-131">Описываются идентификаторы, которые создаются веб-служб Exchange, начиная с Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a7d49-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="a7d49-132">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="a7d49-132">EntryId</span></span>  <br/> |<span data-ttu-id="a7d49-133">Описываются идентификаторы MAPI, как и свойство PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="a7d49-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="a7d49-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="a7d49-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="a7d49-135">Описывает представление шестнадцатеричном формате PR_ENTRYID свойства.</span><span class="sxs-lookup"><span data-stu-id="a7d49-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="a7d49-136">Это формат идентификаторы событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="a7d49-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="a7d49-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="a7d49-137">StoreId</span></span>  <br/> |<span data-ttu-id="a7d49-138">Описываются идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7d49-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="a7d49-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="a7d49-139">OwaId</span></span>  <br/> |<span data-ttu-id="a7d49-140">Описывает идентификатор Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="a7d49-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a7d49-141">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7d49-141">Child elements</span></span>

<span data-ttu-id="a7d49-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7d49-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7d49-143">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7d49-143">Parent elements</span></span>

|<span data-ttu-id="a7d49-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7d49-144">**Element**</span></span>|<span data-ttu-id="a7d49-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7d49-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7d49-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="a7d49-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="a7d49-147">Содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="a7d49-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="a7d49-148">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a7d49-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7d49-149">Замечания</span><span class="sxs-lookup"><span data-stu-id="a7d49-149">Remarks</span></span>

<span data-ttu-id="a7d49-150">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a7d49-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7d49-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7d49-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7d49-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7d49-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7d49-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7d49-153">Schema Name</span></span>  <br/> |<span data-ttu-id="a7d49-154">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a7d49-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7d49-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7d49-155">Validation File</span></span>  <br/> |<span data-ttu-id="a7d49-156">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7d49-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7d49-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7d49-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7d49-158">True</span><span class="sxs-lookup"><span data-stu-id="a7d49-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7d49-159">См. также</span><span class="sxs-lookup"><span data-stu-id="a7d49-159">See also</span></span>

- [<span data-ttu-id="a7d49-160">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="a7d49-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="a7d49-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7d49-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a7d49-162">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="a7d49-162">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

