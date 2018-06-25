---
title: OldFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: Элемент OldFolderId содержит исходный идентификатор папки, который был перемещен или скопирован.
ms.openlocfilehash: ef73cad73213a1e8b5341907cd22177d8e1ba628
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834645"
---
# <a name="oldfolderid"></a><span data-ttu-id="46f82-103">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="46f82-103">OldFolderId</span></span>

<span data-ttu-id="46f82-104">Элемент **OldFolderId** содержит исходный идентификатор папки, который был перемещен или скопирован.</span><span class="sxs-lookup"><span data-stu-id="46f82-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="46f82-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="46f82-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46f82-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46f82-106">Attributes and elements</span></span>

<span data-ttu-id="46f82-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46f82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46f82-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46f82-108">Attributes</span></span>

|<span data-ttu-id="46f82-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="46f82-109">**Attribute**</span></span>|<span data-ttu-id="46f82-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46f82-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46f82-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="46f82-111">**Id**</span></span> <br/> |<span data-ttu-id="46f82-112">Содержит строку, которая определяет папке в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f82-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="46f82-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="46f82-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="46f82-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="46f82-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="46f82-115">Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии.</span><span class="sxs-lookup"><span data-stu-id="46f82-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="46f82-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="46f82-116">This attribute is optional.</span></span> <span data-ttu-id="46f82-117">Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.</span><span class="sxs-lookup"><span data-stu-id="46f82-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="46f82-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46f82-118">Child elements</span></span>

<span data-ttu-id="46f82-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="46f82-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46f82-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46f82-120">Parent elements</span></span>

|<span data-ttu-id="46f82-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46f82-121">**Element**</span></span>|<span data-ttu-id="46f82-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46f82-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46f82-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="46f82-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="46f82-124">Представляет событие, в котором копирование элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="46f82-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="46f82-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="46f82-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="46f82-126">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="46f82-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46f82-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="46f82-127">Remarks</span></span>

<span data-ttu-id="46f82-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46f82-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46f82-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46f82-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46f82-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46f82-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46f82-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46f82-131">Schema Name</span></span>  <br/> |<span data-ttu-id="46f82-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46f82-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="46f82-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46f82-133">Validation File</span></span>  <br/> |<span data-ttu-id="46f82-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46f82-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46f82-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46f82-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="46f82-136">False</span><span class="sxs-lookup"><span data-stu-id="46f82-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46f82-137">См. также</span><span class="sxs-lookup"><span data-stu-id="46f82-137">See also</span></span>



[<span data-ttu-id="46f82-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="46f82-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="46f82-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="46f82-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="46f82-140">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="46f82-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="46f82-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46f82-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

