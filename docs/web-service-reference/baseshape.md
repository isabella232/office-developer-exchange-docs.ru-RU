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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761555"
---
# <a name="baseshape"></a><span data-ttu-id="7391f-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="7391f-103">BaseShape</span></span>

<span data-ttu-id="7391f-104">Элемент **BaseShape** определяет набор свойств, чтобы вернуться в элемент или папку ответ.</span><span class="sxs-lookup"><span data-stu-id="7391f-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="7391f-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="7391f-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7391f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7391f-106">Attributes and elements</span></span>

<span data-ttu-id="7391f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7391f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7391f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7391f-108">Attributes</span></span>

<span data-ttu-id="7391f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7391f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7391f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7391f-110">Child elements</span></span>

<span data-ttu-id="7391f-111">Нет</span><span class="sxs-lookup"><span data-stu-id="7391f-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7391f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7391f-112">Parent elements</span></span>

|<span data-ttu-id="7391f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7391f-113">**Element**</span></span>|<span data-ttu-id="7391f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7391f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7391f-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="7391f-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="7391f-116">Задает свойства папки для включения в ответе GetFolder, FindFolder или SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="7391f-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="7391f-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7391f-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="7391f-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7391f-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="7391f-119">Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="7391f-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="7391f-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7391f-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7391f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7391f-121">Text value</span></span>

<span data-ttu-id="7391f-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7391f-122">A text value is required.</span></span> <span data-ttu-id="7391f-123">В следующей таблице перечислены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="7391f-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="7391f-124">**Текстовые значения для элемента BaseShape**</span><span class="sxs-lookup"><span data-stu-id="7391f-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="7391f-125">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7391f-125">**Value**</span></span>|<span data-ttu-id="7391f-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7391f-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7391f-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="7391f-127">IdOnly</span></span>  <br/> |<span data-ttu-id="7391f-128">Возвращает только идентификатор элемента или папки</span><span class="sxs-lookup"><span data-stu-id="7391f-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="7391f-129">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="7391f-129">Default</span></span>  <br/> |<span data-ttu-id="7391f-130">Возвращает набор свойств, которые определены по умолчанию для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="7391f-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="7391f-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="7391f-131">AllProperties</span></span>  <br/> |<span data-ttu-id="7391f-132">Возвращает все свойства, используемые уровнем бизнес-логики Exchange для создания папки.</span><span class="sxs-lookup"><span data-stu-id="7391f-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="7391f-133">В следующей таблице приведены свойства по умолчанию, возвращенных по запросу FindFolder.</span><span class="sxs-lookup"><span data-stu-id="7391f-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="7391f-134">Все вложенные папки указанной папки возвращаются в порядке по имени.</span><span class="sxs-lookup"><span data-stu-id="7391f-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="7391f-135">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="7391f-135">**Default properties**</span></span>

|<span data-ttu-id="7391f-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="7391f-136">**Folder**</span></span>|<span data-ttu-id="7391f-137">**Свойства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="7391f-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7391f-138">Inbox</span><span class="sxs-lookup"><span data-stu-id="7391f-138">Inbox</span></span>  <br/> |<span data-ttu-id="7391f-139">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-140">Контакты</span><span class="sxs-lookup"><span data-stu-id="7391f-140">Contacts</span></span>  <br/> |<span data-ttu-id="7391f-141">FolderId, отображаемое имя, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-142">Календарь</span><span class="sxs-lookup"><span data-stu-id="7391f-142">Calendar</span></span>  <br/> |<span data-ttu-id="7391f-143">FolderId, отображаемое имя вложенной папке count</span><span class="sxs-lookup"><span data-stu-id="7391f-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-144">���������</span><span class="sxs-lookup"><span data-stu-id="7391f-144">Drafts</span></span>  <br/> |<span data-ttu-id="7391f-145">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-146">"Удаленные"</span><span class="sxs-lookup"><span data-stu-id="7391f-146">Deleted items</span></span>  <br/> |<span data-ttu-id="7391f-147">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-148">Другие папки</span><span class="sxs-lookup"><span data-stu-id="7391f-148">Other folders</span></span>  <br/> |<span data-ttu-id="7391f-149">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-150">Исходящие</span><span class="sxs-lookup"><span data-stu-id="7391f-150">Outbox</span></span>  <br/> |<span data-ttu-id="7391f-151">FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-152">Задачи</span><span class="sxs-lookup"><span data-stu-id="7391f-152">Tasks</span></span>  <br/> |<span data-ttu-id="7391f-153">FolderId, отображаемое имя просроченных count, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7391f-154">����������</span><span class="sxs-lookup"><span data-stu-id="7391f-154">Notes</span></span>  <br/> |<span data-ttu-id="7391f-155">FolderId, отображаемое имя, общее число, число вложенной папке</span><span class="sxs-lookup"><span data-stu-id="7391f-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7391f-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="7391f-156">Remarks</span></span>

<span data-ttu-id="7391f-157">Чтобы вернуть свойства помимо тех, обнаруженных в элементе [BaseShape](baseshape.md) , используйте элемент [AdditionalProperties](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="7391f-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="7391f-158">Пример</span><span class="sxs-lookup"><span data-stu-id="7391f-158">Example</span></span>

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

## <a name="element-information"></a><span data-ttu-id="7391f-159">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7391f-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7391f-160">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7391f-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7391f-161">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7391f-161">Schema Name</span></span>  <br/> |<span data-ttu-id="7391f-162">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7391f-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="7391f-163">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7391f-163">Validation File</span></span>  <br/> |<span data-ttu-id="7391f-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7391f-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7391f-165">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7391f-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="7391f-166">False</span><span class="sxs-lookup"><span data-stu-id="7391f-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7391f-167">См. также</span><span class="sxs-lookup"><span data-stu-id="7391f-167">See also</span></span>

- [<span data-ttu-id="7391f-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="7391f-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="7391f-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7391f-169">ItemShape</span></span>](itemshape.md)

