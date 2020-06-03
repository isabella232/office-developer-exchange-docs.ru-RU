---
title: Элемент (Уплоадитемтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Элемент Item представляет отдельный элемент для отправки в почтовый ящик.
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467552"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="565f3-103">Элемент (Уплоадитемтипе)</span><span class="sxs-lookup"><span data-stu-id="565f3-103">Item (UploadItemType)</span></span>

<span data-ttu-id="565f3-104">Элемент **Item** представляет отдельный элемент для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="565f3-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="565f3-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="565f3-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="565f3-106">Элементы (Нонемптяррайофуплоадитемстипе)</span><span class="sxs-lookup"><span data-stu-id="565f3-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="565f3-107">Элемент (Уплоадитемтипе)</span><span class="sxs-lookup"><span data-stu-id="565f3-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="565f3-108">**уплоадитемтипе**</span><span class="sxs-lookup"><span data-stu-id="565f3-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="565f3-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="565f3-109">Attributes and elements</span></span>

<span data-ttu-id="565f3-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="565f3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="565f3-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="565f3-111">Attributes</span></span>

|<span data-ttu-id="565f3-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="565f3-112">**Attribute**</span></span>|<span data-ttu-id="565f3-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="565f3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="565f3-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="565f3-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="565f3-115">Задает действие для отправки элемента в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="565f3-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="565f3-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="565f3-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="565f3-117">**Связанный**</span><span class="sxs-lookup"><span data-stu-id="565f3-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="565f3-118">Указывает, является ли отправленный элемент связанным с папкой.</span><span class="sxs-lookup"><span data-stu-id="565f3-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="565f3-119">Этот атрибут является логическим значением.</span><span class="sxs-lookup"><span data-stu-id="565f3-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="565f3-120">Значение **true** указывает, что элемент является элементом, связанным с папкой.</span><span class="sxs-lookup"><span data-stu-id="565f3-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="565f3-121">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="565f3-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="565f3-122">Атрибут CreateAction</span><span class="sxs-lookup"><span data-stu-id="565f3-122">CreateAction Attribute</span></span>

|<span data-ttu-id="565f3-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="565f3-123">**Value**</span></span>|<span data-ttu-id="565f3-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="565f3-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="565f3-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="565f3-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="565f3-126">Указывает, что новая копия исходного элемента будет отправлена в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="565f3-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="565f3-127">Элемент [ItemId](itemid.md) не должен присутствовать, если используется значение CreateNew.</span><span class="sxs-lookup"><span data-stu-id="565f3-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="565f3-128">В ответе возвращается идентификатор нового элемента.</span><span class="sxs-lookup"><span data-stu-id="565f3-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="565f3-129">**Обновление**</span><span class="sxs-lookup"><span data-stu-id="565f3-129">**Update**</span></span> <br/> |<span data-ttu-id="565f3-130">Указывает, что элемент, указанный с помощью элемента **ItemId** , будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="565f3-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="565f3-131">Если элемент **ItemId** отсутствует или не существует в папке, указанной с помощью элемента [ParentFolderId](parentfolderid.md) , возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="565f3-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="565f3-132">**упдатеоркреате**</span><span class="sxs-lookup"><span data-stu-id="565f3-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="565f3-133">Указывает, что сначала выполняется попытка обновления элемента.</span><span class="sxs-lookup"><span data-stu-id="565f3-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="565f3-134">Если элемент не существует в папке, указанной с помощью элемента **ParentFolderId** , создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="565f3-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="565f3-135">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="565f3-135">Child elements</span></span>

|<span data-ttu-id="565f3-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="565f3-136">**Element**</span></span>|<span data-ttu-id="565f3-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="565f3-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="565f3-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="565f3-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="565f3-139">Представляет идентификатор родительской папки, в которой создается новый элемент, или содержащая обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="565f3-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="565f3-140">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="565f3-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="565f3-141">Содержит уникальный идентификатор и ключ изменения элемента для создания или обновления в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="565f3-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="565f3-142">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="565f3-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="565f3-143">Содержит данные одного элемента для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="565f3-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="565f3-144">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="565f3-144">Parent elements</span></span>

|<span data-ttu-id="565f3-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="565f3-145">**Element**</span></span>|<span data-ttu-id="565f3-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="565f3-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="565f3-147">Элементы (Нонемптяррайофуплоадитемстипе)</span><span class="sxs-lookup"><span data-stu-id="565f3-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="565f3-148">Содержит массив элементов для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="565f3-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="565f3-149">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="565f3-149">Text value</span></span>

<span data-ttu-id="565f3-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="565f3-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="565f3-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="565f3-151">Remarks</span></span>

<span data-ttu-id="565f3-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="565f3-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="565f3-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="565f3-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="565f3-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="565f3-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="565f3-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="565f3-155">Schema Name</span></span>  <br/> |<span data-ttu-id="565f3-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="565f3-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="565f3-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="565f3-157">Validation File</span></span>  <br/> |<span data-ttu-id="565f3-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="565f3-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="565f3-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="565f3-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="565f3-160">False</span><span class="sxs-lookup"><span data-stu-id="565f3-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="565f3-161">См. также</span><span class="sxs-lookup"><span data-stu-id="565f3-161">See also</span></span>



[<span data-ttu-id="565f3-162">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="565f3-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="565f3-163">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="565f3-163">UploadItems operation</span></span>](uploaditems-operation.md)

