---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: Элемент EmptyFolder определяет запрос на очистку папки в почтовом ящике в хранилище Exchange. Кроме того, при очистке папки также можно удалить вложенные папки.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457279"
---
# <a name="emptyfolder"></a><span data-ttu-id="d0f5b-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d0f5b-104">EmptyFolder</span></span>

<span data-ttu-id="d0f5b-105">Элемент **EmptyFolder** определяет запрос на очистку папки в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="d0f5b-106">Кроме того, при очистке папки также можно удалить вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="d0f5b-107">**емптифолдертипе**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0f5b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0f5b-108">Attributes and elements</span></span>

<span data-ttu-id="d0f5b-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0f5b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d0f5b-110">Attributes</span></span>

|<span data-ttu-id="d0f5b-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-111">**Attribute**</span></span>|<span data-ttu-id="d0f5b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0f5b-113">**делететипе**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="d0f5b-114">Указывает, как очищается папка.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="d0f5b-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d0f5b-116">**делетесубфолдерс**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="d0f5b-117">Указывает, следует ли удалять подпапки.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="d0f5b-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="d0f5b-119">Атрибут Делететипе</span><span class="sxs-lookup"><span data-stu-id="d0f5b-119">DeleteType Attribute</span></span>

|<span data-ttu-id="d0f5b-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-120">**Value**</span></span>|<span data-ttu-id="d0f5b-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0f5b-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="d0f5b-122">HardDelete</span></span>  <br/> |<span data-ttu-id="d0f5b-123">Сообщения и папки безвозвратно удаляются из хранилища.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="d0f5b-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="d0f5b-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="d0f5b-125">При включенной корзине сообщения и папки перемещаются в корзину.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="d0f5b-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="d0f5b-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="d0f5b-127">Сообщения и папки перемещаются в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="d0f5b-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d0f5b-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d0f5b-128">Child elements</span></span>

|<span data-ttu-id="d0f5b-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-129">**Element**</span></span>|<span data-ttu-id="d0f5b-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0f5b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0f5b-131">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="d0f5b-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="d0f5b-132">Содержит массив идентификаторов папок, которые используются для идентификации папок, которые необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0f5b-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d0f5b-133">Parent elements</span></span>

<span data-ttu-id="d0f5b-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d0f5b-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d0f5b-135">Text value</span></span>

<span data-ttu-id="d0f5b-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0f5b-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="d0f5b-137">Remarks</span></span>

<span data-ttu-id="d0f5b-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0f5b-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0f5b-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d0f5b-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0f5b-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d0f5b-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0f5b-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d0f5b-141">Schema Name</span></span>  <br/> |<span data-ttu-id="d0f5b-142">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="d0f5b-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="d0f5b-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d0f5b-143">Validation File</span></span>  <br/> |<span data-ttu-id="d0f5b-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d0f5b-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0f5b-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d0f5b-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0f5b-146">False</span><span class="sxs-lookup"><span data-stu-id="d0f5b-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0f5b-147">См. также</span><span class="sxs-lookup"><span data-stu-id="d0f5b-147">See also</span></span>



[<span data-ttu-id="d0f5b-148">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d0f5b-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

