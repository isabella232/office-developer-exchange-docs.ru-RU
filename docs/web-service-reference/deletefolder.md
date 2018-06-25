---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: Элемент DeleteFolder определяет запрос на удаление папки из почтового ящика в хранилище Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762036"
---
# <a name="deletefolder"></a><span data-ttu-id="54f24-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="54f24-103">DeleteFolder</span></span>

<span data-ttu-id="54f24-104">Элемент **DeleteFolder** определяет запрос на удаление папки из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="54f24-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="54f24-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="54f24-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f24-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54f24-106">Attributes and elements</span></span>

<span data-ttu-id="54f24-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54f24-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f24-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54f24-108">Attributes</span></span>

|<span data-ttu-id="54f24-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="54f24-109">**Attribute**</span></span>|<span data-ttu-id="54f24-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54f24-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54f24-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="54f24-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="54f24-112">Описывает, как удалить папку.</span><span class="sxs-lookup"><span data-stu-id="54f24-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="54f24-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="54f24-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="54f24-114">Атрибут DeleteType</span><span class="sxs-lookup"><span data-stu-id="54f24-114">DeleteType attribute</span></span>

|<span data-ttu-id="54f24-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="54f24-115">**Value**</span></span>|<span data-ttu-id="54f24-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54f24-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54f24-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="54f24-117">HardDelete</span></span>  <br/> |<span data-ttu-id="54f24-118">Папка окончательно удалить из хранилища.</span><span class="sxs-lookup"><span data-stu-id="54f24-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="54f24-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="54f24-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="54f24-120">Папка перемещается в корзину Если корзины включена.</span><span class="sxs-lookup"><span data-stu-id="54f24-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="54f24-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="54f24-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="54f24-122">Папка переносится для папки «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="54f24-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="54f24-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54f24-123">Child elements</span></span>

|<span data-ttu-id="54f24-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54f24-124">**Element**</span></span>|<span data-ttu-id="54f24-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54f24-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f24-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="54f24-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="54f24-127">Содержит массив идентификаторов папок, которые используются для определения папок, которые следует удалить.</span><span class="sxs-lookup"><span data-stu-id="54f24-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54f24-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54f24-128">Parent elements</span></span>

<span data-ttu-id="54f24-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="54f24-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="54f24-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="54f24-130">Text value</span></span>

<span data-ttu-id="54f24-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="54f24-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54f24-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="54f24-132">Remarks</span></span>

<span data-ttu-id="54f24-133">Параметры **MoveToDeletedItems** и **HardDelete** являются транзакций, это означает, что с на время завершения вызова веб-службы, базы данных переместить элемент папки «Удаленные» или окончательно удалить элемент из базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="54f24-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="54f24-134">Это поведение не зависит от MicrosoftExchange Server 2007 и Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="54f24-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="54f24-135">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="54f24-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f24-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54f24-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f24-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54f24-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54f24-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54f24-138">Schema Name</span></span>  <br/> |<span data-ttu-id="54f24-139">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="54f24-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="54f24-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54f24-140">Validation File</span></span>  <br/> |<span data-ttu-id="54f24-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54f24-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54f24-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54f24-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="54f24-143">False</span><span class="sxs-lookup"><span data-stu-id="54f24-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54f24-144">См. также</span><span class="sxs-lookup"><span data-stu-id="54f24-144">See also</span></span>

- [<span data-ttu-id="54f24-145">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="54f24-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

