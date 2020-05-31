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
description: Элемент DeleteFolder определяет запрос на удаление папок из почтового ящика в хранилище Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762036"
---
# <a name="deletefolder"></a><span data-ttu-id="7458b-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="7458b-103">DeleteFolder</span></span>

<span data-ttu-id="7458b-104">Элемент **DeleteFolder** определяет запрос на удаление папок из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7458b-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="7458b-105">**делетефолдертипе**</span><span class="sxs-lookup"><span data-stu-id="7458b-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7458b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7458b-106">Attributes and elements</span></span>

<span data-ttu-id="7458b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7458b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7458b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7458b-108">Attributes</span></span>

|<span data-ttu-id="7458b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7458b-109">**Attribute**</span></span>|<span data-ttu-id="7458b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7458b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7458b-111">**делететипе**</span><span class="sxs-lookup"><span data-stu-id="7458b-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="7458b-112">Описывает, как удаляется папка.</span><span class="sxs-lookup"><span data-stu-id="7458b-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="7458b-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7458b-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="7458b-114">Атрибут Делететипе</span><span class="sxs-lookup"><span data-stu-id="7458b-114">DeleteType attribute</span></span>

|<span data-ttu-id="7458b-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7458b-115">**Value**</span></span>|<span data-ttu-id="7458b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7458b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7458b-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="7458b-117">HardDelete</span></span>  <br/> |<span data-ttu-id="7458b-118">Папка безвозвратно удаляется из хранилища.</span><span class="sxs-lookup"><span data-stu-id="7458b-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="7458b-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="7458b-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="7458b-120">При включенной корзине папка перемещается в корзину.</span><span class="sxs-lookup"><span data-stu-id="7458b-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="7458b-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="7458b-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="7458b-122">Папка перемещается в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="7458b-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7458b-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7458b-123">Child elements</span></span>

|<span data-ttu-id="7458b-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7458b-124">**Element**</span></span>|<span data-ttu-id="7458b-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7458b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7458b-126">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="7458b-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7458b-127">Содержит массив идентификаторов папок, которые используются для идентификации папок, которые необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="7458b-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7458b-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7458b-128">Parent elements</span></span>

<span data-ttu-id="7458b-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="7458b-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7458b-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7458b-130">Text value</span></span>

<span data-ttu-id="7458b-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="7458b-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7458b-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="7458b-132">Remarks</span></span>

<span data-ttu-id="7458b-133">Параметры **MoveToDeletedItems** и **HardDelete** являются транзакционными, что означает, что по завершении вызова веб-службы база данных переместит элемент в папку "Удаленные" или окончательно удалил его из базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="7458b-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="7458b-134">Это одно и то же поведение для Майкрософт Exchange Server 2007 и Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="7458b-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="7458b-135">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7458b-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7458b-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7458b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7458b-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7458b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7458b-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7458b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7458b-139">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="7458b-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="7458b-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7458b-140">Validation File</span></span>  <br/> |<span data-ttu-id="7458b-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7458b-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7458b-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7458b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7458b-143">False</span><span class="sxs-lookup"><span data-stu-id="7458b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7458b-144">См. также</span><span class="sxs-lookup"><span data-stu-id="7458b-144">See also</span></span>

- [<span data-ttu-id="7458b-145">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="7458b-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

