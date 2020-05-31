---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: Элемент SendItem является корневым элементом в запросе на отправку элемента в хранилище Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835340"
---
# <a name="senditem"></a><span data-ttu-id="2e9bd-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="2e9bd-103">SendItem</span></span>

<span data-ttu-id="2e9bd-104">Элемент **SendItem** является корневым элементом в запросе на отправку элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="2e9bd-105">**сендитемтипе**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e9bd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2e9bd-106">Attributes and elements</span></span>

<span data-ttu-id="2e9bd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e9bd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2e9bd-108">Attributes</span></span>

|<span data-ttu-id="2e9bd-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-109">**Attribute**</span></span>|<span data-ttu-id="2e9bd-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e9bd-111">**савеитемтофолдер**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="2e9bd-112">Определяет, будет ли сохранена копия отправленного элемента.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="2e9bd-113">Действие Save зависит от значения **савеитемтофолдер** и наличия элемента [саведитемфолдерид](saveditemfolderid.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="2e9bd-114">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="2e9bd-115">Атрибут Савеитемтофолдер</span><span class="sxs-lookup"><span data-stu-id="2e9bd-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="2e9bd-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-116">**Value**</span></span>|<span data-ttu-id="2e9bd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e9bd-118">**относится**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-118">**true**</span></span> <br/> |<span data-ttu-id="2e9bd-119">Если элемент [саведитемфолдерид](saveditemfolderid.md) отсутствует, элемент сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="2e9bd-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="2e9bd-120">Если присутствует элемент [саведитемфолдерид](saveditemfolderid.md) , он сохраняется в папке, указанной элементом [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="2e9bd-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="2e9bd-121">**значения**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-121">**false**</span></span> <br/> |<span data-ttu-id="2e9bd-122">Если элемент [саведитемфолдерид](saveditemfolderid.md) отсутствует, элемент не сохраняется.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="2e9bd-123">Если присутствует элемент [саведитемфолдерид](saveditemfolderid.md) , возвращается ответ об ошибке с элементом [респонсекоде](responsecode.md) , содержащим значение **ерроринвалидсендитемсавесеттингс** .</span><span class="sxs-lookup"><span data-stu-id="2e9bd-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e9bd-124">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2e9bd-124">Child elements</span></span>

|<span data-ttu-id="2e9bd-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-125">**Element**</span></span>|<span data-ttu-id="2e9bd-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e9bd-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e9bd-127">итемидс</span><span class="sxs-lookup"><span data-stu-id="2e9bd-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="2e9bd-128">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2e9bd-129">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="2e9bd-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="2e9bd-130">Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e9bd-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2e9bd-131">Parent elements</span></span>

<span data-ttu-id="2e9bd-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2e9bd-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="2e9bd-133">Remarks</span></span>

<span data-ttu-id="2e9bd-134">При отправке элемента в папке "Отправленные" элемент удаляется, а его копия помещается в папку "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="2e9bd-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="2e9bd-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2e9bd-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e9bd-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2e9bd-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e9bd-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2e9bd-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e9bd-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2e9bd-138">Schema Name</span></span>  <br/> |<span data-ttu-id="2e9bd-139">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2e9bd-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e9bd-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2e9bd-140">Validation File</span></span>  <br/> |<span data-ttu-id="2e9bd-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2e9bd-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e9bd-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2e9bd-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e9bd-143">False</span><span class="sxs-lookup"><span data-stu-id="2e9bd-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e9bd-144">См. также</span><span class="sxs-lookup"><span data-stu-id="2e9bd-144">See also</span></span>



[<span data-ttu-id="2e9bd-145">Операция SendItem</span><span class="sxs-lookup"><span data-stu-id="2e9bd-145">SendItem operation</span></span>](senditem-operation.md)

