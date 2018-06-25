---
title: BaseShape
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
description: Элемент BaseShape определяет набор свойств, чтобы вернуться в элемент или папку ответ.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761555"
---
# <a name="baseshape"></a><span data-ttu-id="64a30-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="64a30-103">BaseShape</span></span>

<span data-ttu-id="64a30-104">Элемент **BaseShape** определяет набор свойств, чтобы вернуться в элемент или папку ответ.</span><span class="sxs-lookup"><span data-stu-id="64a30-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="64a30-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="64a30-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64a30-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64a30-106">Attributes and elements</span></span>

<span data-ttu-id="64a30-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="64a30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64a30-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64a30-108">Attributes</span></span>

<span data-ttu-id="64a30-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="64a30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64a30-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64a30-110">Child elements</span></span>

<span data-ttu-id="64a30-111">Нет</span><span class="sxs-lookup"><span data-stu-id="64a30-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64a30-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64a30-112">Parent elements</span></span>

|<span data-ttu-id="64a30-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64a30-113">**Element**</span></span>|<span data-ttu-id="64a30-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64a30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64a30-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="64a30-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="64a30-116">Задает свойства папки для включения в ответе GetFolder, FindFolder или SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="64a30-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="64a30-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="64a30-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="64a30-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="64a30-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="64a30-119">Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="64a30-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="64a30-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="64a30-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64a30-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64a30-121">Text value</span></span>

<span data-ttu-id="64a30-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="64a30-122">A text value is required.</span></span> <span data-ttu-id="64a30-123">В следующей таблице перечислены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="64a30-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="64a30-124">**Текстовые значения для элемента BaseShape**</span><span class="sxs-lookup"><span data-stu-id="64a30-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="64a30-125">**Значение**</span><span class="sxs-lookup"><span data-stu-id="64a30-125">**Value**</span></span>|<span data-ttu-id="64a30-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64a30-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64a30-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="64a30-127">IdOnly</span></span>  <br/> |<span data-ttu-id="64a30-128">Возвращает только идентификатор элемента или папки</span><span class="sxs-lookup"><span data-stu-id="64a30-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="64a30-129">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="64a30-129">Default</span></span>  <br/> |<span data-ttu-id="64a30-130">Возвращает набор свойств, которые определены по умолчанию для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="64a30-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="64a30-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="64a30-131">AllProperties</span></span>  <br/> |<span data-ttu-id="64a30-132">Возвращает все свойства, используемые уровнем бизнес-логики Exchange для создания папки.</span><span class="sxs-lookup"><span data-stu-id="64a30-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="64a30-133">В следующей таблице приведены свойства по умолчанию, возвращенных по запросу FindFolder.</span><span class="sxs-lookup"><span data-stu-id="64a30-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="64a30-134">Все вложенные папки указанной папки возвращаются в порядке по имени.</span><span class="sxs-lookup"><span data-stu-id="64a30-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="64a30-135">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="64a30-135">**Default properties**</span></span>

|<span data-ttu-id="64a30-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="64a30-136">**Folder**</span></span>|<span data-ttu-id="64a30-137">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="64a30-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64a30-138">Inbox</span><span class="sxs-lookup"><span data-stu-id="64a30-138">Inbox</span></span>  <br/> |<span data-ttu-id="64a30-139">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-140">Контакты</span><span class="sxs-lookup"><span data-stu-id="64a30-140">Contacts</span></span>  <br/> |<span data-ttu-id="64a30-141">FolderId, отображаемое имя, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-142">Календарь</span><span class="sxs-lookup"><span data-stu-id="64a30-142">Calendar</span></span>  <br/> |<span data-ttu-id="64a30-143">FolderId, отображаемое имя вложенной папке count</span><span class="sxs-lookup"><span data-stu-id="64a30-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-144">���������</span><span class="sxs-lookup"><span data-stu-id="64a30-144">Drafts</span></span>  <br/> |<span data-ttu-id="64a30-145">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-146">"Удаленные"</span><span class="sxs-lookup"><span data-stu-id="64a30-146">Deleted items</span></span>  <br/> |<span data-ttu-id="64a30-147">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-148">Другие папки</span><span class="sxs-lookup"><span data-stu-id="64a30-148">Other folders</span></span>  <br/> |<span data-ttu-id="64a30-149">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-150">Исходящие</span><span class="sxs-lookup"><span data-stu-id="64a30-150">Outbox</span></span>  <br/> |<span data-ttu-id="64a30-151">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-152">Задачи</span><span class="sxs-lookup"><span data-stu-id="64a30-152">Tasks</span></span>  <br/> |<span data-ttu-id="64a30-153">FolderId, отображаемое имя просроченных count, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="64a30-154">����������</span><span class="sxs-lookup"><span data-stu-id="64a30-154">Notes</span></span>  <br/> |<span data-ttu-id="64a30-155">FolderId, отображаемое имя, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="64a30-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64a30-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="64a30-156">Remarks</span></span>

<span data-ttu-id="64a30-157">Чтобы вернуть свойства помимо тех, обнаруженных в элементе [BaseShape](baseshape.md) , используйте элемент [AdditionalProperties](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="64a30-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="64a30-158">Пример</span><span class="sxs-lookup"><span data-stu-id="64a30-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="64a30-159">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64a30-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64a30-160">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64a30-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64a30-161">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64a30-161">Schema Name</span></span>  <br/> |<span data-ttu-id="64a30-162">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64a30-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="64a30-163">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64a30-163">Validation File</span></span>  <br/> |<span data-ttu-id="64a30-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64a30-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64a30-165">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64a30-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="64a30-166">False</span><span class="sxs-lookup"><span data-stu-id="64a30-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64a30-167">См. также</span><span class="sxs-lookup"><span data-stu-id="64a30-167">See also</span></span>

- [<span data-ttu-id="64a30-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="64a30-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="64a30-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="64a30-169">ItemShape</span></span>](itemshape.md)

