---
title: басешапе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: Элемент Басешапе определяет набор свойств, возвращаемых в ответе элемента или папки.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464492"
---
# <a name="baseshape"></a><span data-ttu-id="030b4-103">басешапе</span><span class="sxs-lookup"><span data-stu-id="030b4-103">BaseShape</span></span>

<span data-ttu-id="030b4-104">Элемент **басешапе** определяет набор свойств, возвращаемых в ответе элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="030b4-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="030b4-105">**дефаултшапенаместипе**</span><span class="sxs-lookup"><span data-stu-id="030b4-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="030b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="030b4-106">Attributes and elements</span></span>

<span data-ttu-id="030b4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="030b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="030b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="030b4-108">Attributes</span></span>

<span data-ttu-id="030b4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="030b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="030b4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="030b4-110">Child elements</span></span>

<span data-ttu-id="030b4-111">Нет</span><span class="sxs-lookup"><span data-stu-id="030b4-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="030b4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="030b4-112">Parent elements</span></span>

|<span data-ttu-id="030b4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="030b4-113">**Element**</span></span>|<span data-ttu-id="030b4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="030b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="030b4-115">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="030b4-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="030b4-116">Определяет свойства папки, которые необходимо включить в ответ "GetResponse Folder", "FindFolder" или "SyncFolderHierarchy".</span><span class="sxs-lookup"><span data-stu-id="030b4-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="030b4-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="030b4-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="030b4-118">итемшапе</span><span class="sxs-lookup"><span data-stu-id="030b4-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="030b4-119">Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="030b4-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="030b4-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="030b4-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="030b4-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="030b4-121">Text value</span></span>

<span data-ttu-id="030b4-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="030b4-122">A text value is required.</span></span> <span data-ttu-id="030b4-123">В приведенной ниже таблице перечислены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="030b4-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="030b4-124">**Текстовые значения для элемента Басешапе**</span><span class="sxs-lookup"><span data-stu-id="030b4-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="030b4-125">**Значение**</span><span class="sxs-lookup"><span data-stu-id="030b4-125">**Value**</span></span>|<span data-ttu-id="030b4-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="030b4-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="030b4-127">идонли</span><span class="sxs-lookup"><span data-stu-id="030b4-127">IdOnly</span></span>  <br/> |<span data-ttu-id="030b4-128">Возвращает только идентификатор элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="030b4-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="030b4-129">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="030b4-129">Default</span></span>  <br/> |<span data-ttu-id="030b4-130">Возвращает набор свойств, которые определены как значения по умолчанию для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="030b4-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="030b4-131">аллпропертиес</span><span class="sxs-lookup"><span data-stu-id="030b4-131">AllProperties</span></span>  <br/> |<span data-ttu-id="030b4-132">Возвращает все свойства, используемые уровнем бизнес-логики Exchange для создания папки.</span><span class="sxs-lookup"><span data-stu-id="030b4-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="030b4-133">В следующей таблице перечислены свойства по умолчанию, которые возвращаются для запроса FindFolder.</span><span class="sxs-lookup"><span data-stu-id="030b4-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="030b4-134">Все подпапки данной папки возвращаются в порядке по имени.</span><span class="sxs-lookup"><span data-stu-id="030b4-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="030b4-135">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="030b4-135">**Default properties**</span></span>

|<span data-ttu-id="030b4-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="030b4-136">**Folder**</span></span>|<span data-ttu-id="030b4-137">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="030b4-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="030b4-138">Inbox;</span><span class="sxs-lookup"><span data-stu-id="030b4-138">Inbox</span></span>  <br/> |<span data-ttu-id="030b4-139">FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений</span><span class="sxs-lookup"><span data-stu-id="030b4-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-140">Контакты</span><span class="sxs-lookup"><span data-stu-id="030b4-140">Contacts</span></span>  <br/> |<span data-ttu-id="030b4-141">FolderId, отображаемое имя, общее количество, число вложенных папок</span><span class="sxs-lookup"><span data-stu-id="030b4-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-142">Календарь</span><span class="sxs-lookup"><span data-stu-id="030b4-142">Calendar</span></span>  <br/> |<span data-ttu-id="030b4-143">FolderId, отображаемое имя, число вложенных папок</span><span class="sxs-lookup"><span data-stu-id="030b4-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-144">Черновики</span><span class="sxs-lookup"><span data-stu-id="030b4-144">Drafts</span></span>  <br/> |<span data-ttu-id="030b4-145">FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений</span><span class="sxs-lookup"><span data-stu-id="030b4-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-146">Удаленные элементы</span><span class="sxs-lookup"><span data-stu-id="030b4-146">Deleted items</span></span>  <br/> |<span data-ttu-id="030b4-147">FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений</span><span class="sxs-lookup"><span data-stu-id="030b4-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-148">Другие папки</span><span class="sxs-lookup"><span data-stu-id="030b4-148">Other folders</span></span>  <br/> |<span data-ttu-id="030b4-149">FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений</span><span class="sxs-lookup"><span data-stu-id="030b4-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-150">Исходящие</span><span class="sxs-lookup"><span data-stu-id="030b4-150">Outbox</span></span>  <br/> |<span data-ttu-id="030b4-151">FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений</span><span class="sxs-lookup"><span data-stu-id="030b4-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-152">Задачи</span><span class="sxs-lookup"><span data-stu-id="030b4-152">Tasks</span></span>  <br/> |<span data-ttu-id="030b4-153">FolderId, отображаемое имя, количество просроченных, общее количество, число вложенных папок</span><span class="sxs-lookup"><span data-stu-id="030b4-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="030b4-154">Примечания</span><span class="sxs-lookup"><span data-stu-id="030b4-154">Notes</span></span>  <br/> |<span data-ttu-id="030b4-155">FolderId, отображаемое имя, общее количество, число вложенных папок</span><span class="sxs-lookup"><span data-stu-id="030b4-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="030b4-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="030b4-156">Remarks</span></span>

<span data-ttu-id="030b4-157">Чтобы вернуть свойства в дополнение к элементам, идентифицируемым элементом [басешапе](baseshape.md) , используйте элемент [аддитионалпропертиес](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="030b4-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="030b4-158">Пример</span><span class="sxs-lookup"><span data-stu-id="030b4-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="030b4-159">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="030b4-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="030b4-160">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="030b4-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="030b4-161">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="030b4-161">Schema Name</span></span>  <br/> |<span data-ttu-id="030b4-162">Схема Types</span><span class="sxs-lookup"><span data-stu-id="030b4-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="030b4-163">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="030b4-163">Validation File</span></span>  <br/> |<span data-ttu-id="030b4-164">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="030b4-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="030b4-165">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="030b4-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="030b4-166">False</span><span class="sxs-lookup"><span data-stu-id="030b4-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="030b4-167">См. также</span><span class="sxs-lookup"><span data-stu-id="030b4-167">See also</span></span>

- [<span data-ttu-id="030b4-168">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="030b4-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="030b4-169">итемшапе</span><span class="sxs-lookup"><span data-stu-id="030b4-169">ItemShape</span></span>](itemshape.md)

