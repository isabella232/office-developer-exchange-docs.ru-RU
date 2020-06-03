---
title: алтернатепубликфолдерид
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
description: Элемент Алтернатепубликфолдерид описывает идентификатор общедоступной папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 54ad663117839222ea1174cd1c25600f31aa6b43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464800"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="4e041-104">алтернатепубликфолдерид</span><span class="sxs-lookup"><span data-stu-id="4e041-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="4e041-105">Элемент **алтернатепубликфолдерид** описывает идентификатор общедоступной папки для преобразования в другой формат идентификатора.</span><span class="sxs-lookup"><span data-stu-id="4e041-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="4e041-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4e041-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="4e041-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="4e041-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="4e041-108">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="4e041-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="4e041-109">алтернатепубликфолдерид</span><span class="sxs-lookup"><span data-stu-id="4e041-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="4e041-110">**алтернатепубликфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="4e041-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e041-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4e041-111">Attributes and elements</span></span>

<span data-ttu-id="4e041-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4e041-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e041-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4e041-113">Attributes</span></span>

|<span data-ttu-id="4e041-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4e041-114">**Attribute**</span></span>|<span data-ttu-id="4e041-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e041-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e041-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="4e041-116">FolderId</span></span>  <br/> |<span data-ttu-id="4e041-117">Содержит идентификатор общедоступной папки для преобразования.</span><span class="sxs-lookup"><span data-stu-id="4e041-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="4e041-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4e041-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4e041-119">Format</span><span class="sxs-lookup"><span data-stu-id="4e041-119">Format</span></span>  <br/> |<span data-ttu-id="4e041-120">Определяет формат, описывающий преобразуемый идентификатор общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="4e041-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="4e041-121">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4e041-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="4e041-122">Атрибут Format</span><span class="sxs-lookup"><span data-stu-id="4e041-122">Format attribute</span></span>

|<span data-ttu-id="4e041-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4e041-123">**Value**</span></span>|<span data-ttu-id="4e041-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e041-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e041-125">евслегациид</span><span class="sxs-lookup"><span data-stu-id="4e041-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="4e041-126">Описывает идентификаторы, созданные веб-службами Exchange в исходной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="4e041-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="4e041-127">евсид</span><span class="sxs-lookup"><span data-stu-id="4e041-127">EwsId</span></span>  <br/> |<span data-ttu-id="4e041-128">Описание идентификаторов, создаваемых веб-службами Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4e041-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="4e041-129">Код</span><span class="sxs-lookup"><span data-stu-id="4e041-129">EntryId</span></span>  <br/> |<span data-ttu-id="4e041-130">Описывает идентификаторы MAPI, как в свойстве PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="4e041-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="4e041-131">хексентрид</span><span class="sxs-lookup"><span data-stu-id="4e041-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="4e041-132">Описывает представление свойства PR_ENTRYID в шестнадцатеричном формате.</span><span class="sxs-lookup"><span data-stu-id="4e041-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="4e041-133">Это формат идентификаторов событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="4e041-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="4e041-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="4e041-134">StoreId</span></span>  <br/> |<span data-ttu-id="4e041-135">Описывает идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e041-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="4e041-136">оваид</span><span class="sxs-lookup"><span data-stu-id="4e041-136">OwaId</span></span>  <br/> |<span data-ttu-id="4e041-137">Описывает идентификатор Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="4e041-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4e041-138">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4e041-138">Child elements</span></span>

<span data-ttu-id="4e041-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e041-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e041-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4e041-140">Parent elements</span></span>

|<span data-ttu-id="4e041-141">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e041-141">**Element**</span></span>|<span data-ttu-id="4e041-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e041-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e041-143">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="4e041-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="4e041-144">Содержит идентификаторы источников для преобразования.</span><span class="sxs-lookup"><span data-stu-id="4e041-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="4e041-145">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4e041-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4e041-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4e041-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e041-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4e041-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e041-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4e041-148">Schema Name</span></span>  <br/> |<span data-ttu-id="4e041-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4e041-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="4e041-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4e041-150">Validation File</span></span>  <br/> |<span data-ttu-id="4e041-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4e041-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e041-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4e041-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e041-153">True</span><span class="sxs-lookup"><span data-stu-id="4e041-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e041-154">См. также</span><span class="sxs-lookup"><span data-stu-id="4e041-154">See also</span></span>

- [<span data-ttu-id="4e041-155">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="4e041-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="4e041-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4e041-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="4e041-157">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="4e041-157">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

