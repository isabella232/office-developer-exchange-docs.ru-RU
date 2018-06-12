---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: Элемент AlternatePublicFolderId описывает идентификатор общих папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761377"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="aa710-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="aa710-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="aa710-105">Элемент **AlternatePublicFolderId** описывает идентификатор общих папок для преобразования в другой формат идентификатора.</span><span class="sxs-lookup"><span data-stu-id="aa710-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="aa710-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="aa710-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="aa710-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="aa710-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="aa710-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="aa710-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="aa710-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="aa710-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="aa710-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="aa710-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa710-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa710-111">Attributes and elements</span></span>

<span data-ttu-id="aa710-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aa710-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa710-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa710-113">Attributes</span></span>

|<span data-ttu-id="aa710-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="aa710-114">**Attribute**</span></span>|<span data-ttu-id="aa710-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa710-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa710-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="aa710-116">FolderId</span></span>  <br/> |<span data-ttu-id="aa710-117">Содержит идентификатор общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="aa710-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="aa710-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="aa710-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="aa710-119">Формат</span><span class="sxs-lookup"><span data-stu-id="aa710-119">Format</span></span>  <br/> |<span data-ttu-id="aa710-120">Определяет формат, который описывает идентификатор общей папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="aa710-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="aa710-121">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="aa710-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="aa710-122">Атрибут формата</span><span class="sxs-lookup"><span data-stu-id="aa710-122">Format attribute</span></span>

|<span data-ttu-id="aa710-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="aa710-123">**Value**</span></span>|<span data-ttu-id="aa710-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa710-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa710-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="aa710-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="aa710-126">Описываются идентификаторы, которые создаются веб-служб Exchange в первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="aa710-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="aa710-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="aa710-127">EwsId</span></span>  <br/> |<span data-ttu-id="aa710-128">Описываются идентификаторы, которые создаются веб-служб Exchange, начиная с Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="aa710-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="aa710-129">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="aa710-129">EntryId</span></span>  <br/> |<span data-ttu-id="aa710-130">Описываются идентификаторы MAPI, как и свойство PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="aa710-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="aa710-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="aa710-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="aa710-132">Описывает представление шестнадцатеричном формате PR_ENTRYID свойства.</span><span class="sxs-lookup"><span data-stu-id="aa710-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="aa710-133">Это формат идентификаторы событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="aa710-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="aa710-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="aa710-134">StoreId</span></span>  <br/> |<span data-ttu-id="aa710-135">Описываются идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa710-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="aa710-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="aa710-136">OwaId</span></span>  <br/> |<span data-ttu-id="aa710-137">Описывает идентификатор Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="aa710-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa710-138">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa710-138">Child elements</span></span>

<span data-ttu-id="aa710-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa710-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa710-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa710-140">Parent elements</span></span>

|<span data-ttu-id="aa710-141">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa710-141">**Element**</span></span>|<span data-ttu-id="aa710-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa710-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa710-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="aa710-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="aa710-144">Содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="aa710-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="aa710-145">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="aa710-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="aa710-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa710-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa710-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa710-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa710-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa710-148">Schema Name</span></span>  <br/> |<span data-ttu-id="aa710-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aa710-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa710-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa710-150">Validation File</span></span>  <br/> |<span data-ttu-id="aa710-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa710-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa710-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa710-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa710-153">True</span><span class="sxs-lookup"><span data-stu-id="aa710-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa710-154">См. также</span><span class="sxs-lookup"><span data-stu-id="aa710-154">See also</span></span>

- [<span data-ttu-id="aa710-155">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="aa710-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="aa710-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aa710-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="aa710-157">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="aa710-157">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

