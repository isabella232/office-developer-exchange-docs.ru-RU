---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: Элемент EmptyFolder определяет запрос, чтобы очистить папку почтового ящика в хранилище Exchange. При необходимости вложенных папок можно также удаляются при папки.
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762327"
---
# <a name="emptyfolder"></a><span data-ttu-id="2c713-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="2c713-104">EmptyFolder</span></span>

<span data-ttu-id="2c713-105">Элемент **EmptyFolder** определяет запрос, чтобы очистить папку почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c713-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="2c713-106">При необходимости вложенных папок можно также удаляются при папки.</span><span class="sxs-lookup"><span data-stu-id="2c713-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="2c713-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="2c713-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c713-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c713-108">Attributes and elements</span></span>

<span data-ttu-id="2c713-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2c713-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c713-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c713-110">Attributes</span></span>

|<span data-ttu-id="2c713-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="2c713-111">**Attribute**</span></span>|<span data-ttu-id="2c713-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c713-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c713-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="2c713-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="2c713-114">Указывает, как папки.</span><span class="sxs-lookup"><span data-stu-id="2c713-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="2c713-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2c713-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="2c713-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="2c713-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="2c713-117">Указывает, являются ли вложенные папки к удалению.</span><span class="sxs-lookup"><span data-stu-id="2c713-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="2c713-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2c713-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="2c713-119">Атрибут DeleteType</span><span class="sxs-lookup"><span data-stu-id="2c713-119">DeleteType Attribute</span></span>

|<span data-ttu-id="2c713-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2c713-120">**Value**</span></span>|<span data-ttu-id="2c713-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c713-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c713-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="2c713-122">HardDelete</span></span>  <br/> |<span data-ttu-id="2c713-123">A сообщений и папок окончательно удалить из хранилища.</span><span class="sxs-lookup"><span data-stu-id="2c713-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="2c713-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="2c713-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="2c713-125">A сообщений и папок, перемещаются в корзину Если корзина включена.</span><span class="sxs-lookup"><span data-stu-id="2c713-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="2c713-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="2c713-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="2c713-127">A сообщений и папок, перемещаются в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="2c713-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2c713-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c713-128">Child elements</span></span>

|<span data-ttu-id="2c713-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c713-129">**Element**</span></span>|<span data-ttu-id="2c713-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c713-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c713-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="2c713-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="2c713-132">Содержит массив идентификаторов папок, которые используются для определения папок, которые следует удалить.</span><span class="sxs-lookup"><span data-stu-id="2c713-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c713-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c713-133">Parent elements</span></span>

<span data-ttu-id="2c713-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c713-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2c713-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2c713-135">Text value</span></span>

<span data-ttu-id="2c713-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c713-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c713-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="2c713-137">Remarks</span></span>

<span data-ttu-id="2c713-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c713-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c713-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c713-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c713-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2c713-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2c713-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c713-141">Schema Name</span></span>  <br/> |<span data-ttu-id="2c713-142">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="2c713-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="2c713-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c713-143">Validation File</span></span>  <br/> |<span data-ttu-id="2c713-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2c713-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2c713-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c713-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c713-146">False</span><span class="sxs-lookup"><span data-stu-id="2c713-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c713-147">См. также</span><span class="sxs-lookup"><span data-stu-id="2c713-147">See also</span></span>



[<span data-ttu-id="2c713-148">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="2c713-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

