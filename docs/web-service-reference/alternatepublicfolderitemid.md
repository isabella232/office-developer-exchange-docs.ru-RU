---
title: алтернатепубликфолдеритемид
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
description: Элемент Алтернатепубликфолдеритемид описывает идентификатор элемента общедоступной папки, который необходимо преобразовать в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 11a9fafec78a9bd14e4d98982fd38954d45e4d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464772"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="e0c5c-104">алтернатепубликфолдеритемид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="e0c5c-105">Элемент **алтернатепубликфолдеритемид** описывает идентификатор элемента общедоступной папки, который необходимо преобразовать в другой формат идентификатора.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="e0c5c-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e0c5c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="e0c5c-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="e0c5c-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="e0c5c-108">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="e0c5c-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="e0c5c-109">алтернатепубликфолдеритемид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="e0c5c-110">**алтернатепубликфолдеритемидтипе**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0c5c-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0c5c-111">Attributes and elements</span></span>

<span data-ttu-id="e0c5c-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0c5c-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0c5c-113">Attributes</span></span>

|<span data-ttu-id="e0c5c-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-114">**Attribute**</span></span>|<span data-ttu-id="e0c5c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0c5c-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="e0c5c-116">FolderId</span></span>  <br/> |<span data-ttu-id="e0c5c-117">Определяет общую папку, содержащую элемент общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="e0c5c-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-119">Format</span><span class="sxs-lookup"><span data-stu-id="e0c5c-119">Format</span></span>  <br/> |<span data-ttu-id="e0c5c-120">Определяет формат, описывающий идентификатор элемента общедоступной папки, который требуется преобразовать.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="e0c5c-121">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-122">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e0c5c-122">ItemId</span></span>  <br/> |<span data-ttu-id="e0c5c-123">Identifier — элемент общедоступной папки, который требуется преобразовать.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="e0c5c-124">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="e0c5c-125">Форматирование значений атрибутов</span><span class="sxs-lookup"><span data-stu-id="e0c5c-125">Format attribute values</span></span>

|<span data-ttu-id="e0c5c-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-126">**Value**</span></span>|<span data-ttu-id="e0c5c-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0c5c-128">евслегациид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="e0c5c-129">Описывает идентификаторы, созданные веб-службами Exchange в исходной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-130">евсид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-130">EwsId</span></span>  <br/> |<span data-ttu-id="e0c5c-131">Описание идентификаторов, создаваемых веб-службами Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e0c5c-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-132">Код</span><span class="sxs-lookup"><span data-stu-id="e0c5c-132">EntryId</span></span>  <br/> |<span data-ttu-id="e0c5c-133">Описывает идентификаторы MAPI, как в свойстве PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-134">хексентрид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="e0c5c-135">Описывает представление свойства PR_ENTRYID в шестнадцатеричном формате.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="e0c5c-136">Это формат идентификаторов событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="e0c5c-137">StoreId</span></span>  <br/> |<span data-ttu-id="e0c5c-138">Описывает идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="e0c5c-139">оваид</span><span class="sxs-lookup"><span data-stu-id="e0c5c-139">OwaId</span></span>  <br/> |<span data-ttu-id="e0c5c-140">Описывает идентификатор Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e0c5c-141">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0c5c-141">Child elements</span></span>

<span data-ttu-id="e0c5c-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0c5c-143">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0c5c-143">Parent elements</span></span>

|<span data-ttu-id="e0c5c-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-144">**Element**</span></span>|<span data-ttu-id="e0c5c-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0c5c-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0c5c-146">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="e0c5c-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="e0c5c-147">Содержит идентификаторы источников для преобразования.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="e0c5c-148">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e0c5c-149">Примечания</span><span class="sxs-lookup"><span data-stu-id="e0c5c-149">Remarks</span></span>

<span data-ttu-id="e0c5c-150">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e0c5c-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0c5c-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0c5c-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0c5c-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0c5c-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0c5c-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0c5c-153">Schema Name</span></span>  <br/> |<span data-ttu-id="e0c5c-154">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e0c5c-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0c5c-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0c5c-155">Validation File</span></span>  <br/> |<span data-ttu-id="e0c5c-156">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e0c5c-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0c5c-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0c5c-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0c5c-158">True</span><span class="sxs-lookup"><span data-stu-id="e0c5c-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0c5c-159">См. также</span><span class="sxs-lookup"><span data-stu-id="e0c5c-159">See also</span></span>

- [<span data-ttu-id="e0c5c-160">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="e0c5c-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="e0c5c-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0c5c-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="e0c5c-162">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="e0c5c-162">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

